# <a name="microsoft-teams-api-overview-preview"></a>Visão geral da API de equipes da Microsoft (versão prévia)

O Microsoft Teams é o melhor hub para trabalhos em equipe e comunicações inteligentes. Criado com base na força e na escala do Office 365, que conta com mais de 120 milhões de usuários, o Microsoft Teams oferece recursos de colaboração, reuniões, chamadas e voz empresarial baseados em bate-papo.

## <a name="why-integrate-with-microsoft-teams"></a>Por que integrar-se com o Microsoft Teams?

A integração com o Microsoft Teams facilita a criação de seus próprios serviços e aplicativos, atingindo milhões de usuários corporativos e ajudando as pessoas a trabalhar em conjunto. Você pode usar o Microsoft Graph para criar e gerenciar equipes, canais, mensagens e muito mais.

### <a name="use-microsoft-graph-in-any-kind-of-app"></a>Use o Microsoft Graph em qualquer tipo de aplicativo

Os aplicativos do Microsoft Teams criados no Microsoft Graph oferecem aos grupos de trabalho uma nova ferramenta para tornar a colaboração mais produtiva e atraente. Com o Microsoft Teams, os usuários do grupo de trabalho compartilham recursos, interagem pelo bate-papo e agendam eventos no calendário da equipe. Aumente o valor do Microsoft Teams adicionando automação de equipe, canal e conversas usando aplicativos baseados na API do Microsoft Teams.

Os sites, serviços e aplicativos de plataformas nativas não são executados na experiência do usuário do Microsoft Teams, mas podem ser usados para chamar as APIs do Microsoft Teams que habilitam os cenários de automação do Microsoft Teams.

**Tipos de aplicativos habilitados para o Microsoft Teams**

![Chame a API do Microsoft Teams em guias, bots, sites e serviços](images/TeamsAppEndpoints.png)

Essas ferramentas de colaboração incluem guias habilitadas para o Microsoft Graph ou aplicativos de bot executados no Microsoft Teams. Você também pode chamar o Microsoft Graph fora de um aplicativo do Microsoft Teams, como de um site ou de serviço Web. Se já tiver habilitado seu site para o Microsoft Graph, você poderá usar esse trabalho para o Microsoft Teams utilizando a [plataforma de desenvolvedor do Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/#pivot=home&panel=home-all) para criar um aplicativo de guias que usa o código de site existente.

Se um aplicativo de bot ou uma guia do Microsoft Teams não for a maneira ideal de concluir seu cenário, escolha um dos seguintes tipos de aplicativos.

|Tipo de aplicativo|Descrição do cenário|
|:-------|:-------------------|
|Guias|Exiba conteúdo aprimorado no Microsoft Teams.|
|Conectores|Poste atualizações aprimoradas nos canais.|
|Mensagens acionáveis|Adicione interação aprimorada aos cartões do conector.|
|Sites|Exiba conteúdo aprimorado em suas páginas da Web.|
|Bots|Ajude os usuários a concluir tarefas em conversas.|
|Feed de atividades|Envolva os usuários por meio de notificações do feed.|
|Extensões de mensagens|Permita que os usuários consultem e compartilhem cartões aprimorados em conversas.|
|Serviços|Aprimore seus aplicativos cliente com dados do Microsoft Graph por meio do seu serviço Web.|

### <a name="create-multiple-teams-and-channels"></a>Criar várias equipes e canais

Permita que seus clientes criem novas [equipes](../api-reference/beta/resources/team.md) e [canais](../api-reference/beta/resources/channel.md) vinculados ao seu aplicativo. Facilite a criação de um grande número de equipes e o preenchimento delas com usuários e canais usando a API do Microsoft Teams.

### <a name="automate-team-lifecycles"></a>Automatizar o ciclo de vida da equipe

Use o Microsoft Graph para criar uma nova equipe virtual quando surgir um novo problema de negócios, [preencha a equipe](../api-reference/v1.0/api/group_post_members.md) com as pessoas certas e configure canais para a equipe. Para iniciar uma discussão no canal da equipe sobre o novo problema de negócios, você pode propagar o canal com um novo tópico de conversa para postar uma mensagem de boas-vindas aos novos membros da equipe. Se quiser reunir a nova equipe para discutir o problema de negócios, adicione um novo evento à agenda da equipe e convide os membros da equipe para o evento.

Quando o problema de negócios for resolvido e você já não precisar da equipe virtual, use a API do Microsoft Teams para desfazer a equipe. Se, ao criar a equipe virtual, você souber qual será sua duração máxima, defina uma [política de expiração de grupo do Office 365](https://support.office.com/en-us/article/office-365-group-expiration-policy-8d253fe5-0e09-4b3c-8b5e-f48def064733?ui=en-US&rs=en-US&ad=US) para a equipe que removerá automaticamente a equipe de acordo com o que foi definido na política.

## <a name="next-steps"></a>Próximas etapas

- Saiba como [usar a API do Microsoft Teams](../api-reference/beta/resources/teams_api_overview.md).
- Analise em detalhes os métodos, propriedades e relações dos recursos de [equipe](../api-reference/beta/resources/team.md), [canal](../api-reference/beta/resources/channel.md) e [grupo](../api-reference/v1.0/resources/group.md).
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/en-us/graph/graph-explorer).
- Leia mais sobre o [modelo de programação do Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/concepts-overview).
- Comece a trabalhar com um [código de exemplo](https://github.com/OfficeDev/microsoft-teams-sample-graph).
