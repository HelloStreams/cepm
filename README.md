CEPM
====

Complex Event Processing Module

This is the heart of Hello Streams solution. Built over STORM, this module does the realtime stream processing in a distribute manner.

- Stream Config : Reads the stream configuration from the CouchDB database and sets that into the STORM topology configuration.
- Spouts : Read the tuples from the Message Queue
- Filter Bolt : Apply various filters as per the stream configuration
- GroupBy Bolt : Does the temporal and spatial aggregations as per the stream configuration
- Join Bolt : Joins a stream with static data or with another stream
- Sink : Emit the topology output as per the sinks defined in stream config
