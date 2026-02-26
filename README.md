# SSN Virginia-class Sonar Dashboard - Fixed Version

A sophisticated sonar simulation dashboard inspired by nuclear-powered attack submarines (SSNs).

## Overview

This project simulates a modern submarine sonar system with realistic radar sweeps, contact tracking, torpedo systems, and acoustic analysis. The fixed version addresses critical bugs in the original implementation.

## Repository Information

- **Original Code**: Single HTML file with embedded CSS and JavaScript
- **Fixed Version**: All critical bugs resolved (v2.0)
- **Repository**: https://github.com/theTotesmagoats/sonar-dashboard-debug

## Features

### Navigation & Operations Panel
- Real-time depth control with safety filters
- Vessel statistics monitoring (depth, speed, heading, reactor status)
- Torpedo tube management with arming/safe controls
- Fire control system with reload timers

### Sonar Display Array (Center Panel)
- 360-degree radar sweep animation
- Contact detection and tracking
- Ghost echo filtering for realistic radar behavior
- Coordinate readout with bearing and range
- FPS counter and contact count display

### Acoustic Analysis Panel
- LED indicators for system status (SONAR, GHOST ECHOES, TRAILS)
- Range filtering controls
- Target coordinate input for fire control
- Contact log with timestamped events
- Acoustic environment data (noise floor, temperature, salinity)

## Bug Fixes Applied

### Critical Issues Resolved:
1. **Color replacement bug** - Fixed hex color alpha handling
2. **Torpedo lifetime** - Torpedoes now properly expire after 600 frames (10 seconds)
3. **Explosion collision detection** - Explosions now destroy contacts within their radius
4. **Range filtering** - Added maximum range filter to prevent clutter
5. **FPS calculation** - Fixed potential division by zero issues
6. **DOM element safety** - Added null checks for all DOM access

See [BUGFIXES.md](./BUGFIXES.md) for detailed technical information.

## How to Use

### Basic Operation:
1. Open `index.html` in a modern web browser
2. Monitor the sonar display for contacts (green = friendly, red = hostile)
3. Adjust depth and range filters using sliders
4. Arm torpedoes using the tube control buttons
5. Set target coordinates and fire when ready

### Keyboard Shortcuts:
- **F** - Fire torpedo
- **S** - Toggle sonar active/passive
- **G** - Toggle ghost echoes
- **T** - Toggle contact trails
- **1-8** - Select specific torpedo tube

## Technical Details

### System Requirements:
- Modern web browser with HTML5 Canvas support
- JavaScript ES6+ capable
- Audio support for sonar effects (Chrome, Firefox, Edge)

### Architecture:
- Single-page application with no external dependencies
- Canvas-based rendering with custom animation loop
- Event-driven UI updates with real-time data binding

## Known Limitations

1. **Performance**: Large numbers of contacts (>50) may impact frame rate
2. **Browser Compatibility**: Some advanced audio features may not work in all browsers
3. **Realism**: This is a simulation - actual submarine operations are far more complex

## Future Enhancements

- [ ] Multiplayer support for coordinated operations
- [ ] More realistic sonar physics (Doppler shift, water temperature layers)
- [ ] Advanced torpedo guidance systems
- [ ] Enemy AI improvements
- [ ] Save/load mission state

## License

This project is provided as-is for educational and entertainment purposes.

## Credits

- Original concept and design: Unknown
- Bug fixes and improvements: AI-assisted code review

## Support

For bug reports or feature requests, please create an issue in the GitHub repository.

---

**Version**: 2.0 (Fixed)  
**Last Updated**: February 26, 2026  
**Repository**: https://github.com/theTotesmagoats/sonar-dashboard-debug
