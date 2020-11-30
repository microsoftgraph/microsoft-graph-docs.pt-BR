---
title: Enviar notificações de feed de atividades para usuários no Microsoft Teams
description: Enviar notificações de feed de atividades para usuários no Microsoft Teams usando o Teams app e o Microsoft Graph.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 33a44ef158a1336e198e7382e144efed11ff35e7
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377423"
---
# <a name="send-activity-feed-notifications-to-users-in-microsoft-teams"></a>Enviar notificações de feed de atividades para usuários no Microsoft Teams

O feed de atividades do Microsoft Teams permite que os usuários façam a triagem de itens que exigem atenção ao notificá-los das alterações. Você pode usar as APIs de notificação do feed de atividades no Microsoft Graph para estender essa funcionalidade para seus aplicativos. Isso permite que seus aplicativos ofereçam experiências mais ricas e envolvam melhor os usuários, ajudando a mantê-los atualizados com as ferramentas e os fluxos de trabalho usados.

## <a name="understanding-the-basics-of-activity-feed-notification"></a>Noções básicas sobre a notificação do feed de atividades

As notificações do feed de atividades no Microsoft Teams são compostas por vários bits de informações, exibidas juntas, conforme mostrado na imagem a seguir.

![Imagem mostrando componentes de uma notificação de feed de atividades](images/teams-activityfeednotifications/notificationtemplate.png)

Os componentes incluem:
- O ator que iniciou a atividade
- Um ícone que representa o tipo de atividade
- O motivo pelo qual o ator fazia a atividade
- Uma visualização de texto
- Um carimbo de data/hora
- O local da atividade

O exemplo a seguir mostra como esses componentes fornecem os detalhes sobre uma notificação. Este exemplo é uma notificação sobre um usuário mencionado em uma comunidade do Yammer.

![Exemplo de notificação do Yammer actifity](images/teams-activityfeednotifications/examplefeednotification.png)

## <a name="requirements-for-using-the-activity-feed-notification-apis"></a>Requisitos para o uso das APIs de notificação do feed de atividades

As APIs de feed de atividades trabalham com um [aplicativo do teams](/microsoftteams/platform/overview). Estes são os requisitos para o envio de notificações de feed de atividades:

- O manifesto do aplicativo Teams deve ter a ID de aplicativo do Azure AD adicionada à `webApplicationInfo` seção. Para obter detalhes, consulte [esquema de manifesto](/microsoftteams/platform/resources/schema/manifest-schema).
- Os tipos de atividade devem ser declarados na `activities` seção. Para obter detalhes, consulte [esquema de manifesto](/microsoftteams/platform/resources/schema/manifest-schema).
- O aplicativo Teams deve estar instalado para o destinatário, pessoalmente ou em uma [equipe](/graph/api/resources/team?preserve-view=true) ou em um [chat](/graph/api/resources/chat?preserve-view=true) do qual fazem parte. Para obter mais informações, consulte [Team app Installation](/graph/api/resources/teamsappinstallation?preserve-view=true).

### <a name="teams-app-manifest-changes"></a>Alterações de manifesto do aplicativo do teams

Esta seção descreve as alterações que precisam ser adicionadas ao manifesto do teams app. Observe que você deve estar usando a versão de [manifesto do aplicativo Teams](/microsoftteams/platform/resources/schema/manifest-schema) `1.7` ou superior.

