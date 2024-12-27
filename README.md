# Zigbee Latency Analysis

A comprehensive tool for analyzing and visualizing latency patterns in Zigbee networks, specifically designed for smart home setups using Zigbee2MQTT.

## Features

- Real-time monitoring of Zigbee2MQTT logs
- Detailed latency analysis for motion-triggered events
- Network topology visualization
- Time-based pattern analysis
- Performance anomaly detection
- Comprehensive statistical reporting

## Installation

1. Clone the repository:
```bash
git clone https://github.com/michaelnoergaard/zigbee-latency-analysis.git
cd zigbee-latency-analysis
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Install the package in development mode:
```bash
pip install -e .
```

## Usage

Run the analysis tool with default settings:
```bash
zigbee-analysis
```

Specify custom report interval and output directory:
```bash
zigbee-analysis --report-interval 1800 --output-dir /path/to/output
```

### Configuration

The tool's configuration can be adjusted in `src/config.py`, including:
- Log directory path
- Latency thresholds
- Time window definitions
- Device type mappings

## Analysis Features

### Network Topology
- Visualizes the Zigbee mesh network structure
- Shows connection quality between devices
- Identifies potential network bottlenecks

### Latency Analysis
- Separates initial triggers from timer resets
- Provides statistical analysis by time of day
- Tracks performance trends over time
- Identifies anomalies in device behavior

### Time-based Patterns
Analyzes performance across different time windows:
- Morning (6:00-12:00)
- Afternoon (12:00-18:00)
- Evening (18:00-22:00)
- Night (22:00-6:00)

### Performance Reports
Generates comprehensive reports including:
- Device-specific statistics
- Network-wide metrics
- Anomaly detection
- Time-based patterns

## Output

The tool generates several types of output:
- Text-based performance reports
- Network topology visualizations
- Latency distribution graphs
- Time pattern analysis charts

All outputs are saved in the specified output directory with timestamps.

## Requirements

- Python 3.7+
- Zigbee2MQTT setup with accessible log files
- Dependencies listed in `requirements.txt`

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.