# pyRCV

Standalone Python 3 scripts for counting various preferential voting elections, including:

* [Wright STV](http://www.aph.gov.au/Parliamentary_Business/Committees/House_of_Representatives_Committees?url=/em/elect07/subs/sub051.1.pdf)
* Single Transferable Vote (weighted inclusive Gregory)
* Instant Runoff Voting (aka. the Alternative Vote)

Like preferential voting? Why not check out [helios-server-mixnet](https://github.com/RunasSudo/helios-server-mixnet), an end-to-end voter verifiable online voting system which supports preferential voting?

## wright_stv.py

    ./wright_stv.py election.json result.json 2

Takes as input a JSON file containing the [raw Helios data for an election](https://helios.example.com/helios/elections/12345678-90ab-cdef-1234-567890abcdef), the [raw result](https://helios.example.com/helios/elections/12345678-90ab-cdef-1234-567890abcdef/result) and the number of seats to be filled, and calculates the winners under Wright STV.
