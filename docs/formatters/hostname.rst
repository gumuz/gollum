Hostname
========

Hostname is a formatter that prefixes a message with the hostname.


Parameters
----------

**HostnameDataFormatter**
  HostnameDataFormatter defines the formatter for the data transferred as message.
  By default this is set to "format.Envelope".

**HostnameSeparator**
  HostnameSeparator sets the separator character placed after the hostname.
  This is set to " " by default.

Example
-------

.. code-block:: yaml

	- "stream.Broadcast":
	    Formatter: "format.Hostname"
	    HostnameFormatter: "format.Envelope"
	    HostnameSeparator: " "
