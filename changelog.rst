Changelog
=========

v0.8.0 (2017-05-09)
-------------------

Fix
~~~

- Bugfix: use start_time instead of time_slot in satpy_writer. [Martin
  Raspaud]

Other
~~~~~

- Update changelog. [Panu Lahtinen]

- Bump version: 0.7.0 → 0.8.0. [Panu Lahtinen]

- Bugfix satpy resampler. [Martin Raspaud]

- Fix satpy resampler for satpy syntax. [Martin Raspaud]

- Bugfix in satpy compositor. [Martin Raspaud]

- Add fetch plugin. [Martin Raspaud]

- Fix PyYAML case as dependency in setup.cfg. [Martin Raspaud]

v0.7.0 (2017-04-04)
-------------------

- Update changelog. [Panu Lahtinen]

- Bump version: 0.6.0 → 0.7.0. [Panu Lahtinen]

- Add restart() and is_alive() [Panu Lahtinen]

- Add restart() and is_alive(), remove double setting of logger. [Panu
  Lahtinen]

- Move _prev_lock to class attribute, add is_alive() [Panu Lahtinen]

- Move _prev_lock to class attribute, add self.is_alive() [Panu
  Lahtinen]

- Skip coverage calculation if min_coverage is not defined. [Panu
  Lahtinen]

v0.6.0 (2017-03-28)
-------------------

- Update changelog. [Panu Lahtinen]

- Bump version: 0.5.1 → 0.6.0. [Panu Lahtinen]

- Wrap a long line. [Panu Lahtinen]

- Add locking functionality to enhance.Pansharpener. [Panu Lahtinen]

- Fix import, fix name of area defs in scene info dictionary. [Panu
  Lahtinen]

- Add minimal product config. [Panu Lahtinen]

- Add _template to filenames. [Panu Lahtinen]

- Rename example config. [Panu Lahtinen]

- Set save_settings to empty dict if no settings are given. [Panu
  Lahtinen]

- Add minimal config example. [Panu Lahtinen]

- Add coverage module. [Panu Lahtinen]

- Add plugin to check coverage. [Panu Lahtinen]

  This plugin removes areas from production if the data doesn't cover the
  area well enough.


- Reflow overlong line. [Panu Lahtinen]

- Add raised error message to log. [Panu Lahtinen]

- Import trollflow_sat.utils instead of trollflow.utils. [Panu Lahtinen]

- Fix typo in call to release_locks() [Panu Lahtinen]

- Fix incorrect call to release_locks() [Panu Lahtinen]

- Fix typo in function call. [Panu Lahtinen]

- Fix typo. [Panu Lahtinen]

- Add TypeError to catched errors. [Panu Lahtinen]

- Pass full message, not only message data. [Panu Lahtinen]

- Add missing kwarg. [Panu Lahtinen]

v0.5.1 (2017-03-21)
-------------------

- Update changelog. [Panu Lahtinen]

- Bump version: 0.5.0 → 0.5.1. [Panu Lahtinen]

- Fix missing acquire_lock. [Panu Lahtinen]

v0.5.0 (2017-03-21)
-------------------

- Update changelog. [Panu Lahtinen]

- Bump version: 0.4.0 → 0.5.0. [Panu Lahtinen]

- Add missing parameters. [Panu Lahtinen]

- Add check for valid instruments. [Panu Lahtinen]

- Bring satpy plugins up-to-date with mpop versions. [Panu Lahtinen]

- Remove import of acquire_lock(), instead use utils.acquire_lock()
  [Panu Lahtinen]

- Move monitor messaging after scene creation. [Panu Lahtinen]

- Fix publisher name. [Panu Lahtinen]

- Add monitoring message setting examples. [Panu Lahtinen]

- Use lock release wrapper. [Panu Lahtinen]

- Add wrapper to lock release. [Panu Lahtinen]

- Remove unused import. [Panu Lahtinen]

- Add more tests for utils. [Panu Lahtinen]

- Add helper functions for monitoring messaging. [Panu Lahtinen]

- Add monitoring messages. [Panu Lahtinen]

v0.4.0 (2017-03-14)
-------------------

- Update changelog. [Panu Lahtinen]

- Bump version: 0.3.0 → 0.4.0. [Panu Lahtinen]

- Merge branch 'master' into develop. [Panu Lahtinen]

- Add list of used instruments. [Panu Lahtinen]

- Fix getting filenames from collected datasets. [Panu Lahtinen]

- Fix checking what type of collection is used. [Panu Lahtinen]

- Fix reading filenames from a collection. [Panu Lahtinen]

- Add check for collection id, catch some errors when loading data.
  [Panu Lahtinen]

- Fix formatting of log message. [Panu Lahtinen]

- Fix typo. [Panu Lahtinen]

- Get configuration for single product. [Panu Lahtinen]

- Fix incorrect logic. [Panu Lahtinen]

- Add missing argument. [Panu Lahtinen]

- Add a possibility to limit production based on Sun zenith angle. [Panu
  Lahtinen]

- Fix syntax error. [Panu Lahtinen]

- Catch NoSectionError when trying to create composites. [Panu Lahtinen]

- Release previous lock when skipping data, add logging. [Panu Lahtinen]

- Add log message listing used files. [Panu Lahtinen]

- Check used instruments, give data filenames as arguments to load()
  [Panu Lahtinen]

v0.3.0 (2017-03-07)
-------------------

- Update changelog. [Panu Lahtinen]

- Bump version: 0.2.0 → 0.3.0. [Panu Lahtinen]

- Compose the topic to include {area_id} (if configured) [Panu Lahtinen]

