# cache-redis-config

## Description
A lightweight, flexible, and customizable Redis configuration and caching manager for Node.js applications.

## Features
* Support for Redis clustering and sentinel
* Automatic connection pooling and connection string management
* Support for multiple Redis hosts
* Advanced caching with TTL (Time To Live) and expiration rules
* Customizable cache data serialization and deserialization
* Support for Redis data types (hashes, lists, sets, maps, etc.)
* High-performance, efficient caching and data retrieval

## Technologies Used
* Node.js (14.x) and higher
* Redis (6.x) and higher
* TypeScript (for type safety and code maintainability)

## Installation

### Installation via npm
```bash
npm install cache-redis-config
```

### Installation via yarn
```bash
yarn add cache-redis-config
```

### Installation via GitHub
```bash
git clone https://github.com/your-username/cache-redis-config.git
cd cache-redis-config
npm install
```

## Quick Start
```javascript
import { CacheRedisConfig } from 'cache-redis-config';

const redisConfig = new CacheRedisConfig({
  // Redis cluster configuration
  hosts: [
    { host: 'localhost', port: 6379 },
    { host: 'localhost', port: 6380 },
    { host: 'localhost', port: 6381 },
  ],
});

// Set a simple key-value pair in cache
redisConfig.set('myKey', 'myValue', { TTL: 10000 });

// Get the value of the key from cache
const value = await redisConfig.get('myKey');

console.log(value);
```

## API Documentation
* [CacheRedisConfig](https://your-username.github.io/cache-redis-config/docs/classes/CacheRedisConfig.html)
* [CacheRedisConfig#set](https://your-username.github.io/cache-redis-config/docs/classes/CacheRedisConfig.html#set)
* [CacheRedisConfig#get](https://your-username.github.io/cache-redis-config/docs/classes/CacheRedisConfig.html#get)

## Contributing
Contributions are welcome and encouraged. Please submit a pull request to this repository with your changes and follow standard professional guidelines for code formatting and documentation.

## License
Licensed under the MIT License.

## Changelog
Check the [CHANGELOG](https://github.com/your-username/cache-redis-config/blob/main/CHANGELOG.md) file for recent changes and updates.

## Author
Your Name

## Email
your.email@example.com

## GitHub
https://github.com/your-username