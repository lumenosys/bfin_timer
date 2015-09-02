bfin_timer
===

**bfin_timer** is an Erlang driver for accessing the timer devices on the Analog Devices Blackfin processor. This driver can be used by applications that need to do things like control servos, generate pulses, flash LEDs, measure pulse widths, etc., on the Lumenosys Robotics [BMOD][1] board.

Dependencies
------------

To build you will need a working installation of Erlang 17 (or
later). <br/>
Please refer to [Erlang/OTP](http://www.erlang.org) for information on building and installing Erlang/OTP.

This application is built using [rebar](https://github.com/rebar/rebar). Refer to [building rebar](https://github.com/rebar/rebar/wiki/Building-rebar) for information on building and using rebar.

Downloading
-----------

```sh
$ git clone git://github.com/lumenosys/bfin_timer.git
```
Building
--------

Compile:

```sh
$ cd bfin_timer
$ make all
...
==> bfin_timer (compile)
```

Usage example
-------------

```sh
$ export ERL_LIBS=/path/to/bfin_timer
$ erl -sname master@local -setcookie lumenosys -boot start_sasl -eval "application:start(bfin_timer)"
```

Copyright and License
---------------------

> %CopyrightBegin%
>
> Copyright Lumenosys Robotics 2014-2015. All Rights Reserved.
>
> Licensed under the Apache License, Version 2.0 (the "License");
> you may not use this file except in compliance with the License.
> You may obtain a copy of the License at
>
>     http://www.apache.org/licenses/LICENSE-2.0
>
> Unless required by applicable law or agreed to in writing, software
> distributed under the License is distributed on an "AS IS" BASIS,
> WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
> See the License for the specific language governing permissions and
> limitations under the License.
>
> %CopyrightEnd%


[1]: https://lumenosys.com/products