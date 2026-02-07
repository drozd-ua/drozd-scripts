#!/usr/bin/env bash

# pick a random action
actions=(
  "open_editor"
  "write_random_file"
  "list_home"
  "show_datetime"
  "open_browser"
)

pick=${actions[$RANDOM % ${#actions[@]}]}

open_editor() {
  xdg-open .
}

write_random_file() {
  file="/tmp/random_$(date +%s).txt"
  echo "random number: $RANDOM" > "$file"
  echo "created $file"
}

list_home() {
  ls -1 ~
}

show_datetime() {
  date
}

open_browser() {
  xdg-open "https://goto"
}

$pick
