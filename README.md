# whi_move_base_msgs
Extended move_base_msgs for whi_move_base to bypass outside goals while whi_move_base is handling internal interaction goals

## Extended interaction enum
| name                     | value | stands for                                                                                        |
|--------------------------|-------|---------------------------------------------------------------------------------------------------|
| INTERACTION_NONE         | 0     | normal mode to handle goals like move_base                                                        |
| INTERACTION_BLOCK        | 1     | block goals during internal interaction and execute new arrived internal goal                     |
| INTERACTION_BLOCK_ONLY   | 2     | block goals during internal interaction                                                           |
| INTERACTION_UNBLOCK      | 3     | to unblock and accept all goals, back to normal mode. meanwhile execute new arrived internal goal |
| INTERACTION_UNBLOCK_ONLY | 4     | to unblock and accept all goals, back to normal mode                                              |
| INTERACTION_WAITBLOCK    | 5     | TBD                                                                                               |
