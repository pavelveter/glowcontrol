# **GlowControl**

### _A Powerful Bash Utility for Your Yeelight Smart Bulbs_

![GlowControl](gc_logo.png)

Welcome to **GlowControl** — your ultimate Bash utility to seamlessly control Yeelight smart bulbs over Wi-Fi. With a simple yet powerful command-line interface, GlowControl empowers you to light up your world exactly the way you want it. Whether you're looking to create the perfect ambiance for movie night, set the mood for a party, or just adjust the lighting for daily activities, GlowControl has you covered.

## **Features**

- **Easy Control:** Manage single or multiple Yeelight bulbs with just a few keystrokes.
- **Customizable Lighting:** Set the perfect color and brightness to match any occasion.
- **Exciting Modes:** Engage disco mode for a party atmosphere or sunrise mode to start your day right.
- **Notifications:** Use your lights as a notification system with color-coded alerts.

## **Getting Started**

### **Usage**

```bash
light.sh <ip|@alias> <command>
```

**`<ip>`**: A single IP, multiple IPs, or a range of IP addresses to control specific bulbs.

**`<@alias>`**: An alias for a bulb or a group of bulbs (e.g., `@room`, `@kitchen`, `@all`).

**`<command>`**: The action you want to perform, such as turning the light on, setting a color, adjusting brightness, and more.

### **Commands**

- **`on`**: Turn on the light.
- **`off`**: Turn off the light.
- **`[color] <color>`**: Set the light to a specific color. The `color` key is optional.
- **`[t] <number>`**: Set the white light temperature (1700K to 6500K). The `t` key is optional.
- **`disco`**: Activate disco mode.
- **`sunrise`**: Activate sunrise mode.
- **`notify-<color>`**: Send a notification using a specified color.
- **`dim`**: Dim the light to 5% brightness.
- **`undim`**: Reset the light to 100% brightness.
- **`[brightness] <level>`**: Set the brightness level (1-100). The `brightness` key is optional.

### **Colors Available**

Choose from a wide range of colors to match your mood:

- Amber, Blue, Cyan, Dandelion, Emerald, Flamingo, Green, Honeydew, Indigo, Jade, Khaki, Lavender, Magenta, Navy, Olive, Purple, Quartz, Red, Silver, Teal, Ultramarine, Violet, White, Xanadu, Yellow, Zinnwaldite.

### **Aliases Available**

Control groups of bulbs with ease:

- `@room`, `@kitchen`, `@bathroom`, `@monitor`, `@stand`, `@tv`, `@all`.

### **Examples**

1. **Turn on a single bulb:**
   ```bash
   light.sh 192.168.1.1 on
   ```
2. **Set three bulbs to red:**
   ```bash
   light.sh 192.168.1.1-2 192.168.1.4 color red
   ```
3. **Adjust brightness of two bulbs:**
   ```bash
   light.sh 192.168.1.1 192.168.1.3 50
   ```
4. **Set white temperature to 4100K:**
   ```bash
   light.sh 192.168.1.2 t 4100
   ```
5. **Notify via room bulbs with blue color:**
   ```bash
   light.sh @room notify-blue
   ```

## **Installation**

Clone the repository and give the script executable permissions:

```bash
git clone https://github.com/yourusername/glowcontrol.git
cd glowcontrol
chmod +x light.sh
```

## **Contributing**

We welcome contributions! Feel free to submit issues, fork the repo, and send pull requests. Let's make GlowControl even better together.

## **License**

GlowControl is licensed under the MIT License.

---

Illuminate your life with the power of Bash and Yeelight — experience GlowControl today!

p.s. Based on github.com/shyamvalsan/YeelightController
