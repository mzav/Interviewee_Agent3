# **Interviewee Agent**

![Deploy](https://github.com/dimadem/ai-agent-conversation/actions/workflows/digitalocean-deploy.yml/badge.svg)

#### **requirenments.txt**
[FASTAPI](https://fastapi.tiangolo.com/)

[UVICORN](https://pypi.org/project/uvicorn/)

[OPENAI](https://platform.openai.com/docs/api-reference/responses)

[OPENAI AGENT SDK](https://openai.github.io/openai-agents-python/)

[OPENAI FM](https://www.openai.fm/)

---

### **Setup**

1. собрать проект -> ./setup.sh
2. добавить нужные ключи в .env файл
3. запустить проект -> ./dev.sh

---

### **Deploy**

1. В репозитории -> Settings
2. Secrets and Variables -> Repository secrets
3. DROPLET_IP -> current ip
4. DROPLET_PASSWORD -> current password
5. OPENAI_API_KEY -> current openai api key

### **Development**
1. 

---

### **Описание**

```
⎿  📁 app
     ├─ 📄 __init__.py
     ├─ 📁 agents                <!-- Агенты для различных задач -->
     │  ├─ 📄 evaluation_agent.py
     │  ├─ 📄 interviewee_agent.py
     │  ├─ 📁 prompts            <!-- Шаблоны и утилиты для агентов -->
     │  │  ├─ 📄 __init__.py
     │  │  ├─ 📄 evaluation_system_prompt.yaml
     │  │  ├─ 📄 persona_system_prompt.yaml
     │  │  ├─ 📄 utils.py
     │  ├─ 📁 tools              <!-- Инструменты для агентов -->
     │  │  ├─ 📄 extract_action.py
     │  │  ├─ 📄 extract_result.py
     │  │  ├─ 📄 extract_situation.py
     │  │  ├─ 📄 extract_task.py
     │  │  ├─ 📄 lie_answer.py
     ├─ 📁 api                   <!-- API для взаимодействия с фронтендом -->
     │  ├─ 📄 __init__.py
     │  ├─ 📄 evaluation.py
     │  ├─ 📄 interview.py
     ├─ 📁 core                  <!-- Основные конфигурации и константы -->
     │  ├─ 📄 __init__.py
     │  ├─ 📄 config.py
     │  ├─ 📄 constants.py
     │  ├─ 📄 openai.py
     ├─ 📁 frontend              <!-- HTML файлы для фронтенда -->
     │  ├─ 📄 evaluation.html
     │  ├─ 📄 index.html
     │  ├─ 📄 interview.html
     │  ├─ 📄 report.html
     │  ├─ 📄 select-candidate.html
     ├─ 📄 main.py               <!-- Главный файл запуска приложения -->
     ├─ 📁 model                 <!-- Модели для обработки данных -->
     │  ├─ 📄 __init__.py
     │  ├─ 📄 stt.py
     │  ├─ 📄 tts.py
     │  ├─ 📄 ttt.py
     ├─ 📁 utils                 <!-- Утилиты и вспомогательные функции -->
     │  └─ 📄 __init__.py
```

---
