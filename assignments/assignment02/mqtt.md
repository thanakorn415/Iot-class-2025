# Exploring MQTT QoS Levels

Experiment with QoS 0, 1, and 2.
Observe how message delivery changes based on QoS settings.

## Publisher_qos.py output

```
d:\term4.1\IOT\Iot-class-2025\Iot-class-2025-gateway\app\publisher_qos.py:20: DeprecationWarning: Callback API version 1 is deprecated, update to latest version
  client = mqtt.Client()
[16:04:44] DEBUG | Sending CONNECT (u0, p0, wr0, wq0, wf0, c1, k60) client_id=b''
Enter message to publish: [16:04:44] DEBUG | Received CONNACK (0, 0)
egadgfdjhkkkkkgfhhjhgfdjhdtythgfshdgthsir
Enter QoS level (0, 1, 2): 2
[16:04:53] DEBUG | Sending PUBLISH (d0, q2, r0, m1), 'b'test/qos/6510301023'', ... (41 bytes)
[16:04:53] PUBLISH REQUESTED | QoS=2 | Message='egadgfdjhkkkkkgfhhjhgfdjhdtythgfshdgthsir' | msgid=1
Enter message to publish: [16:04:53] DEBUG | Received PUBREC (Mid: 1)
[16:04:53] DEBUG | Sending PUBREL (Mid: 1)
[16:04:53] DEBUG | Received PUBCOMP (Mid: 1)
[16:04:53] PUBLISHED | msgid=1
[16:05:44] DEBUG | Sending PINGREQ
[16:05:44] DEBUG | Received PINGRESP
[16:06:45] DEBUG | Sending PINGREQ
[16:06:45] DEBUG | Received PINGRESP
[16:07:45] DEBUG | Sending PINGREQ
[16:07:45] DEBUG | Received PINGRESP
```

## Subscriber_qos.py Output

```
d:\term4.1\IOT\Iot-class-2025\Iot-class-2025-gateway\app\subscriber_qos.py:25: DeprecationWarning: Callback API version 1 is deprecated, update to latest version
  client = mqtt.Client()
[16:04:23] DEBUG | Sending CONNECT (u0, p0, wr0, wq0, wf0, c1, k60) client_id=b''
[16:04:23] DEBUG | Received CONNACK (0, 0)
[16:04:23] Connected with result code 0
[16:04:23] DEBUG | Sending SUBSCRIBE (d0, m1) [(b'test/qos/6510301023', 2)]
[16:04:23] DEBUG | Received SUBACK
[16:04:53] DEBUG | Received PUBLISH (d0, q2, r0, m1), 'test/qos/6510301023', ...  (41 bytes)
[16:04:53] DEBUG | Sending PUBREC (Mid: 1)
[16:04:53] DEBUG | Received PUBREL (Mid: 1)
[16:04:53] RECEIVED | QoS=2 | Topic=test/qos/6510301023 | Message=egadgfdjhkkkkkgfhhjhgfdjhdtythgfshdgthsir | msgid=1
[16:04:53] DEBUG | Sending PUBCOMP (Mid: 1)
[16:05:24] DEBUG | Sending PINGREQ
[16:05:24] DEBUG | Received PINGRESP
[16:06:25] DEBUG | Sending PINGREQ
[16:06:25] DEBUG | Received PINGRESP
[16:07:25] DEBUG | Sending PINGREQ
[16:07:25] DEBUG | Received PINGRESP
[16:08:26] DEBUG | Sending PINGREQ
[16:08:26] DEBUG | Received PINGRESP
```