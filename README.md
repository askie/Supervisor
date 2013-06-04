# Supervisor [![Build Status](https://secure.travis-ci.org/yzalis/Supervisor.png)](http://travis-ci.org/yzalis/Supervisor)

**Supervisor** is a library which helps you to manage your supervisor instance.

## Basic Usage

Create a new Supervisor instance
```php
$supervisor = new \Supervisor\Supervisor('Server #1', '127.0.0.1', 'username', 'password', '9001');
```

List all processes
```php
$processes = $supervisor->getProcesses();
foreach ($processes as $process) {
    // ...
    echo $process->getName();
    // ...
}
```

Please check the `Supervisor\Supervisor` and `Supervisor\Process` classes for listing all available methods.

## Unit Tests

To run unit tests, you'll need a set of dependencies you can install using Composer:
```
php composer.phar install
```

Once installed, just launch the following command:
```
phpunit
```

You're done.

## Credits

* Benjamin Laugueux <benjamin@yzalis.com>
* [All contributors](https://github.com/yzalis/Supervisor/contributors)

Thanks for providing a huge amount of data to run tests:
* [http://user-agent-string.info](http://user-agent-string.info)
* [http://www.useragentstring.com](http://www.useragentstring.com)

## License

Supervisor is released under the MIT License. See the bundled LICENSE file for details.