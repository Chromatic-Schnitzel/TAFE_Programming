Mongos = Primary Router, it works out which shard needs to be communicated with
The config server tracks data locations to tell the router where things are
Shards hold the data, the primary in a shard communicates changes made to it every second or so
Large Range Wide Variation = Good
Large Range Narrow Variation = Bad

Shard Key Options:
	Humidity (%)
	Temperature (°C)
	Vapor Pressure (kPa)
	Wind Direction (°)
