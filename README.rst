
python-jambel
=============

.. image:: https://github.com/jambit/python-jambel/actions/workflows/check.yml/badge.svg
    :target: https://github.com/jambit/python-jambel/actions/workflows/check.yml

Interface to jambit's project traffic lights.

A simple example::

    import jambel
    light = jambel.Jambel('ampel3.dev.jambit.com')
    light.green.on()
    light.yellow.blink()
    light.red.flash()

It is also possible to query the jambel's status::

    status = light.status()
    if stats[jambel.GREEN] == jambel.BLINK:
        print('green light is blinking!')

Interested in the hardware? Contact us at fast-feedback-lights@jambit.com
