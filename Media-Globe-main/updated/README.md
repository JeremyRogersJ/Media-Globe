# Media Globe - TV Integration Update

## 🎯 What's New

This updated version integrates **real IPTV news channels** from the iptv-org database, adding live TV streaming alongside the existing radio functionality.

## ✨ Key Features

### **Real IPTV Data**
- Fetches live data from `https://iptv-org.github.io/api/`
- Uses actual news channels with working stream URLs
- Displays real channel logos and metadata

### **Geographic Organization**
- TV channels grouped by country/region/capital cities
- 📺 Red markers for TV news stations
- 📻 Green markers for radio stations (existing)

### **Streaming Capabilities**
- Full HLS/m3u8 video streaming
- Audio fallback for unsupported formats
- Integrated media controls
- Volume control and playback management

### **Smart Filtering**
- Shows only news category channels
- Filters out channels without working streams
- Organized by geographic location

## 🌍 Geographic Coverage

The system maps TV news channels to their broadcast regions using capital city coordinates for:
- **US**: Washington DC
- **UK**: London  
- **FR**: Paris
- **DE**: Berlin
- **And 100+ more countries**

## 🎮 How to Use

1. **Open** `media-globe-with-tv.html` in your browser
2. **Enable both platforms** in the control panel (Radio + TV)
3. **Navigate the globe** to find red TV markers
4. **Click markers** to see available news channels
5. **Click channels** to start streaming

## 🔧 Technical Implementation

### **API Endpoints Used:**
- `channels.json` - Channel metadata
- `streams.json` - Streaming URLs  
- `logos.json` - Channel logos

### **Data Processing:**
1. Fetches all IPTV channels
2. Filters for news category only
3. Groups by country/city coordinates
4. Maps to capital city locations
5. Creates clickable markers

### **Streaming:**
- Primary: HTML5 video element
- Fallback: HTML5 audio element
- Supports most HLS/m3u8 formats

## 🚀 Quick Start

```bash
# Just open the file in your browser:
media-globe-with-tv.html
```

## 📊 Expected Data Volume

- **~500-800 news channels** worldwide
- **~150 geographic locations**  
- **Real-time streaming** from live sources
- **Channel logos** when available

## 🎨 Visual Design

- **TV Stations**: Red 📺 markers, larger based on channel count
- **Radio Stations**: Green 📻 markers, individual dots
- **Combined Interface**: Unified media overlay
- **Logo Support**: Real channel branding

The integration maintains the existing Radio Garden aesthetic while adding professional TV news streaming capabilities.