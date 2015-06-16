# Ansible Monit Role for Debian Wheezy

This role configures monit to monitor: haproxy, nginx and unicorn.

### Optional Configuration

It is assumed your application is located within /home/*username*/*appname*/
This can be configured with the following variable:

```yaml
  roles:
    - { role: tholder.monit, app_root: '/var/www/{{ app_name }}'}
```

### Limitations

This role only works with Debian Wheezy for time being.

Nginx must be running on port 8080 as the backend.

Notifications are sent to "sysops@simpleweb.co.uk"

### Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
