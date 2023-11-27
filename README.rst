Introduction
============


.. image:: https://github.com/CedarGroveStudios/Clue_Scale/workflows/Build%20CI/badge.svg
    :target: https://github.com/CedarGroveStudios/Cedargrove_CircuitPython_RangeSlicer/actions
    :alt: Build Status


.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code Style: Black

The Clue Coffee Scale can accurately measure the weight of the ground beans or the extraction output,
getting closer to an exact and repeatable approach for creating your preferred brew. To measure the contents
of a container, the scale can be zeroed with a push of a button to subtract the container's tare weight.
The scale uses a load cell sensor device that consists of a very sensitive resistance array (a strain gauge)
attached to a metal bending beam. When connected to an exciter voltage, the resistance array provides a
differential voltage output signal proportional to the torque of the mass placed on the load cell. The signal
voltage is very low so a sensitive amplifier and high-resolution analog to digital converter (ADC) are used to
provide a microcontroller-compatible measurement.
T

.. image:: https://github.com/CedarGroveStudios/Clue_Scale/blob/master/media/range_slicer_models.png
   :alt: Clue Coffee Scale


Dependencies
=============
This driver depends on:

* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_

Please ensure all dependencies are available on the CircuitPython filesystem.
This is easily achieved by downloading
`the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
or individual libraries can be installed using
`circup <https://github.com/adafruit/circup>`_.


Installing to a Connected CircuitPython Device with Circup
==========================================================

Make sure that you have ``circup`` installed in your Python environment.
Install it with the following command if necessary:

.. code-block:: shell

    pip3 install circup

With ``circup`` installed and your CircuitPython device connected use the
following command to install:

.. code-block:: shell

    circup install cedargrove_rangeslicer

Or the following command to update an existing version:

.. code-block:: shell

    circup update


