Snux System 11 Driver Board
===========================

+------------------------------------------------------------------------------+
| Related Config File Sections                                                 |
+==============================================================================+
| :doc:`/config/hardware`                                                      |
+------------------------------------------------------------------------------+
| :doc:`/config/snux`                                                          |
+------------------------------------------------------------------------------+
| :doc:`/config/system11`                                                      |
+------------------------------------------------------------------------------+
| :doc:`/config/switches`                                                      |
+------------------------------------------------------------------------------+
| :doc:`/config/coils`                                                         |
+------------------------------------------------------------------------------+

:doc:`/about/help_us_to_write_it`

This is an example:

.. code-block:: mpf-config

   hardware:
       platform: virtual
       driverboards: wpc
       coils: snux

   system11:
       ac_relay_delay_ms: 75
       ac_relay_driver: c_ac_relay

   snux:
       flipper_enable_driver: c_flipper_enable_driver
       diag_led_driver: c_diag_led_driver
       platform:

   coils:
       c_diag_led_driver:
           number: c24
           default_hold_power: 1.0
       c_flipper_enable_driver:
           number: c23
           default_hold_power: 1.0
       c_ac_relay:
           number: c25
           default_hold_power: 1.0
       c_side_a1:
           number: c11a
       c_side_a2:
           number: c12a
           default_hold_power: 0.5
       c_side_c1:
           number: c11c
       c_side_c2:
           number: c12c
           default_hold_power: 0.5
       c_virtual:
           number:
