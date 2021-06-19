---
title: Obter notificações de alteração para qualquer alteração na associação do Teams usando o Microsoft Graph
description: Obter notificações de alteração para quaisquer alterações (criar, atualizar e excluir) na associação do Teams usando o Microsoft Graph
author: anandab
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 4e8d403354c16f7f11fd4c7dcf6b756f83242cda
ms.sourcegitcommit: 39a8c6eccc07ead237dac17387cd269733a86abd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53025023"
---
# <a name="get-change-notifications-for-changes-in-teams-membership-using-microsoft-graph"></a><span data-ttu-id="42863-103">Obter notificações de alteração para alterações na associação do Teams usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="42863-103">Get change notifications for changes in Teams membership using Microsoft Graph</span></span>

<span data-ttu-id="42863-104">As notificações de alteração permitem que você se inscreva para receber alterações (criar, atualizar e excluir) na associação do Teams.</span><span class="sxs-lookup"><span data-stu-id="42863-104">Change notifications enable you to subscribe to changes (create, update, and delete) in teams membership.</span></span> <span data-ttu-id="42863-105">Você pode ser notificado sempre que um membro for adicionado, removido ou atualizado em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="42863-105">You can get notified whenever member is added, removed or updated in a team.</span></span> <span data-ttu-id="42863-106">Você também pode obter os dados do recurso nas notificações e, portanto, evitar chamar a API para obter o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="42863-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

## <a name="subscribe-to-changes-in-membership-of-a-particular-team"></a><span data-ttu-id="42863-107">Inscrever-se para receber alterações na associação de uma equipe específica</span><span class="sxs-lookup"><span data-stu-id="42863-107">Subscribe to changes in membership of a particular team</span></span>

<span data-ttu-id="42863-108">Para obter notificações de alterações para alterações de membros em uma equipe específica, inscreva-se em `/teams/{team-id}/members`.</span><span class="sxs-lookup"><span data-stu-id="42863-108">To get change notifications for membership changes in a particular team, subscribe to `/teams/{team-id}/members`.</span></span> <span data-ttu-id="42863-109">Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.</span><span class="sxs-lookup"><span data-stu-id="42863-109">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="42863-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="42863-110">Permissions</span></span>

|<span data-ttu-id="42863-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42863-111">Permission type</span></span>      | <span data-ttu-id="42863-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42863-112">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="42863-113">Versões com suporte</span><span class="sxs-lookup"><span data-stu-id="42863-113">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="42863-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42863-114">Delegated (work or school account)</span></span> | <span data-ttu-id="42863-115">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42863-115">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> | <span data-ttu-id="42863-116">beta</span><span class="sxs-lookup"><span data-stu-id="42863-116">beta</span></span> |
|<span data-ttu-id="42863-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42863-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42863-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42863-118">Not supported.</span></span>    | <span data-ttu-id="42863-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42863-119">Not supported.</span></span> |
|<span data-ttu-id="42863-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42863-120">Application</span></span> | <span data-ttu-id="42863-121">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42863-121">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span></span>   | <span data-ttu-id="42863-122">beta</span><span class="sxs-lookup"><span data-stu-id="42863-122">beta</span></span> |

><span data-ttu-id="42863-123">**Nota:** As permissões marcadas com \* são suportadas como parte do [consentimento específico do recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span><span class="sxs-lookup"><span data-stu-id="42863-123">**Note:** Permissions marked with \* are supported as part of [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

#### <a name="example"></a><span data-ttu-id="42863-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42863-124">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,deleted,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/members",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```



### <a name="notifications-with-resource-data"></a><span data-ttu-id="42863-125">Notificações com dados de recursos</span><span class="sxs-lookup"><span data-stu-id="42863-125">Notifications with resource data</span></span>

<span data-ttu-id="42863-126">Para notificações com dados de recursos, a carga se parece com a seguinte.</span><span class="sxs-lookup"><span data-stu-id="42863-126">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="42863-127">Essa carga útil é para uma alteração de associação em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="42863-127">This payload is for a membership change in a team.</span></span>

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')",
        "resourceData": {
            "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
            "@odata.type": "#Microsoft.Graph.aadUserConversationMember",
            "@odata.id": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')"
        },
        "encryptedContent": {
            "data": "<<--EncryptedContent-->",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
    }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

<span data-ttu-id="42863-128">Para obter detalhes sobre como validar tokens e descriptografar a carga útil, consulte [Definir notificações de alteração que incluem dados de recursos](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="42863-128">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="42863-129">A carga de notificação descriptografada parece com a seguinte.</span><span class="sxs-lookup"><span data-stu-id="42863-129">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="42863-130">O conteúdo está em conformidade com o esquema [aaduserconversationmember](/graph/api/resources/aaduserconversationmember?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="42863-130">The payload conforms to the [aaduserconversationmember](/graph/api/resources/aaduserconversationmember?preserve-view=true) schema.</span></span> <span data-ttu-id="42863-131">A carga é semelhante à devolvida pelas operações GET.</span><span class="sxs-lookup"><span data-stu-id="42863-131">The payload is similar to that returned by GET operations.</span></span>

```json
{
  "id": "/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
  "roles": [
    "owner"
  ],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```

### <a name="notifications-without-resource-data"></a><span data-ttu-id="42863-132">Notificações sem dados de recursos</span><span class="sxs-lookup"><span data-stu-id="42863-132">Notifications without resource data</span></span>

<span data-ttu-id="42863-133">Notificações sem dados de recursos dão informações suficientes para fazer chamadas GET para obter o conteúdo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="42863-133">Notifications without resource data give you enough information to make GET calls to get the message content.</span></span> <span data-ttu-id="42863-134">As assinaturas para notificações sem dados de recursos não exigem um certificado de criptografia (porque os dados reais dos recursos não são enviados).</span><span class="sxs-lookup"><span data-stu-id="42863-134">Subscriptions for notifications without resource data don't require an encryption certificate (because actual resource data is not sent over).</span></span>

<span data-ttu-id="42863-135">Para notificações sem dados de recursos, a carga se parecerá com o seguinte.</span><span class="sxs-lookup"><span data-stu-id="42863-135">For notifications without resource data, the payload looks like the following.</span></span> <span data-ttu-id="42863-136">Essa carga útil é para uma alteração de associação em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="42863-136">This payload is for a membership change in a team.</span></span>

```json
{
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')",
  "resourceData": {
    "id": "ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk",
    "@odata.type": "#Microsoft.Graph.aadUserConversationMember",
    "@odata.id": "teams('ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062')/members('ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=')"
  }
}
```

<span data-ttu-id="42863-137">As propriedades **recurso** e **@odata.id** podem ser usados para fazer chamadas para o Microsoft Graph para obter o conteúdo para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="42863-137">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the message.</span></span> <span data-ttu-id="42863-138">As chamadas GET sempre retornarão o estado atual da mensagem.</span><span class="sxs-lookup"><span data-stu-id="42863-138">GET calls will always return the current state of the message.</span></span> <span data-ttu-id="42863-139">Se a mensagem for alterada entre quando a notificação for enviada e quando a mensagem for recuperada, a operação retornará a mensagem atualizada.</span><span class="sxs-lookup"><span data-stu-id="42863-139">If the message is changed between when the notification is sent and when the message is retrieved, the operation will return the updated message.</span></span>

## <a name="see-also"></a><span data-ttu-id="42863-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="42863-140">See also</span></span>
- [<span data-ttu-id="42863-141">Notificações de alteração do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="42863-141">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="42863-142">Visão geral da API do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="42863-142">Microsoft Teams API overview</span></span>](teams-concept-overview.md)