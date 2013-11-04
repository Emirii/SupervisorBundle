Supervisor Control Bundle
=========================

This bundle for quick configure and usage separate instance of [supervisord](http://supervisord.org/).

All Symfony2 commands run supervisor from kernel.root_dir path.
If use config created by supervisor:init use [local configure file](http://supervisord.org/configuration.html).

Bundle has commands:

  * supervisor:init
    - create supervisord.conf file and supervisor folder in app folder
  * supervisor:run
    - check instance of supervisord and run it if need
    - add this command to cron - simple quick watchdog for supervisord
  * supervisor:control
    - run any supervisorCtl command
  * supervisor:gen
    - generate simple programm section for symfony2 console command

Service supervisor may run daemon, execute any command, and generate files for supervisord.