v0.2.0 (2017-02-28)
-------------------

- Update changelog. [Panu Lahtinen]

- Bump version: 0.1.0 → 0.2.0. [Panu Lahtinen]

- Add missing calls to release_lock() [Panu Lahtinen]

- Ensure non-unicode filename (I'm looking at you, gdal) [Panu Lahtinen]

- Fix dictionary key naming "areaname" to "area_id" [Panu Lahtinen]

- Ensure downstream workers have finished before releasing upstream
  locks. [Panu Lahtinen]

- Add use_lock for daemons to config templates. [Panu Lahtinen]

- Add "use_lock" kwarg to daemons, lock only if set to True. [Panu
  Lahtinen]

- Adjust lock handling order, use trollflow.utils for lock
  acquire/release. [Panu Lahtinen]

- Move lock acquire/release to trollflow.utils. [Panu Lahtinen]

- Fix locking, add data reload, add satproj. [Panu Lahtinen]

  - use RLock instead of Lock
  - fix incorrectly understood lock acquire/release
  - reload data for each area group
  - make it possible to save data in satellite projection by
    defining areaname as "satproj"
  - check lock usage as first step in invoke()
  - if using locking, wait 1 sec after releasing local lock


- Add config examples for locking. [Panu Lahtinen]

- Remove unnecessary "content" dictionaries. [Panu Lahtinen]

- Delete incomplete plugin. [Panu Lahtinen]

- Fix locking. [Panu Lahtinen]

- Add locking. [Panu Lahtinen]

- Add queue.task_done() [Panu Lahtinen]

- Remove incomplete components. [Panu Lahtinen]

- PEP8. [Panu Lahtinen]

- PEP8. [Panu Lahtinen]

- PEP8. [Panu Lahtinen]

- PEP8. [Panu Lahtinen]

- Fix package name for coverage. [Panu Lahtinen]

- Update "format" section. [Panu Lahtinen]

- Fix intendation. [Panu Lahtinen]

- Add config option for use_threading. [Panu Lahtinen]

- Fix class names, change items under "config" to dicts. [Panu Lahtinen]

- Adjust log messages, set output queues to None by default. [Panu
  Lahtinen]

- Adjust log messages. [Panu Lahtinen]

- Change default argument of nameservers from [] to None and handle the
  change. [Panu Lahtinen]

- Fix unittest so that they use ordered_load and the new format
  structure. [Panu Lahtinen]

- Return list instead of a set. [Panu Lahtinen]

- Remove hardcoded loading of composite "overview" [Panu Lahtinen]

- Fix writer indexing. [Panu Lahtinen]

- Make it possible to define specific writers for satpy. [Panu Lahtinen]

- Fix function name. [Panu Lahtinen]

- Add handling for dataset messages and placeholder for collections.
  [Panu Lahtinen]

- Add log config example. [Panu Lahtinen]

- Add tests for time name adjustments. [Panu Lahtinen]

- Fix time name adjustment, ignore time tags having 'proc' and 'end' in
  them. [Panu Lahtinen]

- Add plugins using satpy instead of mpop, add example YAML configs.
  [Panu Lahtinen]

- Add logger, figure out time name used in filename pattern and metadata
  and use them to update pattern if necessary. [Panu Lahtinen]

- Change composites from list to dict. [Panu Lahtinen]

v0.1.0 (2016-11-22)
-------------------

- Update changelog. [Panu Lahtinen]

- Bump version: 0.0.1 → 0.1.0. [Panu Lahtinen]

- Fix path to version file. [Panu Lahtinen]

- Adjust install requirements. [Panu Lahtinen]

- Adjust to use listener from posttroll. [Panu Lahtinen]

- Moved to posttroll. [Panu Lahtinen]

- Update TODO. [Panu Lahtinen]

- Add unittests for trollflow_sat.utils.create_fnames() [Panu Lahtinen]

- Clarify naming, fix incorrect dict structure, adjust logging. [Panu
  Lahtinen]

- Ensure absolute path for URI. [Panu Lahtinen]

- Fix import, adapt to YAML config patterns. [Panu Lahtinen]

- Fix import, adapt to YAML config patterns. [Panu Lahtinen]

- Fix import, clarify naming. [Panu Lahtinen]

- Fix syntax, change out_dir to output_dir, add log warning if no output
  directory is given. [Panu Lahtinen]

- Clarify structure, add missing quotes around file patterns. [Panu
  Lahtinen]

- Fix package name. [Panu Lahtinen]

- Rename package. [Panu Lahtinen]

- Set built-in default for output format. [Panu Lahtinen]

- Remove check for empty file pattern, as default is used if all else
  fails, give warning if this happens. [Panu Lahtinen]

- Use common settings if more specific settings are not given. [Panu
  Lahtinen]

- Add .eggs/ to ignored files. [Panu Lahtinen]

- Adjust requirements. [Panu Lahtinen]

- Add unittests. [Panu Lahtinen]

- Example product confgi in YAML. [Panu Lahtinen]

- Add todo-list. [Panu Lahtinen]

- Get area specific resampling search radius if available. [Panu
  Lahtinen]

- Take output directory name from config. [Panu Lahtinen]

- Adjust to YAML product config, simplify what is passed to output
  queue. [Panu Lahtinen]

- Add example configs, adapt to new package name. [Panu Lahtinen]

- Copy plugins from trollduction@feature_trollflow. [Panu Lahtinen]

- Add basic files. [Panu Lahtinen]

- Add placeholder for tests. [Panu Lahtinen]

- Initial commit. [Panu Lahtinen]


