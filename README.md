# 🌍 Countries, States & Cities Data

<div align="center">

![GitHub stars](https://img.shields.io/github/stars/hussainu6/Countries-States-Cities-Data?style=social)
![GitHub forks](https://img.shields.io/github/forks/hussainu6/Countries-States-Cities-Data?style=social)
![GitHub issues](https://img.shields.io/github/issues/hussainu6/Countries-States-Cities-Data)
![GitHub license](https://img.shields.io/github/license/hussainu6/Countries-States-Cities-Data)

**Complete dataset of countries, states, and cities** - Ready to use for your projects!

[📥 Download CSV Files](#-quick-download) • [🚀 Quick Start](#-quick-start) • [📊 Dataset Info](#-dataset-overview)

</div>

---

## 🎯 Why This Repository?

- ✅ **Up-to-date data** from the reliable `country-state-city` npm package
- ✅ **Ready-to-use CSV format** - No parsing required
- ✅ **Comprehensive coverage** - 250 countries, 4,963 states, 148,038 cities
- ✅ **Developer-friendly** - Easy integration with any programming language
- ✅ **Free forever** - No API keys or subscriptions needed

---

## 📊 Dataset Overview

| Data Type | Count | File Size | Last Updated |
|-----------|-------|-----------|--------------|
| 🌍 Countries | 250 | ~13 KB | Latest |
| 🗺️ States | 4,963 | ~142 KB | Latest |
| 🏙️ Cities | 148,038 | ~4.5 MB | Latest |

---

## 📁 Files Structure

```
📦 Countries-States-Cities-Data/
├── 📄 README.md              # Complete documentation and usage guide
├── 🌍 countries.csv          # 250 countries with complete info
├── 🗺️ states.csv             # 4,963 states with country mapping
└── 🏙️ cities.csv             # 148,038 cities with state & country mapping
```

---

## 📋 Data Fields

### 🌍 Countries (`countries.csv`)
| Field | Description | Example |
|-------|-------------|---------|
| `name` | Country name | "United States" |
| `iso2` | ISO 3166-1 alpha-2 code | "US" |
| `iso3` | ISO 3166-1 alpha-3 code | "USA" |
| `numericCode` | ISO numeric code | "840" |
| `phonecode` | International dialing code | "+1" |
| `capital` | Capital city | "Washington D.C." |
| `currency` | Currency code | "USD" |
| `currencyName` | Currency name | "United States dollar" |
| `currencySymbol` | Currency symbol | "$" |
| `native` | Native country name | "United States" |
| `emoji` | Country flag emoji | "🇺🇸" |
| `emojiU` | Unicode representation | "U+1F1FA U+1F1F8" |

### 🗺️ States (`states.csv`)
| Field | Description | Example |
|-------|-------------|---------|
| `name` | State/province name | "California" |
| `iso2` | State ISO code | "CA" |
| `countryCode` | Country ISO2 code | "US" |
| `countryName` | Country name | "United States" |

### 🏙️ Cities (`cities.csv`)
| Field | Description | Example |
|-------|-------------|---------|
| `name` | City name | "Los Angeles" |
| `countryCode` | Country ISO2 code | "US" |
| `countryName` | Country name | "United States" |
| `stateCode` | State ISO code | "CA" |
| `stateName` | State name | "California" |

---

## � Quick Download

### Direct CSV Downloads
- 🌍 [Download countries.csv](./countries.csv) (13 KB)
- 🗺️ [Download states.csv](./states.csv) (142 KB)  
- 🏙️ [Download cities.csv](./cities.csv) (4.5 MB)

### Download All Files
```bash
# Clone the entire repository
git clone https://github.com/hussainu6/Countries-States-Cities-Data.git
```

---

## 🚀 Quick Start

### 🟢 JavaScript/Node.js
```javascript
// Using fetch to load CSV data
async function loadCountries() {
    const response = await fetch('./countries.csv');
    const csvData = await response.text();
    // Parse CSV data...
    console.log(csvData);
}

// Or use with node-fetch
const fs = require('fs');
const csvData = fs.readFileSync('./countries.csv', 'utf8');
```

### 🐍 Python
```python
import pandas as pd

# Load data into pandas DataFrame
countries = pd.read_csv('countries.csv')
states = pd.read_csv('states.csv')
cities = pd.read_csv('cities.csv')

# Example: Get all cities in a specific country
us_cities = cities[cities['countryCode'] == 'US']
print(f"Found {len(us_cities)} cities in USA")
```

### 📊 Excel/Google Sheets
1. Open Excel/Google Sheets
2. Go to **Data** → **From Text/CSV**
3. Select the CSV file
4. Import and start analyzing!

### 🌐 Web Application
```html
<!-- Direct link to CSV files -->
<a href="https://raw.githubusercontent.com/hussainu6/Countries-States-Cities-Data/main/countries.csv" download>
    Download Countries CSV
</a>
```

---

## 💡 Use Cases

- 🌐 **Web Applications** - Country/state/city dropdowns
- 📱 **Mobile Apps** - Location-based features
- 📊 **Data Analysis** - Geographic data studies
- 🗺️ **Mapping Projects** - Location markers and boundaries
- 🏢 **Business Intelligence** - Market analysis by region
- 🎯 **Form Validation** - Address verification
- 📚 **Educational Projects** - Geography learning tools

---

## 🔄 Data Updates

This data is generated using the `country-state-city` npm package. To update the data:

1. **Install dependencies**:
   ```bash
   npm install
   ```

2. **Run the export script**:
   ```bash
   node export-data.js
   ```

3. **Commit changes**:
   ```bash
   git add .
   git commit -m "Update dataset"
   git push
   ```

---


---

## 🤝 Contributing

We welcome contributions! Here's how you can help:

- 🐛 **Report Issues**: Found incorrect data? [Open an issue](https://github.com/hussainu6/Countries-States-Cities-Data/issues)
- 💡 **Feature Requests**: Have ideas? [Start a discussion](https://github.com/hussainu6/Countries-States-Cities-Data/discussions)
- 🔧 **Pull Requests**: Want to improve? [Submit a PR](https://github.com/hussainu6/Countries-States-Cities-Data/pulls)

### Contribution Guidelines
1. Fork this repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This dataset is maintained for public use. Please check the original [country-state-city package](https://www.npmjs.com/package/country-state-city) for specific licensing terms.

---

## ⭐ Show Support

If this dataset helps your project, please consider:

- 🌟 **Giving a star** to this repository
- 🔄 **Sharing** with other developers
- 📝 **Leaving feedback** or suggestions
- 💝 **Sponsoring** if you find it valuable for commercial use

---

<div align="center">

**Made with ❤️ for the developer community**

[⬆️ Back to Top](#-countries-states--cities-data)

</div>
