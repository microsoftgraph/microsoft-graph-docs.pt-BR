---
title: Enviar notificações do feed de atividades aos usuários no Microsoft Teams
description: Envie notificações do feed de atividades aos usuários em Microsoft Teams usando Teams aplicativo e o Microsoft Graph.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
ms.openlocfilehash: 990c7da84691c0cd15ad1362a899180c1f4b08c1
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695027"
---
# <a name="send-activity-feed-notifications-to-users-in-microsoft-teams"></a>Enviar notificações do feed de atividades aos usuários no Microsoft Teams

O Microsoft Teams feed de atividades permite que os usuários triagem itens que exigem atenção notificando-os sobre alterações. Você pode usar as APIs de notificação do feed de atividades no Microsoft Graph para estender essa funcionalidade para seus aplicativos. Isso permite que seus aplicativos forneçam experiências mais avançadas e envolvam melhor os usuários, ajudando a mantê-los atualizados com as alterações nas ferramentas e nos fluxos de trabalho que eles usam.

## <a name="understanding-the-basics-of-activity-feed-notification"></a>Noções básicas da notificação do feed de atividades

As notificações do feed de atividades Microsoft Teams são compostas por vários bits de informações, exibidos juntos, conforme mostrado na imagem a seguir.

![Imagem mostrando componentes de uma notificação do feed de atividades](images/teams-activityfeednotifications/notificationtemplate.png)

Os componentes incluem:
- O ator que iniciou a atividade
- Um ícone que representa o tipo de atividade
- O motivo pelo qual o ator fez a atividade
- Uma visualização de texto
- Um carimbo de data/hora.
- O local da atividade

O exemplo a seguir mostra como esses componentes juntos fornecem os detalhes sobre uma notificação. Este exemplo é uma notificação sobre um usuário mencionado em uma Yammer comunidade.

![Yammer de notificação de ativação](images/teams-activityfeednotifications/examplefeednotification.png)

## <a name="requirements-for-using-the-activity-feed-notification-apis"></a>Requisitos para usar as APIs de notificação do feed de atividades

As APIs do feed de atividades funcionam [com um Teams aplicativo](/microsoftteams/platform/overview). A seguir estão os requisitos para enviar notificações do feed de atividades:

- O Teams manifesto do aplicativo deve ter a Azure AD ID do aplicativo adicionada à `webApplicationInfo` seção. Para obter detalhes, consulte [o esquema de manifesto](/microsoftteams/platform/resources/schema/manifest-schema).
- Os tipos de atividade devem ser declarados na `activities` seção. Para obter detalhes, consulte [o esquema de manifesto](/microsoftteams/platform/resources/schema/manifest-schema).
- O Teams aplicativo deve ser instalado para o destinatário, pessoalmente ou em uma equipe ou [chat](/graph/api/resources/chat?preserve-view=true) do que eles fazem [](/graph/api/resources/team?preserve-view=true) parte. Para obter mais informações, [consulte Teams instalação do aplicativo](/graph/api/resources/teamsappinstallation?preserve-view=true).

### <a name="teams-app-manifest-changes"></a>Teams de manifesto do aplicativo

Esta seção descreve as alterações que precisam ser adicionadas ao Teams manifesto do aplicativo. Observe que você deve estar usando a versão [Teams do manifesto do aplicativo](/microsoftteams/platform/resources/schema/manifest-schema) ou `1.7` superior.

