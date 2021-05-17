# Indirect Output

When the behavior of the system under test (SUT) includes actions that cannot be observed through the public API of the SUT but which are seen or experienced by other systems or application components, we call those actions the indirect outputs of the SUT. 

Indirect outputs may be method or function calls to another component, messages sent on a message channel (e.g. MQ or JMS), records inserted into a database or written to a file. 

Verification of the indirect output behaviors of the SUT requires the appropriate observation points on the "back side" of the SUT. 

Mock Objects are often used to implement the observation point by intercepting the indirect outputs of the SUT and comparing them to the expected values.

