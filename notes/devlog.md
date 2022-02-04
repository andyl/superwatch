# Superwatch 

## CLI Challenge

Wanted: getch, readline, tab completion

Notes:
- impossible with gets
- impossible with nif 
- seems impossible with port (exe can't read stdin..)
- could it be done with NCurses?  (one-line? full-screen?)
- And yet: IEx does it!

Approach:
- near term: gets-style CLI only
- long term: study IEx, emulate it's features, release as lib

## 2022 Jan 18 Tue

- [x] Drop Worker 
- [x] Rename runner to worker
- [x] Fix CaptureIO (Process Leader...)
- [x] Remove streamio from state

## 2022 Jan 19 Wed

- [x] Implement Manager as Module not Escript
- [x] Design Config and State settings
- [x] Refactor module names
- [x] Create CLI framework

## 2022 Jan 31 Mon

- [x] Short-term Elixir CLI: no tab completion

## 2022 Feb 01 Tue

- [x] add help system 
- [x] successful test with Ports launching Nvim 

## 2022 Feb 02 Wed

- [x] Make a util/editor module 
- [x] Add an editor.launch function 

## 2022 Feb 03 Thu

Overview:
- [x] read agents from config file (agent select)
- [x] read agent from config file 
- [x] read state 
- [x] write state 

Vim Work: 
- updated snippets 
- fixed Telescope MRU

Concept Work: 
- reorganized UI (agents and prefs) 
- added an API layer 
- services register with a pre-defined name - easier testing
- changed prefs from a map to a list

## TODO

Commands:
- [x] run 
- [x] agent list 
- [x] agent edit 
- [ ] agent select 
- [ ] prefs show 
- [x] prefs edit 
- [ ] prefs reset 
- [ ] exit 
- [ ] help

Features: 
- [ ] Reload after Agent Edit 
- [ ] Reload after Prefs Edit
- [ ] Update prefs after Agent Select 
- [ ] Implement PrefsShow 
- [ ] Implement PrefsReset
- [ ] Validate Agent format (use ecto?)
- [ ] Validate Prefs formatting (use ecto?) 

Release:
- [ ] Add release config 
- [ ] Add Burrito config 
- [ ] Create release page with burrito executables

Long Term:
- [ ] Add tab completion