```json
"$schema": "https://developer.microsoft.com/json-schemas/teams/v1.7/MicrosoftTeams.schema.json",
"manifestVersion": "1.7",
````

#### <a name="webapplicationinfo-section-changes"></a>Alterações na seção webApplicationInfo

```json
"webApplicationInfo":
{
    "id": "a3111f15-658e-457c-9689-fd20fe907330",
    "resource": "https://contosoapp.com"
}
```

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|id|string|Azure AD ID do aplicativo (ID do cliente).|
|recurso|string|Recurso associado ao aplicativo Azure AD aplicativo. Também conhecido como URL de resposta ou redirecionamento no Portal do Azure.|

> **Nota:** Você poderá receber um erro se vários Teams aplicativos no mesmo escopo (equipe, chat ou usuário) estão usando o mesmo Azure AD aplicativo. Verifique se você está usando aplicativos Azure AD exclusivos.

#### <a name="activities-section-changes"></a>alterações na seção de atividades

```json
"activities":
{
  "activityTypes": [
    {
      "type": "taskCreated",
      "description": "Task Created Activity",
      "templateText": "{actor} created task {taskId} for you"
    },
    {
      "type": "approvalRequired",
      "description": "Deployment requires your approval",
      "templateText": "{actor} created a new deployment {deploymentId}"
    }
  ]
}
```

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|type|string|Tipo de atividade. Isso precisa ser exclusivo em um manifesto específico.|
|description|string|Descrição curta legível por humanos. Isso ficará visível no cliente Microsoft Teams cliente.|
|templateText|cadeia de caracteres|Texto do modelo para a notificação de atividade. Você pode declarar seus parâmetros encapsulando parâmetros em `{}`.|

>**Nota:** `actor` é um parâmetro especial que sempre usa o nome do chamador. Em chamadas delegadas, `actor` é o nome do usuário. Em chamadas somente de aplicativo, ele usa o nome do Teams aplicativo.

### <a name="installing-the-teams-app"></a>Instalando o Teams aplicativo

Teams aplicativos podem ser instalados em uma equipe, um chat ou para um usuário pessoalmente e podem ser distribuídos de várias maneiras. Para obter detalhes, [consulte Teams de distribuição de aplicativos](/microsoftteams/platform/concepts/deploy-and-publish/overview). Normalmente, o [sideload é](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) preferencial para fins de desenvolvimento. Após o desenvolvimento, você pode escolher o método de distribuição correto com base em se deseja distribuir para um locatário ou para todos os locatários.

Você também pode usar [apIs Teams instalação do](/graph/api/resources/teamsappinstallation?preserve-view=true) aplicativo para gerenciar Teams de aplicativo.

## <a name="sending-activity-feed-notifications-to-users"></a>Enviar notificações do feed de atividades aos usuários

Como um Teams pode ser instalado para um usuário, em uma equipe ou em um chat, as notificações também podem ser enviadas nesses três contextos:

- [Enviar notificação ao usuário em um chat](/graph/api/chat-sendactivitynotification)
- [Enviar notificação ao usuário em uma equipe](/graph/api/team-sendactivitynotification)
- [Enviar notificação ao usuário](/graph/api/userteamwork-sendactivitynotification)

Além disso, as notificações podem ser enviadas em massa para até 100 usuários por vez:

* [Enviar notificações para vários usuários em massa](/graph/api/teamwork-sendactivitynotificationtorecipients)

Para obter detalhes sobre quais tópicos têm suporte para cada cenário, consulte as APIs específicas. Há suporte para tópicos personalizados baseados em texto em todos os cenários.

> **Nota:** O ícone de atividade é baseado no contexto em que a solicitação é feita. Se a solicitação for feita com permissões delegadas, a foto do usuário aparecerá como o avatar, enquanto o ícone Teams aplicativo será exibido como ícone de atividade. Em um contexto somente de aplicativo, o ícone Teams aplicativo é usado como o avatar e o ícone de atividade é omitido.

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a>Exemplo 1: Notificar um usuário sobre uma tarefa criada em um chat

Este exemplo mostra como você pode enviar uma notificação do feed de atividades para uma nova tarefa criada em um chat. Nesse caso, o Teams aplicativo deve ser instalado em um chat com a ID `chatId` `569363e2-4e49-4661-87f2-16f245c5d66a` e o usuário também deve fazer parte do chat.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/{chatId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "12322"
        }
    ]
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-task-created-in-a-team"></a>Exemplo 2: Notificar um usuário sobre uma tarefa criada em uma equipe

Este exemplo mostra como você pode enviar uma notificação do feed de atividades para uma equipe. Este exemplo notifica o proprietário da equipe sobre uma nova tarefa criada que requer sua atenção.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/{teamId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "12322"
        }
    ]
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-a-custom-topic"></a>Exemplo 3: Notificar um usuário sobre um evento usando um tópico personalizado

Como visto nos exemplos anteriores, você pode vincular a diferentes aspectos de uma equipe ou de um chat. No entanto, se você quiser vincular a um aspecto que não faz parte da equipe ou não é representado pelo Microsoft Graph ou se quiser personalizar o nome, `topic` `text` poderá definir a origem do para e passar um valor personalizado para ele. Além disso, `webUrl` é necessário quando você usa a `topic` origem como `text`.

O Yammer de notificação mostrado anteriormente usa um tópico personalizado porque os recursos do Yammer não têm suporte do Microsoft Graph.

> **Nota:** `webUrl` deve começar com o domínio Microsoft Teams (teams.microsoft.com por exemplo).

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Deployment Approvals Channel",
        "webUrl": "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
    },
    "activityType": "approvalRequired",
    "previewText": {
        "content": "New deployment requires your approval"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "deploymentId",
            "value": "6788662"
        }
    ]
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-4-notify-the-team-members-about-an-event"></a>Exemplo 4: notificar os membros da equipe sobre um evento

Este exemplo mostra como você pode enviar uma notificação do feed de atividades para todos os membros da equipe. Este exemplo notifica os membros da equipe sobre um novo evento. 

> **Nota:** Atualmente, a capacidade de enviar notificações a todos os membros da equipe só está disponível na versão beta.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/7155e3c8-175e-4311-97ef-572edc3aa3db/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Weekly Virtual Social",
        "webUrl": "Teams webUrl"
    },
    "previewText": {
        "content": "It will be fun!"
    },
    "activityType": "eventCreated",
    "recipient": {
        "@odata.type": "microsoft.graph.teamMembersNotificationRecipient",
        "teamId": "7155e3c8-175e-4311-97ef-572edc3aa3db"
    }
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-5-notify-the-channel-members-about-an-event"></a>Exemplo 5: notificar os membros do canal sobre um evento

Este exemplo mostra como você pode enviar uma notificação do feed de atividades para todos os membros do canal. Este exemplo notifica os membros do canal sobre um novo evento. 

> **Nota:** Atualmente, a capacidade de enviar notificações para todos os membros do canal só está disponível na versão beta.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/7155e3c8-175e-4311-97ef-572edc3aa3db/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Weekly Virtual Social",
        "webUrl": "Teams webUrl"
    },
    "previewText": {
        "content": "It will be fun!"
    },
    "activityType": "eventCreated",
    "recipient": {
        "@odata.type": "microsoft.graph.channelMembersNotificationRecipient",
        "teamId": "7155e3c8-175e-4311-97ef-572edc3aa3db",
        "channelId": "19:0ea5de04de4743bcb4cd20cb99235d99@thread.tacv2"
    }
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-6-notify-the-chat-members-about-an-event"></a>Exemplo 6: notificar os membros do chat sobre um evento

Este exemplo mostra como você pode enviar uma notificação do feed de atividades para todos os membros do chat. Este exemplo notifica os membros do chat sobre um novo evento. 

> **Nota:** Atualmente, a capacidade de enviar notificações para todos os membros do chat só está disponível na versão beta.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->

``` http
POST https://graph.microsoft.com/beta/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Weekly Virtual Social",
        "webUrl": "Teams webUrl"
    },
    "previewText": {
        "content": "It will be fun!"
    },
    "activityType": "eventCreated",
    "recipient": {
        "@odata.type": "microsoft.graph.chatMembersNotificationRecipient",
        "chatId": "19:d65713bc498c4a428c71ef9353e6ce20@thread.v2"
    }
}
```

#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-7-notify-multiple-users-about-pending-finance-approval-requests"></a>Exemplo 7: Notificar vários usuários sobre solicitações de aprovação de finanças pendentes

O exemplo a seguir mostra como enviar uma notificação do feed de atividades para vários usuários em massa. Este exemplo notifica vários stakeholders sobre solicitações de aprovação de finanças pendentes.

> **Nota:** Atualmente, a capacidade de enviar notificações a vários usuários em massa só está disponível na versão beta.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "teamwork_sendactivitynotificationtorecipients"
}
-->

``` http
POST https://graph.microsoft.com/beta/teamwork/sendActivityNotificationToRecipients
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppId}"
    },
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipients": [
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
        },
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "ab88234e-0874-477c-9638-d144296ed04f"
        },
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "01c64f53-69aa-42c7-9b7f-9f75195d6bfc"
        }
    ],
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
        }
    ] 
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": false
}
-->

