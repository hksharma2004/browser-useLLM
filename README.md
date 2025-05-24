# Browser-UseLLM 📱🤖

Ever spent hours comparing phone specs across different websites? We've all been there! Browser-UseLLM is your AI-powered research assistant that automatically compares any two phones for you. Just tell it which phones you're considering, and it'll browse the web, gather all the specs, and give you a clean comparison report.

## What It Does

Think of it as having a tech-savvy friend who never gets tired of researching phones. The system uses AI agents to:

- 🔍 **Smart Web Browsing**: Automatically visits tech websites like GSMArena, PhoneArena, and TechRadar
- 📊 **Real-time Data Collection**: Scrapes current prices, specs, and reviews
- 🧠 **Intelligent Analysis**: Uses Gemini Flash and OpenAI to understand and compare features
- 📝 **Clean Reports**: Generates easy-to-read markdown comparison reports
- 📈 **Professional Logging**: Tracks everything with MAXIM AI for reliability

## 🏗️ Agentic Architecture

Our system works like a team of specialized AI agents, each with their own job:

```
┌─────────────────────────────────────────────────────────────┐
│                    BROWSER-USELLM SYSTEM                    │
├─────────────────────────────────────────────────────────────┤
│  📱 User Input: "Compare iPhone 15 Pro vs Galaxy S24"       │
└─────────────────┬───────────────────────────────────────────┘
                  │
┌─────────────────▼───────────────────────────────────────────┐
│              🎯 ORCHESTRATOR AGENT                          │
│  • Coordinates all other agents                             │
│  • Plans comparison strategy                                │
│  • Manages workflow                                         │
└─────────────────┬───────────────────────────────────────────┘
                  │
     ├────────────┼────────────┬────────────────┐
     │            │            │                │
┌────▼─────┐ ┌───▼────┐ ┌─────▼─────┐ ┌───────▼──────┐
│🔍 SEARCH │ │📊 DATA │ │🧠 ANALYSIS│ │📝 REPORT     │
│ AGENT    │ │SCRAPER │ │  AGENT    │ │ GENERATOR    │
│          │ │ AGENT  │ │           │ │   AGENT      │
└────┬─────┘ └───┬────┘ └─────┬─────┘ └───────┬──────┘
     │           │            │               │
┌────▼─────────────────────────────────────────▼─────┐
│            🌐 WEB AUTOMATION LAYER                  │
│  • Playwright for modern sites                     │
│  • Selenium for legacy compatibility               │
│  • BeautifulSoup for data extraction               │
└─────────────────────────────────────────────────────┘
                           │
┌─────────────────────────▼─────────────────────────────┐
│               🤖 AI PROCESSING LAYER                   │
│  • Gemini Flash (Speed & Cost Efficiency)            │
│  • OpenAI GPT-4 (Deep Analysis & Reasoning)          │
│  • Context Management & Decision Making              │
└─────────────────────────┬─────────────────────────────┘
                          │
┌─────────────────────────▼─────────────────────────────┐
│              📊 LOGGING & MONITORING                   │
│  • MAXIM AI Performance Tracking                     │
│  • Error Handling & Recovery                         │
│  • Usage Analytics & Optimization                    │
└───────────────────────────────────────────────────────┘
```

### How the Agents Work Together:

1. **🎯 Orchestrator Agent**: The team leader that breaks down your request and assigns tasks
2. **🔍 Search Agent**: Finds the best websites and sources for each phone
3. **📊 Data Scraper Agent**: Visits websites and extracts specifications, prices, and reviews
4. **🧠 Analysis Agent**: Compares specs, calculates performance metrics, and finds key differences
5. **📝 Report Generator Agent**: Creates the final markdown comparison document

## 🖼️ Demonstration

### Input Example
```
Compare: iPhone 15 Pro vs Samsung Galaxy S24 Ultra
```

### System in Action

![Agent Workflow](./docs/images/agent-workflow.gif)
*AI agents working together to gather and analyze phone data*

![Data Scraping Process](./docs/images/scraping-process.png)
*Real-time web scraping from multiple tech websites*

![AI Analysis Dashboard](./docs/images/analysis-dashboard.png)
*Gemini Flash and OpenAI processing the collected data*

### Sample Output Report

![Sample Report Header](./docs/images/report-header.png)
*Clean, professional comparison report header*

![Specs Comparison Table](./docs/images/specs-table.png)
*Side-by-side specification comparison*

![Performance Charts](./docs/images/performance-charts.png)
*Visual performance and price comparison charts*

## 🚀 Quick Start

Want to try it out? Here's what you need:

1. **Get API Keys**: You'll need keys for Gemini Flash, OpenAI, and MAXIM AI
2. **Install Dependencies**: Just run the setup script
3. **Compare Phones**: Tell the system which phones to compare
4. **Get Your Report**: Receive a detailed markdown comparison

```bash
# Example usage
python compare_phones.py "iPhone 15 Pro" "Galaxy S24 Ultra"
```

## 🎯 What Makes It Special

**Real-Time Data**: Unlike static comparison websites, we pull live data every time. Prices, availability, and even new reviews are always current.

**Smart Analysis**: Our AI doesn't just list specs - it understands what they mean. It knows that a 120Hz display matters for gaming, or that camera sensor size affects photo quality.

**Human-Friendly Reports**: The output reads like a tech reviewer wrote it, not a robot. Clear explanations, practical advice, and honest recommendations.

**Reliable & Fast**: With MAXIM AI logging, we catch issues before they affect your experience. Most comparisons complete in under 2 minutes.

## 🔧 Tech Stack

- **AI Models**: Gemini Flash (speed), OpenAI GPT-4 (analysis)
- **Web Automation**: Playwright, Selenium, BeautifulSoup
- **Data Processing**: Pandas, NumPy for number crunching
- **Logging**: MAXIM AI for professional monitoring
- **Output**: Clean markdown reports with charts and tables

## 🎨 Sample Comparison Categories

### Hardware Deep Dive
- **Display**: Size, resolution, refresh rate, brightness, color accuracy
- **Performance**: Chipset benchmarks, real-world speed tests, gaming performance
- **Camera**: Sensor specs, sample photo comparisons, video capabilities
- **Battery**: Capacity, charging speed, real-world usage estimates

### Smart Insights
- **Value Analysis**: Price-to-performance ratios and bang-for-buck winners
- **Use Case Matching**: Best phone for photography, gaming, business, etc.
- **Future-Proofing**: Update support, longevity predictions
- **Ecosystem Fit**: How well it works with your other devices

## 🔮 What's Coming Next

- **Video Review Analysis**: Process YouTube reviews for real user experiences
- **Price History Tracking**: See price trends and predict the best time to buy
- **Personalized Recommendations**: Learn your preferences for better suggestions
- **Mobile App**: Compare phones on the go

## 💬 Questions?

This project is constantly evolving based on real user needs. Found a bug? Have a feature idea? Just want to chat about phones? 

- **GitHub Issues**: For bugs and feature requests
- **Discussions**: For general questions and ideas
- **Email**: For anything else

---

*Built with ❤️ for people who want to make smarter phone buying decisions without spending hours researching.*