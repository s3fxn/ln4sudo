# ln4sudo

ln4sudo - create a symbolic link in /sbin for easy sudo.


## Installation

    $ gem install ln4sudo
    (you may need to run as root or through sudo.)

## Usage

```
ln4sudo [-f] command...

-f  remove existing destination files

$ which gem
/usr/local/ruby2.5.1/bin/gem

$ sudo gem install ...
sudo: gem: command not found

$ ln4sudo gem
sudo ln -s /usr/local/ruby2.5.1/bin/gem /sbin

$ sudo gem install ...

config:
$ ln4sudo init /usr/local/sbin
change target directory to /usr/local/sbin
```

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/s3fxn/ln4sudo.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
