# OpenShift Memcached Cartridge

The `memcached` cartridge provides [Memcached](http://www.memcached.org/) on OpenShift, to install  create your app and run:

	app cartridge add http://reflector-apps.sapp.io/reflect?github=mignev/openshift-cartridge-memcached --app [APP]

## Environment Variables

The `memcached` cartridge provides following environment variables:

    OPENSHIFT_MEMCACHED_HOST         The Memcached IP address
    OPENSHIFT_MEMCACHED_PORT         The Memcached port
    OPENSHIFT_MEMCACHED_USERNAME     Username (if auth enabled)
    OPENSHIFT_MEMCACHED_PASSWORD     Password (if auth enabled)

To enable authentication, set user env var ENABLE_SASL=1 and restart your application:

    $ app env set ENABLE_SASL=1 --app [APP]"
    $ app stop --app [APP]"
    $ app start --app [APP]"
