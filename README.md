Alpaca Project Template
=====

Just clone this project and rename the files in /src as appropriate.


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
