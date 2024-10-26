# 📢 Wizzard Emitter

Uma biblioteca de notificações interna para aplicações Node.js que permite a criação, armazenamento e gerenciamento dinâmico de notificações via eventos. 

## 🚀 Funcionalidades

- **Emissão de Notificações**: Emita notificações facilmente com base em eventos.
- **Armazenamento em Memória**: Armazene notificações temporariamente até que sejam limpas ou o servidor reiniciado.
- **Manipulação Dinâmica**: Adicione campos personalizados e dinâmicos às notificações.
- **API Simples**: Interface RESTful para interagir com as notificações.

## 📦 Instalação

Para instalar a biblioteca, utilize Bun:

```bash
bun add wizzard-emitter
```

## ⚙️ Uso Básico

Aqui está um exemplo de como usar a biblioteca em seu projeto Node.js:

```javascript
import { createNotification, getNotifications, clearNotifications } from 'wizzard-emitter';

// Criando uma nova notificação
createNotification({
  message: 'Esta é uma notificação!',
  dynamicFields: { user: 'Erivaldo', priority: 'high' }
});

// Obtendo todas as notificações
const notifications = getNotifications();
console.log(notifications);

// Limpando todas as notificações
clearNotifications();
```

## 📜 Roadmap

O roadmap a seguir apresenta as funcionalidades planejadas para futuras versões da biblioteca:

### Q4 2024
- **📈 Persistência de Notificações**: Implementar armazenamento em banco de dados (PostgreSQL, MongoDB).
- **📅 Notificações Agendadas**: Adicionar suporte para agendar notificações para serem disparadas no futuro.

### Q1 2025
- **🔍 Filtragem de Notificações**: Implementar filtros para consultar notificações com base em atributos dinâmicos e timestamps.
- **🔔 Notificações de Vários Tipos**: Expandir a biblioteca para suportar diferentes tipos de notificações (alertas, lembretes, etc.).

### Q2 2025
- **📊 Integração com Sistemas de Mensageria**: Permitir integração com serviços como RabbitMQ ou Kafka para gestão de notificações em larga escala.
- **📖 Documentação Completa**: Criar documentação abrangente com exemplos e melhores práticas.

## 🧪 Testes

Para garantir a qualidade do código, a biblioteca inclui testes automatizados. Para executar os testes, utilize:

```bash
bun test
```

## 🌟 Contribuições

Contribuições são bem-vindas! Se você deseja contribuir para o desenvolvimento da biblioteca, siga estas etapas:

1. Faça um fork do repositório.
2. Crie uma nova branch (`git checkout -b feature/novofuncionalidade`).
3. Faça suas alterações e commit (`git commit -m 'Adicionando nova funcionalidade'`).
4. Envie para o seu fork (`git push origin feature/novofuncionalidade`).
5. Abra um Pull Request.

## 📄 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

---

## 🗣️ Feedback e Suporte

Se você encontrar problemas ou tiver perguntas, sinta-se à vontade para abrir uma [issue](https://github.com/erivaldocazinga22/wizzard-emitter/issues) no GitHub. Agradecemos seu feedback!

---

**Obrigado por usar a Notification Library! 🚀**