``` http
HTTP/1.1 202 Accepted
```

## <a name="customizing-how-the-notifications-alert-you"></a>Personalizando como as notificações alertam você

Microsoft Teams usuários podem personalizar as notificações que veem no feed, como uma faixa e assim por diante. As notificações geradas por meio de APIs do feed de atividades também podem ser personalizadas. Os usuários podem escolher como eles são notificados por meio de configurações Microsoft Teams. Teams aplicativos serão exibidos na lista para o usuário escolher, conforme mostrado na captura de tela a seguir.

![Captura de tela das configurações de Notificações Teams, com a opção Personalizado realçada](images/teams-activityfeednotifications/notificationsettings.png)

Os usuários podem **clicar em Editar** ao lado de um aplicativo e personalizar as notificações, conforme mostrado no exemplo a seguir. O `description` campo no manifesto Teams aplicativo é exibido.

![Captura de tela mostrando notificações personalizadas para Banner e feed para um Teams aplicativo](images/teams-activityfeednotifications/applevelnotificationsettings.png)

## <a name="faqs"></a>Perguntas frequentes

### <a name="who-needs-to-install-the-teams-app"></a>Who precisa instalar o Teams aplicativo?

O usuário de destino deve ter o Teams que está enviando notificações instalado.

### <a name="can-a-user-send-notifications-to-themselves"></a>Um usuário pode enviar notificações para si mesmo?

