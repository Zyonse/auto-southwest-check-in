# Changelog
When upgrading to a new version, make sure to follow the directions under the "Upgrading" header of the corresponding version.
If there is no "Upgrading" header for that version, no post-upgrade actions need to be performed.

## 1.0 (2022-12-10)

### New Features
- Many internal changes were done to improve the codebase, making the execution flow much more practical
(Thanks to [@sdstolworthy](https://github.com/sdstolworthy) for the
[proposed refactors](https://github.com/jdholtz/auto-southwest-check-in/issues/10#issuecomment-1292725481))
- If login credentials are provided, the script will continuously monitor the account for new flights, scheduling
check-ins automatically (Fixes [#10](https://github.com/jdholtz/auto-southwest-check-in/issues/10)).
The interval can be modified with the
[retrieval_interval](https://github.com/jdholtz/auto-southwest-check-in/tree/master#retrieval-interval) config option
- The version of the script can now be retrieved with the `--version` or `-v` flag

### Upgrading
Upgrade the dependencies to the latest versions by running `pip install --upgrade -r requirements.txt`
