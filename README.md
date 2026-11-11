🔐 CyberTech | Controle de Acesso em Linux

📌 Sobre o projeto

Laboratório prático desenvolvido no *Debian Linux 13*, simulando uma empresa fictícia com dois departamentos: Financeiro e Suporte.

*Objetivo:* aplicar o princípio do menor privilégio, restringindo o acesso a arquivos financeiros apenas aos usuários autorizados.

🛠️ Tecnologias utilizadas

- Debian GNU/Linux 13 (máquina virtual)
- Terminal Linux
- Gerenciamento de usuários e grupos
- Comandos: `adduser`, `groupadd`, `usermod`, `chmod`, `chgrp` e `sudo`

⚙️ Implementação

Foram criados dois usuários e seus respectivos grupos:

| Usuário | Grupo |
|---|---|
| Joao | Financeiro |
| Pedro | Suporte |

Foi criado o diretório `/srv/cybertech/Financeiro`, com permissão `770`, e o arquivo `relatorio_financeiro.txt`, com permissão `660`.

Essas configurações permitem que integrantes autorizados do grupo Financeiro leiam e modifiquem o relatório, enquanto usuários sem permissão não conseguem acessá-lo.

🧪 Testes e resultados

| Teste realizado | Resultado |
|---|---|
| Joao acessa o diretório Financeiro | ✅ Permitido |
| Pedro tenta acessar o diretório | ❌ Negado |
| Joao lê e modifica o relatório | ✅ Permitido |
| Pedro tenta ler e modificar o relatório | ❌ Negado |

📷 Evidências

As capturas dos testes realizados no terminal serão disponibilizadas na pasta `evidencias/`.

🎯 Aprendizados

O projeto permitiu aplicar conceitos de **controle de acesso, permissões Linux, gerenciamento de identidades e princípio do menor privilégio**, validando na prática o funcionamento das restrições configuradas.

---

*Projeto educacional desenvolvido em ambiente virtualizado, utilizando dados fictícios.*

As capturas dos comandos e resultados serão organizadas na pasta `evidencias/`.

---

**Projeto educacional realizado em ambiente virtualizado, utilizando contas e informações fictícias.**