Não, um usuário não pode enviar notificações para si mesmo. Para esse cenário, use permissões de aplicativo.

### <a name="can-a-teams-app-control-how-the-notifications-are-shown-to-the-user"></a>Um aplicativo Teams pode controlar como as notificações são mostradas ao usuário?

Não, somente os usuários têm permissão para alterar as configurações de notificação.

### <a name="i-installed-my-app-why-dont-i-see-notification-settings-under-the-user-account"></a>Instalei meu aplicativo, por que não vejo as configurações de notificação na conta de usuário?

As configurações aparecerão depois que a primeira notificação for enviada pelo Teams aplicativo. Isso reduz o número de configurações que os usuários veem.

### <a name="i-started-getting-a-409-conflict-error-how-do-i-resolve-it"></a>Comecei a receber um erro 409 (conflito), como faço para resolvê-lo?

`Conflict`ocorrem principalmente quando vários aplicativos Teams instalados no mesmo escopo (equipe, chat, usuário e assim por diante) têm a mesma Azure AD appId `webApplicationInfo` na seção do manifesto. Quando isso acontecer, você receberá um erro como `Found multiple applications with the same Azure AD App ID 'Your AzureAD AppId'.`. Certifique-se de usar aplicativos Azure AD exclusivos para aplicativos Teams exclusivos. Observe que você pode ter o mesmo aplicativo Teams instalado em vários escopos (equipe + usuário, por exemplo).

## <a name="see-also"></a>Confira também

* [Práticas recomendadas para usar Microsoft Teams de feed de atividades](teams-activity-feed-notifications-best-practices.md)
* [Criar notificações do feed de atividades para Microsoft Teams](/microsoftteams/platform/concepts/design/activity-feed-notifications?tabs=mobile)
