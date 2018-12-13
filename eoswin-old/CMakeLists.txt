cmake_minimum_required(VERSION 3.12)
project(contract)

set(CMAKE_CXX_STANDARD 14)

include_directories(.)
include_directories(blackjack)
include_directories(dice)
include_directories(jackpot)
include_directories(lottery)

add_executable(contract
        blackjack/blackjack.cpp
        blackjack/blackjack.hpp
        blackjack/random.hpp
        blackjack/token.hpp
        dice/config.hpp
        dice/dice.cpp
        dice/eosio.token.hpp
        jackpot/jackpot.cpp
        lottery/config.hpp
        lottery/lottery.cpp
        lottery/lottery.hpp
        lottery/token.cpp
        lottery/token.hpp)
