Zend XML-RPC 2.2.6
==================

A fork of [Zend Framework's XML-RPC Component for ZF2](https://github.com/zendframework/Component_ZendXmlRpc).

Since Zend Framework 2.3.0 requires PHP 5.3.23, installing the Zend XML-RPC component through Composer on older PHP setups resulted in a broken install, with missing dependencies (`XmlSecurity` in the non-existent `Zend\Xml\Security` namespaced class.

This fork attempts to create a working composer installation for PHP 5.3.6 and PHP 5.3.10, by correcting the broken dependencies.


To use this package, add the following to composer.json:

    "repositories": [
        {
            "type": "vcs",
            "url": "http://github.com/jotlabs/ZendXmlRpc"
        },
        {
            "type": "composer",
            "url": "https://packages.zendframework.com/"
        }
    ],

And then require the XML-RPC library:

    "require": {
        ...
        "zendframework/zend-xmlrpc": "2.2.6.*"
    },

Then `composer install` should pull in this repo's version.


If you are on PHP 5.3.23 or above, you should be using Zend's version instead of this.


----

XML-RPC Component from ZF2
==========================

This is the XML-RPC component for ZF2.

- File issues at https://github.com/zendframework/zf2/issues
- Create pull requests against https://github.com/zendframework/zf2
- Documentation is at http://framework.zend.com/docs

LICENSE
-------

The files in this archive are released under the [Zend Framework
license](http://framework.zend.com/license), which is a 3-clause BSD license.

