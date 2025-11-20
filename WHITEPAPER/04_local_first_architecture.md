# Local-First Architecture Overview

## Components:
- **Ollama**: Local LLM runner
- **LM Studio**: Model hosting and management
- **FlameRouter**: Custom orchestrator handling request routing and fallbacks

## Architecture Flow:
1. User sends input to local agent.
2. FlameRouter checks for:
   - Local model availability  
   - Resource load  
   - Fallback conditions (only triggered manually or intentionally)
3. Response is streamed from local LLM.

## Advantages:
- Privacy  
- Latency control  
- Zero dependency on external APIs  
- Air-gap capability  
