# Executive Dashboard

A powerful, open-source executive dashboard for tracking capital burn rate, roadmap initiatives, and operational expenses. Built as a single HTML file with no dependencies, making it perfect for quick deployment and customization.

![Dashboard Preview](https://via.placeholder.com/800x400?text=Dashboard+Preview)

## 🚀 Features

### 📊 Capital Burn Rate Tracking
- Real-time visualization of remaining capital over time
- Configurable starting capital and burn rate
- Visual warnings when capital is depleted

### 🗓️ Roadmap Timeline (Gantt-style)
- Interactive initiative planning with horizontal timeline bars
- Resource multiplier effects on timeline duration  
- Effort estimation with design, development, and product hours
- Dynamic date range adjustment based on initiative timelines

### 💰 Expense Management
- Dynamic expense tracking with monthly and weekly calculations
- Enable/disable expenses for scenario planning
- Categorized expense types with notes

### 💾 Data Persistence
- Automatic save to browser localStorage
- JSON export/import for backup and sharing
- Default configuration file for baseline setup
- No database required - runs entirely in browser

## 🏃‍♂️ Quick Start

### Option 1: Download and Run
1. Download or clone this repository
2. Open `index.html` in any modern web browser
3. Start planning your initiatives and tracking expenses!

### Option 2: GitHub Pages (Coming Soon)
Visit the live demo at: `https://yourusername.github.io/exec-dashboard`

## 📖 Usage Guide

### Initial Setup
1. **Configure Starting Capital**: Set your initial funding amount
2. **Set Start Date**: Choose when your tracking period begins
3. **Add Expenses**: Input monthly operational costs
4. **Create Initiatives**: Define roadmap items with effort estimates

### Managing Expenses
- Click "Add Expense" to create new operational costs
- Use checkboxes to enable/disable expenses for scenario planning
- Monthly costs are automatically converted to weekly rates

### Planning Initiatives
- **Name & Description**: Identify your roadmap items
- **Effort Estimation**: Set weeks of work plus specific role hours
- **Start Date**: When the initiative begins
- **Resource Multiplier**: Adjust for team scaling (0.5x = half speed, 2x = double speed)

### Data Management
- **Auto-save**: Changes automatically save to browser storage
- **Export**: Download current configuration as JSON backup
- **Import**: Load previously exported configurations
- **Reset**: Load default configuration anytime

## 🛠️ Technical Details

### Architecture
- **Single File Application**: Everything in one HTML file
- **No Dependencies**: Uses only browser-native APIs
- **Chart.js Integration**: For beautiful data visualization
- **Responsive Design**: Works on desktop and mobile

### Browser Compatibility
- Chrome/Edge 80+
- Firefox 75+
- Safari 13+
- Mobile browsers supported

### Storage
- **localStorage**: Automatic persistence in browser
- **JSON Files**: Portable backup and sharing format
- **No Server Required**: Runs entirely client-side

## 🔧 Customization

### Modifying Default Data
Edit `default-dashboard-config.json` to change the baseline configuration:

```json
{
  "version": "1.0",
  "settings": {
    "startingCapital": 1000000,
    "startDate": "2024-01-01"
  },
  "expenses": [...],
  "initiatives": [...]
}
```

### Styling
The dashboard uses inline CSS. Search for the `<style>` section in `index.html` to customize:
- Colors and themes
- Layout and spacing  
- Chart appearance
- Button styles

### Adding Features
The modular JavaScript architecture makes it easy to extend:
- `expenses` array: Operational cost data
- `initiatives` array: Roadmap initiative data
- Chart.js configuration: Visualization settings
- Export/import functions: Data management

## 📊 Data Format

### Expense Object
```json
{
  "enabled": true,
  "name": "Engineering Team",
  "monthly": 80000,
  "notes": "4 engineers @ $20k/mo"
}
```

### Initiative Object
```json
{
  "enabled": true,
  "name": "API Integration", 
  "description": "Third-party integrations",
  "weeks": 6,
  "designHours": 40,
  "devHours": 240,
  "productHours": 30,
  "startDate": "2024-02-01",
  "multiplier": 1
}
```

## 🤝 Contributing

We welcome contributions! Here's how to get started:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Development Setup
No build process required! Simply:
1. Clone the repo
2. Open `index.html` in your browser
3. Make changes and refresh to test

### Areas for Contribution
- 🎨 **UI/UX Improvements**: Better design and user experience
- 📊 **Chart Enhancements**: Additional visualization options
- 📱 **Mobile Optimization**: Improved mobile experience
- 🔧 **New Features**: Scenario planning, team management, etc.
- 📖 **Documentation**: Tutorials, examples, and guides
- 🧪 **Testing**: Automated testing framework
- 🌍 **Internationalization**: Multi-language support

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Chart.js** - Beautiful chart library
- **CiteMed Team** - Original development and open source initiative
- **Contributors** - Everyone who helps improve this tool

## 📞 Support & Community

- 🐛 **Issues**: [GitHub Issues](https://github.com/yourusername/exec-dashboard/issues)
- 💬 **Discussions**: [GitHub Discussions](https://github.com/yourusername/exec-dashboard/discussions)
- 📧 **Email**: your-email@domain.com

## 🗺️ Roadmap

### v1.1 (Coming Soon)
- [ ] Multiple scenario comparison
- [ ] Team resource planning
- [ ] Advanced export formats (PDF, Excel)
- [ ] Mobile app version

### v1.2 (Future)
- [ ] Collaborative editing
- [ ] Integration APIs
- [ ] Advanced analytics
- [ ] Custom chart types

---

**Made with ❤️ by the CiteMed team**

*Empowering executives with simple, powerful planning tools.*