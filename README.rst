Clue Coffee Scale
============

.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code Style: Black

The Clue Coffee Scale is designed to measure the weight of the ground beans or the extraction output to
achieve repeatable results for your preferred brew. To measure the contents of a container, the
scale can be zeroed with a push of the Clue's A button to subtract the container's tare weight.

The scale uses a load cell sensor that consists of a very sensitive resistance array (a strain gauge)
attached to a metal bending beam. The specialized NAU7802 Analog-to-Digital Converter (ADC) breakout
board connects to the load cell and measures the slight changes in the array's differential voltage,
calculating the weight of the mass placed on the load cell.

The Clue interfaces with the NAU7802 ADC board and automatically updates a colorful graphics display
showing the results in both ounces and grams.


.. image:: https://github.com/CedarGroveStudios/Clue_Coffee_Scale/blob/master/media/clue_scale_01.jpg
   :width: 400
   :alt: Clue Coffee Scale in Action


Dependencies
=============
This project depends on:

* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_

Please ensure all dependencies are available on the CircuitPython filesystem.
This is easily achieved by downloading
`the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
or individual libraries can be installed using
`circup <https://github.com/adafruit/circup>`_.




