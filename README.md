Alpaca Project Template
=====

Just clone this project and rename the files in /src as appropriate.

You must have Alpaca installed. This will boil down to downloading a release
and ensuring your `ALPACA_ROOT` enviromental variable is set, e.g.

    $ export ALPACA_ROOT=~/alpaca

However, Currently this template uses a branch of the rebar3 plugin 
and you'll have to build Alpaca yourself from master, e.g.

    $ git clone https://github.com/alpaca-lang/alpaca.git &&\
          cd alpaca && rebar3 compile && bash make-release.sh &&\
          cd alpaca-unversioned && export ALPACA_ROOT=$PWD
    

Build
-----

    $ rebar3 compile


Test
-----

    $ rebar3 eunit


Interact
-----
    $ rebar3 shell

    ===> Compiling alpaca_app
    Erlang/OTP 20 [erts-9.0] [source] [64-bit] [smp:4:4] [ds:4:4:10] [async-threads:0] [hipe] [kernel-poll:false] [dtrace]

    Eshell V9.0  (abort with ^G)
    1> alpaca_main:main({}).
    <<"hello world!">>
