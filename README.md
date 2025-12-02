# GrafanaToolServer (by Cumhur Akkaya)
The GrafanaToolServer works by wrapping Grafana’s API endpoints into tool functions that AI agents (e.g., Claude, OpenAI GPT, or other MCP-compatible models) can invoke.

## 🎯 Why This Project?
Grafana Tool Server acts as a utility server that exposes Grafana capabilities to AI models like the MCP ecosystem. It allows LLMs to interact with Grafana dashboards, query Prometheus data, trigger alerts, or retrieve metrics - all through secure, permissioned tool calls.
The GrafanaToolServer works by wrapping Grafana's API endpoints into tool functions that AI agents (e.g., Claude, OpenAI GPT, or other MCP-compatible models) can invoke. This enables automated observability, diagnosis, and metric analysis directly through conversational AI.

We will use the Grafana Tool Server in the integration of Ollama and LLMs.

## 🔧 Architecture

```
┌──────────────────┐
│   Ollama Web UI  │
│  (Ollama + LLMs) │
└────────┬─────────┘
         │ MCP Protocol
         │ 
┌────────▼─────────┐
│ GrafanaToolServer│ Docker +
│  (This Project)  │ Python
└────────┬─────────┘
         │ n8n workflow
         │
┌────────▼────────┐
│ Grafana Server  │
│      API        │
└─────────────────┘
```

----------

## Related Article:  Step-by-Step Tutorial: Observability 3.0: AI-Powered APM = Claude (cloud-based) / Ollama (self-hosted) + MCP Server + Observability Stack 

<img width="4877" height="3408" alt="image" src="https://github.com/user-attachments/assets/2f026eaf-bd8c-44b2-969a-eae52f3188ff" />

In today’s cloud-based world, observability is no longer just about collecting logs, metrics, and traces. We can take observability to the next level with AI-powered APM (Application Performance Monitoring). Tools like Claude (cloud-based AI) and Ollama (self-hosted AI), combined with Prometheus, Grafana, Loki, Tempo, and OpenTelemetry, enable us to create an intelligent observability ecosystem. In this hands-on guide, I’ll show you step-by-step how to integrate AI with observability platforms. We’ll run with various LLM models and compare their results. The integration of AI and observability systems will enable real-time anomaly detection and faster root cause analysis for your systems. I will share with you a comprehensive overview of my experiences with integrating AI and observability systems.

## 📗 Medium Articles Link:

- [📝Observability 3.0 AI-Powered APM = Claude (cloud-based) / Ollama (self-hosted) + MCP Server + n8n + Prometheus, Grafana, Loki, Tempo, OpenTelemetry, PostgreSQL Exporter, Node Exporter, cAdvisor, Promtail, Alert Manager — A Comprehensive Hands-On Guide for Live Monitoring with LLMs (Large Language Models)](https://cmakkaya.medium.com/observability-3-0-ai-powered-apm-claude-cloud-based-ollama-self-hosted-mcp-server-n8n-monitor-6ea436e271fe?postPublishedType=repub) `happy reading.`

- [📝Introduction Observability 3.0: AI-Powered APM = AI Stack + Observability Stack— A Hands-On Guide (Part-2)](https://cmakkaya.medium.com/introduction-observability-3-0-ai-powered-apm-ai-stack-observability-stack-part-2-33b1d6a262d7?postPublishedType=repub) `happy reading.`

- [📝Observability 3.0: AI-Powered APM = Ollama (self-hosted) + GrafanaToolServer + Observability Stack — A Comprehensive Hands-On Guide for Live Monitoring with LLMs (Part-3)]() `soon.`

- [📝Observability 3.0: AI-Powered APM = Claude (cloud-based) + MCP Server + Observability Stack — A Comprehensive Hands-On Guide for Live Monitoring with LLMs (Part-4)]() `soon.`



## Hi there, <img src = "https://github.com/cmakkaya/cmakkaya/blob/main/wavehand.gif" width = "40" align="center"> Nice to see you. <img src="https://emojis.slackmojis.com/emojis/images/1531849430/4246/blob-sunglasses.gif?1531849430" width="40"/>  

✏️ Don't forget to follow [my LinkedIn account](https://www.linkedin.com/in/cumhurakkaya/) or [my Medium account](https://cmakkaya.medium.com/)  to be informed about new updates in the repository.

⭐ Also, thank you for giving `stars` to my GitHub.

I hope they are useful to you.

🙏 I wish you growing success.

## 🤝 Contributing

We welcome your contributions! Feel free to send pull requests.

1. Fork it
2. Create your feature branch (`git checkout -b feature/amazing`)
3. Commit your changes (`git commit -m 'feat: Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing`)
5. Open a Pull Request

----------
### Connect with me 📫 You can learn more about me

- 🌐 [LinkedIn](https://www.linkedin.com/in/cumhurakkaya/)
- ✏️ [Medium Articles](https://cmakkaya.medium.com/)  100+ Articles
- 🌐 [GitHub](https://github.com/cmakkaya/)

----------
## 📝 License

MIT License - See [LICENSE](LICENSE) file for details.

----------

## 🙏 Acknowledgments

- [Anthropic](https://anthropic.com) - For Claude and MCP protocol
- [Model Context Protocol](https://modelcontextprotocol.io) - For excellent documentation
