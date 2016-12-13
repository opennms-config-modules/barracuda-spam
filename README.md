# barracuda-spam
Barracuda Email Security Gateway

## Enable SNMP trap support

.Copy into OpenNMS configuration folders
[source, bash]
----
cp events/barracuda-spam.events.xml ${OPENNMS_HOME}/etc/events
----

.Add include statement as first entry in ${OPENNMS_HOME}/etc/eventconf.xml
[source, bash]
----
<event-file>events/barracuda-spam.events.xml</event-file>
----
