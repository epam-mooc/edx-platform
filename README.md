This is the fork from [general repository](https://github.com/edx/edx-platform). All information about platform and readme you can find there. Here you can see only short guidence how to update your platform to this version.

How to update your platform to this version
-------------------------------------------

1. First of all, add or check these lines at your '/edx/app/edx_ansible/server-vars.yml':
   * edx_platform_repo: https://github.com/epam-mooc/edx-platform.git
   * edx_platform_version: master
2. Only if you want clear installing (for example, if update process is fail, to start from the scratch), **remove entire folder** '/edx/app/edxapp/edx-platform'. Yes, remove all.
3. Execute update command:
   * sudo /edx/bin/update edx-platform master
4. If in the end of execution you see 0 errors, it execute normally, otherwise I'm sorry - in this case you can find log files here: '/edx/var/log' and try to fix it.

License
-------

The code in this repository is licensed under version 3 of the AGPL unless
otherwise noted. Please see the
[`LICENSE`](https://github.com/epam-mooc/edx-platform/blob/master/LICENSE) file
for details.