```json
"$schema": "https://developer.microsoft.com/json-schemas/teams/v1.7/MicrosoftTeams.schema.json",
"manifestVersion": "1.7",
````

#### <a name="webapplicationinfo-section-changes"></a>alterações da seção webApplicationInfo

```json
"webApplicationInfo":
{
    "id": "a3111f15-658e-457c-9689-fd20fe907330",
    "resource": "https://contosoapp.com"
}
```

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|id|string|ID de aplicativo do Azure AD (ID do cliente).|
|recurso|string|Recurso associado ao aplicativo do Azure AD. Também conhecido como resposta ou URL de redirecionamento no portal do Azure.|

> **Observação:** Você pode receber um erro se vários aplicativos do teams no mesmo escopo (equipe, chat ou usuário) estiverem usando o mesmo aplicativo do Azure AD. Certifique-se de que você está usando aplicativos exclusivos do Azure AD.

#### <a name="activities-section-changes"></a>alterações na seção atividades

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
|description|string|Descrição curta legível. Isso estará visível no cliente Microsoft Teams.|
|templateText|string|Texto de modelo para a notificação de atividade. Você pode declarar seus parâmetros ao encapsular parâmetros no `{}` .|

>**Observação:** `actor` é um parâmetro especial que sempre Obtém o nome do chamador. Em chamadas delegadas, `actor` é o nome do usuário. Em chamadas somente aplicativo, ele utiliza o nome do aplicativo Teams.

### <a name="installing-the-teams-app"></a>Instalando o aplicativo Teams

Os aplicativos do teams podem ser instalados em uma equipe, um chat ou um usuário pessoalmente e podem ser distribuídos de várias maneiras. Para obter detalhes, consulte [Teams app Distribution Methods](/microsoftteams/platform/concepts/deploy-and-publish/overview). Normalmente, o [Sideload](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) é preferido para fins de desenvolvimento. Após o desenvolvimento, você pode escolher o método de distribuição certo com base em se deseja distribuir para um locatário ou para todos os locatários.

Você também pode usar as APIs de [instalação de aplicativos do teams](/graph/api/resources/teamsappinstallation?preserve-view=true) para gerenciar instalações de aplicativos do teams.

## <a name="sending-activity-feed-notifications-to-users"></a>Enviando notificações de feed de atividades para usuários

Como um aplicativo do teams pode ser instalado para um usuário, em uma equipe ou em um chat, as notificações também podem ser enviadas nesses três contextos:

- [Enviar notificação para o usuário em um chat](/graph/api/chat-sendactivitynotification)
- [Enviar notificação para o usuário em uma equipe](/graph/api/team-sendactivitynotification)
- [Enviar notificação para o usuário](/graph/api/userteamwork-sendactivitynotification)

Para obter detalhes sobre quais tópicos têm suporte para cada cenário, consulte as APIs específicas. Os tópicos personalizados baseados em texto são compatíveis com todos os cenários.

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a>Exemplo 1: notificar um usuário sobre uma tarefa criada em um chat

Este exemplo mostra como você pode enviar uma notificação de feed de atividades para uma nova tarefa criada em um chat. Nesse caso, o aplicativo Teams deve ser instalado em um chat com ID `chatId` e `569363e2-4e49-4661-87f2-16f245c5d66a` o usuário também deve fazer parte do chat.

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

### <a name="example-2--notify-a-user-about-a-task-created-in-a-team"></a>Exemplo 2: notificar um usuário sobre uma tarefa criada em uma equipe

Este exemplo mostra como você pode enviar uma notificação de feed de atividades para uma equipe. Este exemplo notifica o proprietário da equipe sobre uma nova tarefa criada que requer sua atenção.

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

### <a name="example-3-notify-a-user-about-an-event-using-a-custom-topic"></a>Exemplo 3: notificar um usuário sobre um evento usando um tópico personalizado

Como visto nos exemplos anteriores, você pode vincular a diferentes aspectos de uma equipe ou de um chat. No entanto, se você deseja vincular a um aspecto que não faz parte da equipe ou não é representado pelo Microsoft Graph, ou se você deseja personalizar o nome, você pode definir a fonte do `topic` para `text` e passar um valor personalizado para ele. Além disso, `webUrl` é necessário ao usar `topic` source como `text` .

O exemplo de notificação do Yammer mostrado anteriormente usa um tópico personalizado porque os recursos do Yammer não são suportados pelo Microsoft Graph.

> **Observação:** `webUrl` deve começar com o domínio do Microsoft Teams (teams.microsoft.com, por exemplo).

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
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
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

## <a name="customizing-how-the-notifications-alert-you"></a>Personalizando como o alerta de notificações você

Os usuários do Microsoft Teams podem personalizar as notificações que eles vêem no feed, como uma faixa e assim por diante. As notificações geradas por meio das APIs de feed de atividades também podem ser personalizadas. Os usuários podem escolher como são notificados via configurações no Microsoft Teams. Os aplicativos do teams aparecerão na lista para o usuário escolher, conforme mostrado na captura de tela a seguir.

![Captura de tela das configurações de notificações no Teams, com a opção personalizada realçada](images/teams-activityfeednotifications/notificationsettings.png)

Os usuários podem clicar em **Editar** ao lado de um aplicativo e personalizar as notificações, conforme mostrado no exemplo a seguir. O `description` campo no manifesto do aplicativo Teams é exibido.

![Captura de tela mostrando notificações personalizadas para banner e feed para um aplicativo do teams](images/teams-activityfeednotifications/applevelnotificationsettings.png)
