# 🛠️ DroidPenKit.ps1 — Ferramenta de Automação para Pentest Mobile Android (ADB & Frida)

O DroidPenKit é um script em PowerShell desenvolvido para automatizar tarefas comuns em testes de segurança mobile em ambientes Android. Ele integra o uso de ADB, Emulador Android e Frida, oferecendo uma interface interativa por linha de comando para facilitar operações de análise, injeção de scripts, instalação de APKs, gerenciamento de pacotes e muito mais.

<img width="740" height="1146" alt="image" src="https://github.com/user-attachments/assets/ea9d9d2e-156d-4d20-ad4a-221f226c508e" />

--

<img width="794" height="233" alt="image" src="https://github.com/user-attachments/assets/63ac0392-f80e-411f-8b93-a1b25de8e2d5" />

--

<img width="762" height="87" alt="image" src="https://github.com/user-attachments/assets/4184ef80-88ce-4662-b797-548fa45dfaab" />

--

<img width="757" height="98" alt="image" src="https://github.com/user-attachments/assets/f5b2acf1-25f3-402c-902f-4bdf894ea644" />

--

<img width="768" height="63" alt="image" src="https://github.com/user-attachments/assets/cc01adf2-2536-4b23-8d19-f0311a0d8521" />

--

<img width="1275" height="226" alt="image" src="https://github.com/user-attachments/assets/cbc61530-2c13-4f31-985f-7928d336dcaf" />

--

<img width="898" height="640" alt="image" src="https://github.com/user-attachments/assets/fbae0500-c5e9-4a36-b1e7-7098e3760178" />

--

<img width="932" height="525" alt="image" src="https://github.com/user-attachments/assets/9a100749-a103-4695-8f4d-ea0d731b71b5" />

--

<img width="1489" height="792" alt="image" src="https://github.com/user-attachments/assets/0142027c-a1e4-4dd7-9688-d5a586a2a2f0" />

--

<img width="948" height="873" alt="image" src="https://github.com/user-attachments/assets/37d374db-8920-43a3-8a75-679de508f293" />

---
🔹 Principais Recursos:

- Automação completa de comandos ADB

- Suporte a emuladores Android (AVD)

- Execução e controle de Frida Server / Scripts JS

- Instalação, remoção e manipulação de APKs

- Captura de logs e filtragem com logcat / grep / PID

- Gerenciamento de permissões, pacotes e dados de aplicativos

- Execução por menu interativo ou via parâmetros diretos (.\DroidPenKit.ps1 5)

💻 Ideal para analistas de segurança, desenvolvedores e pentesters que buscam agilidade e padronização nos testes de aplicativos Android.

---

# 🛠 Ferramentas Necessárias para funcionamento


🔹 Android SDK Platform-Tools (adb)

Comunicação com dispositivos e emuladores. O script chama diretamente o adb.exe em:
%USERPROFILE%\AppData\Local\Android\Sdk\platform-tools\adb.exe

🔹 Verifique:

& "$env:USERPROFILE\AppData\Local\Android\Sdk\platform-tools\adb.exe" version


Alternativa: adicione platform-tools ao PATH para chamar adb diretamente.

🔹Android Emulator (emulator)

Listagem e inicialização de AVDs (várias opções do menu usam isso). Path padrão no script:
%USERPROFILE%\AppData\Local\Android\Sdk\emulator\emulator.exe

🔹Verifique:

- & "$env:USERPROFILE\AppData\Local\Android\Sdk\emulator\emulator.exe" -version

- Frida (frida, frida-ps)

Listar processos, aplicações e injetar scripts (várias opções do menu — inclusive múltiplos scripts).

🔹Instale via pip: pip install frida-tools frida (ou conforme sua preferência).

Verifique:

- frida --version
- frida-ps --version



🔹 Como checar rapidamente (exemplos)
- & "$env:USERPROFILE\AppData\Local\Android\Sdk\platform-tools\adb.exe" version
- & "$env:USERPROFILE\AppData\Local\Android\Sdk\emulator\emulator.exe" -version
- frida --version
- frida-ps --version

---
## 🧠 Referências

- [OWASP Mobile Top 10](https://owasp.org/www-project-mobile-top-10/)
- [Android Security Guide](https://source.android.com/security)
- [iOS Security Guide](https://support.apple.com/guide/security/welcome/web)
- [Mobile Security Testing Guide (MSTG)](https://mobile-security.gitbook.io/mobile-security-testing-guide/)

---

## ⚠️ Aviso Legal

> Este repositório tem fins **educacionais**. Não me responsabilizo pelo uso indevido das técnicas e ferramentas aqui apresentadas. Utilize com ética e responsabilidade.

---

## 🤝 Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para abrir *issues* ou enviar *pull requests* com correções, melhorias ou novos conteúdos.

---

## 📧 Contato

Caso queira trocar ideias ou sugerir algo:

- [Carlos Tuma](https://github.com/carlosalbertotuma)
- E-mail: bl4dsc4n@gmail.com

