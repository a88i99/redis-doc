@complexity

O(N) where N is the total number of elements in all given sets.

Returns the members of the set resulting from the union of all the
given sets.

For example:

    key1 = {a,b,c,d}
    key2 = {c}
    key3 = {a,c,e}
    SUNION key1 key2 key3 = {a,b,c,d,e}

Keys that do not exist are considered to be empty sets.

@return

@multi-bulk-reply: list with members of the resulting set.

@examples

    @cli
    SADD key1 "a"
    SADD key1 "b"
    SADD key1 "c"
    SADD key2 "c"
    SADD key2 "d"
    SADD key2 "e"
    SUNION key1 key2

