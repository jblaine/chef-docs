.. The contents of this file may be included in multiple topics (using the includes directive).
.. The contents of this file should be modified in a way that preserves its ability to appear in multiple topics.

.. To test if global forwarding is enabled for an IPv4 address:

.. code-block:: ruby

   describe kernel_parameter('net.ipv4.conf.all.forwarding') do
     its(:value) { should eq 1 }
   end
