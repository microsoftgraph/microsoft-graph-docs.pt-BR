---
title: Configurar notificações de alteração que incluam dados de recurso
description: O Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. As notificações de alteração podem incluir propriedades de recursos.
author: davidmu1
ms.prod: non-product-specific
localization_priority: Priority
ms.openlocfilehash: 4da690a646c47ef857de860d36bde17a4ee26761
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547180"
---
# <a name="set-up-change-notifications-that-include-resource-data"></a><span data-ttu-id="0d46e-104">Configurar notificações de alteração que incluam dados de recurso</span><span class="sxs-lookup"><span data-stu-id="0d46e-104">Set up change notifications that include resource data</span></span>

<span data-ttu-id="0d46e-105">O Microsoft Graph permite que os aplicativos inscrevam-se para alterar as notificações de recursos através do [webhooks](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="0d46e-105">Microsoft Graph allows apps to subscribe to change notifications for resources via [webhooks](webhooks.md).</span></span> <span data-ttu-id="0d46e-106">É possíve configurar as assinaturas para incluir os dados alterados dos recursos (como o conteúdo de uma mensagem de bate-papo ou informações de presença do Microsoft Teams) nas notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="0d46e-106">You can set up subscriptions to include the changed resource data (such as the content of a Microsoft Teams chat message or Microsoft Teams presence information) in change notifications.</span></span> <span data-ttu-id="0d46e-107">Em seguida, seu aplicativo pode usar a lógica de negócios sem ter que fazer uma chamada à API separada para buscar o recurso alterado.</span><span class="sxs-lookup"><span data-stu-id="0d46e-107">Your app can then run its business logic without having to make a separate API call to fetch the changed resource.</span></span> <span data-ttu-id="0d46e-108">Como resultado, o aplicativo funciona melhor ao realizar menos chamadas da API, o que é benéfico em cenários de larga escala.</span><span class="sxs-lookup"><span data-stu-id="0d46e-108">As a result, the app performs better by making fewer API calls, which is beneficial in large scale scenarios.</span></span>

<span data-ttu-id="0d46e-109">A inclusão de dados de recursos como parte das notificações de alteração exige que, para atender aos requisitos de acesso e segurança de dados, você implemente a seguinte lógica adicional :</span><span class="sxs-lookup"><span data-stu-id="0d46e-109">Including resource data as part of change notifications requires you to implement the following additional logic to satisfy data access and security requirements:</span></span> 

- <span data-ttu-id="0d46e-110">[Lide com](webhooks-lifecycle.md#responding-to-reauthorizationrequired-notifications)) as notificações especiais sobre o ciclo de vida da assinatura (visualização) para manter um fluxo ininterrupto de dados.</span><span class="sxs-lookup"><span data-stu-id="0d46e-110">[Handle](webhooks-lifecycle.md#responding-to-reauthorizationrequired-notifications)) special subscription lifecycle notifications (preview) to maintain an uninterrupted flow of data.</span></span> <span data-ttu-id="0d46e-111">O Microsoft Graph envia notificações sobre o ciclo de vida de tempos em tempos para exigir que um aplicativo seja autorizado novamente e para garantir que os problemas de acesso não ocorram inesperadamente, incluindo dados de recursos nas notificações de alterações.</span><span class="sxs-lookup"><span data-stu-id="0d46e-111">Microsoft Graph sends lifecycle notifications from time to time to require an app to re-authorize, to make sure access issues have not unexpectedly cropped up for including resource data in change notifications.</span></span>
- <span data-ttu-id="0d46e-112">[Confirme](#validating-the-authenticity-of-notifications) a autenticidade das notificações de alteração como originárias do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0d46e-112">[Validate](#validating-the-authenticity-of-notifications) the authenticity of change notifications as having originated from Microsoft Graph.</span></span>
- <span data-ttu-id="0d46e-113">[Forneça](#decrypting-resource-data-from-change-notifications) uma chave de criptografia pública e utilize uma chave privada para decriptar os dados de recursos recebidos por meio das notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="0d46e-113">[Provide](#decrypting-resource-data-from-change-notifications) a public encryption key and use a private key to decrypt resource data received through change notifications.</span></span>

## <a name="resource-data-in-notification-payload"></a><span data-ttu-id="0d46e-114">Dados de recursos na carga de notificação </span><span class="sxs-lookup"><span data-stu-id="0d46e-114">Resource data in notification payload</span></span>

<span data-ttu-id="0d46e-115">Geralmente, esse tipo de notificação de alteração inclui os seguintes dados de recursos na carga:</span><span class="sxs-lookup"><span data-stu-id="0d46e-115">In general, this type of change notifications include the following resource data in the payload:</span></span>

- <span data-ttu-id="0d46e-116">ID e tipo de instância de recurso alterado, retornados na propriedade **resourceData**.</span><span class="sxs-lookup"><span data-stu-id="0d46e-116">ID and type of the changed resource instance, returned in the **resourceData** property.</span></span>
- <span data-ttu-id="0d46e-117">Todos os valores de propriedade da instância de recurso, criptografados conforme especificado na assinatura, retornados na propriedade **encryptedContent**.</span><span class="sxs-lookup"><span data-stu-id="0d46e-117">All the property values of that resource instance, encrypted as specified in the subscription, returned in the **encryptedContent** property.</span></span>
- <span data-ttu-id="0d46e-118">Or, dependendo do recurso, propriedades específicas retornadas na propriedade **resourceData**.</span><span class="sxs-lookup"><span data-stu-id="0d46e-118">Or, depending on the resource, specific properties returned in the **resourceData** property.</span></span> <span data-ttu-id="0d46e-119">Para obter somente propriedades específicas, especifique-as como parte da URL do **recurso** na assinatura, usando um parâmetro `$select`.</span><span class="sxs-lookup"><span data-stu-id="0d46e-119">To get only specific properties, specify them as part of the **resource** URL in the subscription, using a `$select` parameter.</span></span>  


## <a name="supported-resources"></a><span data-ttu-id="0d46e-120">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="0d46e-120">Supported resources</span></span>

<span data-ttu-id="0d46e-121">Atualmente, o Microsoft Teams [chatMessage](/graph/api/resources/chatmessage) assim como os recursos de [presença](/graph/api/resources/presence) (visualização) do Microsoft Teams oferecem suporte a notificações de alterações que incluem dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="0d46e-121">Currently, the Microsoft Teams [chatMessage](/graph/api/resources/chatmessage) as well as the Microsoft Teams [presence](/graph/api/resources/presence) (preview) resources supports change notifications that include resource data.</span></span> <span data-ttu-id="0d46e-122">Especificamente, você pode configurar uma assinatura que se aplique a uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="0d46e-122">Specifically, you can set up a subscription that applies to one of the following:</span></span>

- <span data-ttu-id="0d46e-123">Mensagens novas ou alteradas em um canal específico do Teams: `/teams/{id}/channels/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="0d46e-123">New or changed messages in a specific Teams channel: `/teams/{id}/channels/{id}/messages`</span></span>
- <span data-ttu-id="0d46e-124">Mensagens novas ou alteradas em todos os canais do Teams em toda a organização (locatário): `/teams/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="0d46e-124">New or changed messages in all Teams channels: `/teams/getAllMessages`</span></span>
- <span data-ttu-id="0d46e-125">Mensagens novas ou alteradas em um bate-papo específico do Teams: `/chats/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="0d46e-125">New or changed messages in a specific Teams chat: `/chats/{id}/messages`</span></span>
- <span data-ttu-id="0d46e-126">Mensagens novas ou alteradas em todos os bate-papos em toda a organização (locatário): `/chats/getAllMessages`</span><span class="sxs-lookup"><span data-stu-id="0d46e-126">New or changed messages in all Teams chats: `/chats/getAllMessages`</span></span>
- <span data-ttu-id="0d46e-127">Atualização das informações de presença do usuário: `/communications/presences/{id}`</span><span class="sxs-lookup"><span data-stu-id="0d46e-127">User's presence information update: `/communications/presences/{id}`</span></span>

<span data-ttu-id="0d46e-128">Os recursos **chatMessage** e **presence** (visualização) suportam, incluindo todas as propriedades de uma instância modificada em uma notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="0d46e-128">The **chatMessage** and the **presence** (preview) resources support including all the properties of a changed instance in a change notification.</span></span> <span data-ttu-id="0d46e-129">Eles não suportam o retorno de apenas propriedades seletivas da instância.</span><span class="sxs-lookup"><span data-stu-id="0d46e-129">They do not support returning only selective properties of the instance.</span></span> 

<span data-ttu-id="0d46e-130">Este artigo mostra um exemplo de assinatura para alterar as notificações de mensagens em um canal do Teams, com cada notificação de alteração incluindo todos os dados do recurso da instância **chatMessage** alterada.</span><span class="sxs-lookup"><span data-stu-id="0d46e-130">This article walks through an example that shows you how to subscribe to change notifications for messages in a Teams channel, with each change notification including the full resource data of the changed **chatMessage** instance.</span></span> <span data-ttu-id="0d46e-131">Para obter mais detalhes sobre assinaturas baseadas em **chatMessage**, confira [Obter notificações de alteração para mensagens de chat e canal](teams-changenotifications-chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="0d46e-131">For more details about **chatMessage**-based subscriptions, see [Get change notifications for chat and channel messages](teams-changenotifications-chatmessage.md).</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="0d46e-132">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="0d46e-132">Creating a subscription</span></span>

<span data-ttu-id="0d46e-133">Para que os dados de recursos estejam incluídos nas notificações de alteração, você **deve** especificar as seguintes propriedades, além das que geralmente são especificadas ao [criar uma assinatura](webhooks.md#creating-a-subscription):</span><span class="sxs-lookup"><span data-stu-id="0d46e-133">To have resource data included in change notifications, you **must** specify the following properties, in addition to those that are usually specified when [creating a subscription](webhooks.md#creating-a-subscription):</span></span>

- <span data-ttu-id="0d46e-134">**includeResourceData** que deve ser definido como `true` para solicitar explicitamente os dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="0d46e-134">**includeResourceData** which should be set to `true` to explicitly request resource data.</span></span>
- <span data-ttu-id="0d46e-135">**encryptionCertificate** que contém apenas a chave público que o Microsoft Graph usa para criptografar os dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="0d46e-135">**encryptionCertificate** which contains only the public key that Microsoft Graph uses to encrypt resource data.</span></span> <span data-ttu-id="0d46e-136">Mantenha a chave privada correspondente para [descriptografar o conteúdo](#decrypting-resource-data-from-change-notifications).</span><span class="sxs-lookup"><span data-stu-id="0d46e-136">Keep the corresponding private key to [decrypt the content](#decrypting-resource-data-from-change-notifications).</span></span>
- <span data-ttu-id="0d46e-137">**encryptionCertificateId** é o seu próprio identificador para o certificado.</span><span class="sxs-lookup"><span data-stu-id="0d46e-137">**encryptionCertificateId** which is your own identifier for the certificate.</span></span> <span data-ttu-id="0d46e-138">Use esse ID para corresponder a cada notificação de alteração cujo certificado foi utilizado para descriptografia.</span><span class="sxs-lookup"><span data-stu-id="0d46e-138">Use this ID to match in each change notification, which certificate to use for decryption.</span></span>

<span data-ttu-id="0d46e-139">Lembre-se do seguinte:</span><span class="sxs-lookup"><span data-stu-id="0d46e-139">Keep the following in mind:</span></span>

- <span data-ttu-id="0d46e-140">Valide ambos os pontos de extremidade conforme descrito em [Validação de ponto de extremidade de notificação](webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="0d46e-140">Validate both endpoints as described in [Notification endpoint validation](webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="0d46e-141">Se você quiser usar a mesma URL para os dois pontos de extremidade, você receberá e responderá a duas solicitações de validação.</span><span class="sxs-lookup"><span data-stu-id="0d46e-141">If you choose to use the same URL for both endpoints, you will receive and respond to two validation requests.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="0d46e-142">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="0d46e-142">Subscription request example</span></span>

<span data-ttu-id="0d46e-143">O exemplo a seguir assina as mensagens de canal que estão sendo criadas ou atualizadas no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0d46e-143">The following example subscribes to channel messages being created or updated in Microsoft Teams.</span></span>

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="subscription-response"></a><span data-ttu-id="0d46e-144">Resposta de assinatura</span><span class="sxs-lookup"><span data-stu-id="0d46e-144">Subscription response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificateId": "{custom ID}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secret client state}"
}
```

## <a name="subscription-lifecycle-notifications-preview"></a><span data-ttu-id="0d46e-145">Notificações do ciclo de vida da assinatura (visualização)</span><span class="sxs-lookup"><span data-stu-id="0d46e-145">Subscription lifecycle notifications (preview)</span></span>

<span data-ttu-id="0d46e-146">Certos eventos podem interferir no fluxo de notificação de alterações em uma assinatura existente.</span><span class="sxs-lookup"><span data-stu-id="0d46e-146">Certain events can interfere with change notification flow in an existing subscription.</span></span> <span data-ttu-id="0d46e-147">As notificações sobre o ciclo de vida da assinatura informam as ações a serem tomadas para manter um fluxo ininterrupto.</span><span class="sxs-lookup"><span data-stu-id="0d46e-147">Subscription lifecycle notifications inform you actions to take in order to maintain an uninterrupted flow.</span></span> <span data-ttu-id="0d46e-148">Ao contrário de uma notificação de alteração de recurso que informa uma alteração em uma instância de recurso, uma notificação do ciclo de vida é sobre a própria assinatura e seu estado atual no ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="0d46e-148">Unlike a resource change notification which informs a change to a resource instance, a lifecycle notification is about the subscription itself, and its current state in the lifecycle.</span></span> 

<span data-ttu-id="0d46e-149">Para obter mais informações sobre como receber e responder a, notificações de ciclo de vida (visualização), confira [Reduzir assinaturas ausentes e alterar as notificações (visualização)](webhooks-lifecycle.md)</span><span class="sxs-lookup"><span data-stu-id="0d46e-149">For more information about how to receive, and respond to, lifecycle notifications (preview), see [Reduce missing subscriptions and change notifications (preview)](webhooks-lifecycle.md)</span></span>

## <a name="validating-the-authenticity-of-notifications"></a><span data-ttu-id="0d46e-150">Validando a autenticidade das notificações</span><span class="sxs-lookup"><span data-stu-id="0d46e-150">Validating the authenticity of notifications</span></span>

<span data-ttu-id="0d46e-151">Os aplicativos geralmente executam a lógica comercial com base nos dados de recursos incluídos nas notificações de alterações.</span><span class="sxs-lookup"><span data-stu-id="0d46e-151">Apps often run business logic based on resource data included in change notifications.</span></span> <span data-ttu-id="0d46e-152">Verificar a autenticidade de cada notificação de alteração primeiro é importante.</span><span class="sxs-lookup"><span data-stu-id="0d46e-152">Verifying the authenticity of each change notification first is important.</span></span> <span data-ttu-id="0d46e-153">Caso contrário, um terceiro poderá imitar seu aplicativo com notificações de alteração falsa e fazê-lo executar a lógica de negócios incorretamente, e isso pode levar a um incidente de segurança.</span><span class="sxs-lookup"><span data-stu-id="0d46e-153">Otherwise, a third party can spoof your app with false change notifications and make it run its business logic incorrectly, and this can lead to a security incident.</span></span>

<span data-ttu-id="0d46e-154">Para notificações básicas de alterações que não contêm dados de recursos, simplesmente valide-as com base no valor **clientState** conforme descrito em [Processando a notificação de alteração](webhooks.md#processing-the-change-notification).</span><span class="sxs-lookup"><span data-stu-id="0d46e-154">For basic change notifications that do not contain resource data, simply validate them based on the **clientState** value as described in [Processing the change notification](webhooks.md#processing-the-change-notification).</span></span> <span data-ttu-id="0d46e-155">Isso é aceitável, uma vez que você pode fazer chamadas confiáveis subsequentes do Microsoft Graph para obter acesso ao dados do recurso, portanto, o impacto das tentativas de falsificação é limitado.</span><span class="sxs-lookup"><span data-stu-id="0d46e-155">This is acceptable, as you can make subsequent trusted Microsoft Graph calls to get access to resource data, and therefore the impact of any spoofing attempts is limited.</span></span> 

<span data-ttu-id="0d46e-156">Para notificações de alteração que entregam dados de recursos, execute uma validação mais completa antes de processar os dados.</span><span class="sxs-lookup"><span data-stu-id="0d46e-156">For change notifications that deliver resource data, perform a more thorough validation before processing the data.</span></span>

<span data-ttu-id="0d46e-157">Nesta seção:</span><span class="sxs-lookup"><span data-stu-id="0d46e-157">In this section:</span></span>

- [<span data-ttu-id="0d46e-158">Tokens de validação na notificação de alteração</span><span class="sxs-lookup"><span data-stu-id="0d46e-158">Validation tokens in the change notification</span></span>](#validation-tokens-in-the-change-notification)
- [<span data-ttu-id="0d46e-159">Como validar</span><span class="sxs-lookup"><span data-stu-id="0d46e-159">How to validate</span></span>](#how-to-validate)
- [<span data-ttu-id="0d46e-160">Exemplo de token JWT</span><span class="sxs-lookup"><span data-stu-id="0d46e-160">Example JWT token</span></span>](#example-jwt-token)

### <a name="validation-tokens-in-the-change-notification"></a><span data-ttu-id="0d46e-161">Tokens de validação na notificação de alteração</span><span class="sxs-lookup"><span data-stu-id="0d46e-161">Validation tokens in the change notification</span></span>

<span data-ttu-id="0d46e-162">Uma notificação de alteração com os dados do recurso contém uma propriedade adicional, **validationTokens**, com uma matriz de tokens JWT gerados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0d46e-162">A change notification with resource data contains an additional property, **validationTokens**, which contains an array of JWT tokens generated by Microsoft Graph.</span></span> <span data-ttu-id="0d46e-163">O Microsoft Graph gera um token único para cada aplicativo distinto e um par de locatários onde existe um item no conunto **valor**.</span><span class="sxs-lookup"><span data-stu-id="0d46e-163">Microsoft Graph generates a single token for each distinct app and tenant pair for whom there is an item in the **value** array.</span></span> <span data-ttu-id="0d46e-164">Tenha em mente que as notificações de alterações podem conter uma mistura de itens para vários aplicativos e locatários que fizeram assinatura usando o mesmo **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="0d46e-164">Keep in mind that change notifications may contain a mix of items for various apps and tenants that subscribed using the same **notificationUrl**.</span></span>

<span data-ttu-id="0d46e-165">No exemplo a seguir, a notificação de alteração contém dois itens para o mesmo aplicativo e para dois locatários diferentes, portanto, o conjunto **validationTokens** contém dois tokens que precisam ser validados.</span><span class="sxs-lookup"><span data-stu-id="0d46e-165">In the following example, the change notification contains two items for the same app, and for two different tenants, therefore the **validationTokens** array contains two tokens that need to be validated.</span></span>

```json
{
    "value": [
          {
            "subscriptionId": "76619225-ff6b-4489-96ca-4ef547e78b22",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
            "changeType": "created",
            ...
          },
      {
            "subscriptionId": "e990d58f-fd93-40af-acf7-a7c907c5d8ea",
      "tenantId": "46d9e3bd-6309-4177-a016-b256a411e30f",
            "changeType": "created",
            ...
            }
    ],
    "validationTokens": [
        "eyJ0eXAiOiJKV1QiLCJhb...",
    "cGlkYWNyIjoiMiIsImlkc..."
    ]
}
```

> <span data-ttu-id="0d46e-166">**Nota:** para obter uma descrição completa dos dados enviados quando as notificações de alterações são entregues, consulte [ changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="0d46e-166">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="how-to-validate"></a><span data-ttu-id="0d46e-167">Como validar</span><span class="sxs-lookup"><span data-stu-id="0d46e-167">How to validate</span></span>

<span data-ttu-id="0d46e-168">Se você não conhece a validação de token, consulte [Princípios de Validação de Token](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) para obter uma visão geral.</span><span class="sxs-lookup"><span data-stu-id="0d46e-168">If you're new to token validation, see [Principles of Token Validation](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) for an overview.</span></span> <span data-ttu-id="0d46e-169">Use um SDK, como a [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) biblioteca para .NET ou uma biblioteca de terceiros para uma plataforma diferente.</span><span class="sxs-lookup"><span data-stu-id="0d46e-169">Use an SDK, such as the [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) library for .NET, or a third-party library for a different platform.</span></span>

<span data-ttu-id="0d46e-170">Fique atento ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="0d46e-170">Be mindful of the following:</span></span> 

- <span data-ttu-id="0d46e-171">Certifique-se de sempre enviar um `HTTP 202 Accepted` código de status como parte da resposta à notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="0d46e-171">Make sure to always send an `HTTP 202 Accepted` status code as part of the response to the change notification.</span></span> 
- <span data-ttu-id="0d46e-172">Responda antes de validar a notificação de alteração (por exemplo, se você armazenar as notificações de alteração em filas para processamento posterior) ou depois (se você as processar instantaneamente), mesmo se a validação falhar.</span><span class="sxs-lookup"><span data-stu-id="0d46e-172">Respond before validating the change notification (for example, if you store change notifications in queues for later processing) or after (if you process them on the fly), even if validation failed.</span></span>
- <span data-ttu-id="0d46e-173">A aceitação de uma notificação de alteração evita novas tentativas desnecessárias de entrega e também impede que possíveis atores invasores descubram se foram ou não aprovados na validação.</span><span class="sxs-lookup"><span data-stu-id="0d46e-173">Accepting a change notification prevents unnecessary delivery retries and it also prevents any potential rogue actors from finding out if they passed or failed validation.</span></span> <span data-ttu-id="0d46e-174">Você sempre pode optar por ignorar uma notificação de alteração inválida após aceitá-la.</span><span class="sxs-lookup"><span data-stu-id="0d46e-174">You can always choose to ignore an invalid change notification after you have accepted it.</span></span>

<span data-ttu-id="0d46e-175">Especificamente, realize a validação em todos os tokens JWT na coleção **validationTokens**.</span><span class="sxs-lookup"><span data-stu-id="0d46e-175">In particular, perform validation on every JWT token in the **validationTokens** collection.</span></span> <span data-ttu-id="0d46e-176">Se algum token falhar, considere a notificação de alteração suspeita e investigue mais.</span><span class="sxs-lookup"><span data-stu-id="0d46e-176">If any tokens fail, consider the change notification suspicious and investigate further.</span></span> 

<span data-ttu-id="0d46e-177">Use as etapas a seguir para validar tokens e aplicativos que geram tokens:</span><span class="sxs-lookup"><span data-stu-id="0d46e-177">Use the following steps to validate tokens and apps that generate tokens:</span></span>

1. <span data-ttu-id="0d46e-178">Valide se o token não expirou.</span><span class="sxs-lookup"><span data-stu-id="0d46e-178">Validate that the token has not expired.</span></span>

2. <span data-ttu-id="0d46e-179">Valide se o token não foi adulterado e foi emitido pela autoridade esperada, plataforma de identidade da Microsoft:</span><span class="sxs-lookup"><span data-stu-id="0d46e-179">Validate the token has not been tampered with and was issued by the expected authority, Microsoft identity platform:</span></span>

    - <span data-ttu-id="0d46e-180">Obtenha as chaves de assinatura do ponto de extremidade de configuração comum: `https://login.microsoftonline.com/common/.well-known/openid-configuration`.</span><span class="sxs-lookup"><span data-stu-id="0d46e-180">Obtain the signing keys from the common configuration endpoint: `https://login.microsoftonline.com/common/.well-known/openid-configuration`.</span></span> <span data-ttu-id="0d46e-181">Essa configuração é armazenada em cache pelo aplicativo por um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="0d46e-181">This configuration is cached by your app for a period of time.</span></span> <span data-ttu-id="0d46e-182">Lembre-se de que a configuração é atualizada frequentemente, uma vez que as chaves de assinatura são giradas diariamente.</span><span class="sxs-lookup"><span data-stu-id="0d46e-182">Be aware that the configuration is updated frequently as signing keys are rotated daily.</span></span>
    - <span data-ttu-id="0d46e-183">Verifique a assinatura do token JWT usando essas chaves.</span><span class="sxs-lookup"><span data-stu-id="0d46e-183">Verify the signature of the JWT token using those keys.</span></span>

    <span data-ttu-id="0d46e-184">Não aceite tokens emitidos por outra autoridade.</span><span class="sxs-lookup"><span data-stu-id="0d46e-184">Do not accept tokens issued by any other authority.</span></span>

3. <span data-ttu-id="0d46e-185">Valide se o token foi emitido para o aplicativo que está inscrito para alterar as notificações.</span><span class="sxs-lookup"><span data-stu-id="0d46e-185">Validate that the token was issued for your app that is subscribing to change notifications.</span></span>

    <span data-ttu-id="0d46e-186">As etapas a seguir fazem parte da lógica de validação padrão nas bibliotecas de token JWT e podem ser tipicamente executadas como uma única chamada de função.</span><span class="sxs-lookup"><span data-stu-id="0d46e-186">The following steps are part of standard validation logic in JWT token libraries and can typically be executed as a single function call.</span></span> 
    - <span data-ttu-id="0d46e-187">Valide a “audiência” no token que corresponde à ID do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0d46e-187">Validate the "audience" in the token matches your app ID.</span></span>
    - <span data-ttu-id="0d46e-188">Se você tiver mais de um aplicativo recebendo notificações de alterações, verifique a existencia de vários IDs.</span><span class="sxs-lookup"><span data-stu-id="0d46e-188">If you have more than one app receiving change notifications, make sure to check for multiple IDs.</span></span>


4. <span data-ttu-id="0d46e-189">**Crítico**: valide se o aplicativo que gerou o token representa o distribuidor de notificação de alteração do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0d46e-189">**Critical**: Validate that the app that generated the token represents the Microsoft Graph change notification publisher.</span></span> 

    - <span data-ttu-id="0d46e-190">Verifique se a propriedade **appid** no token corresponde ao valor esperado de `0bf30f3b-4a52-48df-9a82-234910c4a086`.</span><span class="sxs-lookup"><span data-stu-id="0d46e-190">Check that the **appid** property in the token matches the expected value of `0bf30f3b-4a52-48df-9a82-234910c4a086`.</span></span>
    - <span data-ttu-id="0d46e-191">Isso garante que as notificações de alteração não sejam enviadas por um aplicativo diferente do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0d46e-191">This ensures that change notifications are not sent by a different app that is not Microsoft Graph.</span></span>


### <a name="example-jwt-token"></a><span data-ttu-id="0d46e-192">Exemplo de Token JWT </span><span class="sxs-lookup"><span data-stu-id="0d46e-192">Example JWT token</span></span>

<span data-ttu-id="0d46e-193">A seguir, é apresentado um exemplo das propriedades incluídas no token JWT que são necessárias para validação.</span><span class="sxs-lookup"><span data-stu-id="0d46e-193">The following is an example of the properties included in the JWT token that are needed for validation.</span></span>

```json
{
  // aud is your app's id 
  "aud": "8e460676-ae3f-4b1e-8790-ee0fb5d6148f",                           
  "iss": "https://sts.windows.net/84bd8158-6d4d-4958-8b9f-9d6445542f95/",
  "iat": 1565046813,
  "nbf": 1565046813,
  // Expiration date 
  "exp": 1565075913,                                                        
  "aio": "42FgYKhZ+uOZrHa7p+7tfruauq1HAA==",
  // appid represents the notification publisher and must always be the same value of 0bf30f3b-4a52-48df-9a82-234910c4a086 
  "appid": "0bf30f3b-4a52-48df-9a82-234910c4a086",                          
  "appidacr": "2",
  "idp": "https://sts.windows.net/84bd8158-6d4d-4958-8b9f-9d6445542f95/",
  "tid": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
  "uti": "-KoJHevhgEGnN4kwuixpAA",
  "ver": "1.0"
}
```

### <a name="example-verifying-validation-tokens"></a><span data-ttu-id="0d46e-194">Exemplo: verificação de tokens de validação</span><span class="sxs-lookup"><span data-stu-id="0d46e-194">Example: Verifying validation tokens</span></span>

```csharp
// add Microsoft.IdentityModel.Protocols.OpenIdConnect and System.IdentityModel.Tokens.Jwt nuget packages to your project
public async Task<bool> ValidateToken(string token, string tenantId, IEnumerable<string> appIds)
{
    var configurationManager = new ConfigurationManager<OpenIdConnectConfiguration>("https://login.microsoftonline.com/common/v2.0/.well-known/openid-configuration", new OpenIdConnectConfigurationRetriever());
    var openIdConfig = await configurationManager.GetConfigurationAsync();
    var handler = new JwtSecurityTokenHandler();
    try
    {
    handler.ValidateToken(token, new TokenValidationParameters
    {
        ValidateIssuer = true,
        ValidateAudience = true,
        ValidateIssuerSigningKey = true,
        ValidateLifetime = true,
        ValidIssuer = $"https://sts.windows.net/{tenantId}/",
        ValidAudiences = appIds,
        IssuerSigningKeys = openIdConfig.SigningKeys
    }, out _);
    return true;
    }
    catch (Exception ex)
    {
    Trace.TraceError($"{ex.Message}:{ex.StackTrace}");
    return false;
    }
}
```
```java
private boolean IsValidationTokenValid(String[] appIds, String tenantId, String serializedToken) {
    try {
        JwkKeyResolver jwksResolver = new JwkKeyResolver();
        Jws<Claims> token = Jwts.parserBuilder()
        .setSigningKeyResolver(jwksResolver)
        .build()
        .parseClaimsJws(serializedToken);
        Claims body = token.getBody();
        String audience = body.getAudience();
        boolean isAudienceValid = false;
        for(String appId : appIds) {
        isAudienceValid = isAudienceValid || appId.equals(audience);
        }
        boolean isTenantValid = body.getIssuer().endsWith(tenantId + "/");
        return isAudienceValid  && isTenantValid; //nbf,exp and signature are already validated by library
    } catch (Exception e) {
        LOGGER.error("could not validate token");
        LOGGER.error(e.getMessage());
        return false;
    }
}
```
```JavaScript
import jwt from 'jsonwebtoken';
import jkwsClient from 'jwks-rsa';

const client = jkwsClient({
  jwksUri: 'https://login.microsoftonline.com/common/discovery/v2.0/keys'
});

export function getKey(header, callback) {
  client.getSigningKey(header.kid, (err, key) => {
    var signingKey = key.publicKey || key.rsaPublicKey;
    callback(null, signingKey);
  });
}

export function isTokenValid(token, appId, tenantId) {
  return new Promise((resolve) => {
    const options = {
      audience: [appId],
      issuer: [`https://sts.windows.net/${tenantId}/`]
    };
    jwt.verify(token, getKey, options, (err) => {
      if (err) {
        // eslint-disable-next-line no-console
        console.error(err);
        resolve(false);
      } else {
        resolve(true);
      }
    });
  });
}
```
<span data-ttu-id="0d46e-195">Para que o exemplo do Java funcione, também será necessário implementar o `JwkKeyResolver`.</span><span class="sxs-lookup"><span data-stu-id="0d46e-195">For the Java sample to work, you will also need to implement the `JwkKeyResolver`.</span></span>  
```java
package com.example.restservice;

import com.auth0.jwk.JwkProvider;
import com.auth0.jwk.UrlJwkProvider;
import com.auth0.jwk.Jwk;
import io.jsonwebtoken.Claims;
import io.jsonwebtoken.JwsHeader;
import io.jsonwebtoken.SigningKeyResolverAdapter;
import java.security.Key;
import java.net.URI;
import org.slf4j.Logger;
import org.slf4j.LoggerFactory;

public class JwkKeyResolver extends SigningKeyResolverAdapter {
    private JwkProvider keyStore;
    private final Logger LOGGER = LoggerFactory.getLogger(this.getClass());
    public JwkKeyResolver() throws java.net.URISyntaxException, java.net.MalformedURLException {
        this.keyStore = new UrlJwkProvider((new URI("https://login.microsoftonline.com/common/discovery/keys").toURL()));
    }
    @Override
    public Key resolveSigningKey(JwsHeader jwsHeader, Claims claims) {
        try {
            String keyId = jwsHeader.getKeyId();
            Jwk pub = keyStore.get(keyId);
            return pub.getPublicKey();
        } catch (Exception e) {
            LOGGER.error(e.getMessage());
            return null;
        }
    }
}
```

## <a name="decrypting-resource-data-from-change-notifications"></a><span data-ttu-id="0d46e-196">Descriptografar os dados de recursos de notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="0d46e-196">Decrypting resource data from change notifications</span></span>

<span data-ttu-id="0d46e-197">A propriedade **resourceData** de uma notificação de alteração inclui apenas o ID básico e as informações do tipo de uma instância de recurso.</span><span class="sxs-lookup"><span data-stu-id="0d46e-197">The **resourceData** property of a change notification includes only the basic ID and type information of a resource instance.</span></span> <span data-ttu-id="0d46e-198">A propriedade **encryptedData** contém os dados de recursos completos, criptografados pelo Microsoft Graph usando a chave pública fornecida na assinatura.</span><span class="sxs-lookup"><span data-stu-id="0d46e-198">The **encryptedData** property contains the full resource data, encrypted by Microsoft Graph using the public key provided in the subscription.</span></span> <span data-ttu-id="0d46e-199">A propriedade também contém valores necessários para verificação e descriptografia.</span><span class="sxs-lookup"><span data-stu-id="0d46e-199">The property also contains values required for verification and decryption.</span></span> <span data-ttu-id="0d46e-200">Isso é feito para aumentar a segurança dos dados do cliente acessados por meio de notificações de alterações.</span><span class="sxs-lookup"><span data-stu-id="0d46e-200">This is done to increase the security of customer data accessed via change notifications.</span></span> <span data-ttu-id="0d46e-201">É da sua responsabilidade proteger a chave privada para garantir que os dados do cliente não sejam decriptados por terceiros, mesmo que eles consigam interceptar as notificações de alteração originais.</span><span class="sxs-lookup"><span data-stu-id="0d46e-201">It is your responsibility to secure the private key to ensure that customer data cannot be decrypted by a third party, even if they manage to intercept the original change notifications.</span></span>

<span data-ttu-id="0d46e-202">Nesta seção:</span><span class="sxs-lookup"><span data-stu-id="0d46e-202">In this section:</span></span>

- [<span data-ttu-id="0d46e-203">Gerenciar as chaves de criptografia</span><span class="sxs-lookup"><span data-stu-id="0d46e-203">Managing encryption keys</span></span>](#managing-encryption-keys)
- [<span data-ttu-id="0d46e-204">Descriptografar os dados de recursos</span><span class="sxs-lookup"><span data-stu-id="0d46e-204">Decrypting resource data</span></span>](#decrypting-resource-data)
- [<span data-ttu-id="0d46e-205">Exemplo: descriptografar uma notificação com dados de recursos criptografados</span><span class="sxs-lookup"><span data-stu-id="0d46e-205">Example: decrypting a notification with encrypted resource data</span></span>](#example-decrypting-a-notification-with-encrypted-resource-data)

### <a name="managing-encryption-keys"></a><span data-ttu-id="0d46e-206">Gerenciar as chaves de criptografia</span><span class="sxs-lookup"><span data-stu-id="0d46e-206">Managing encryption keys</span></span>

1. <span data-ttu-id="0d46e-207">Obtenha um certificado com um par de chaves assimétricas.</span><span class="sxs-lookup"><span data-stu-id="0d46e-207">Obtain a certificate with a pair of asymmetric keys.</span></span>

    - <span data-ttu-id="0d46e-208">Você pode assinatura o certificado sozinho, uma vez que o Microsoft Graph não verifica o emissor do certificado e usa a chave pública somente para criptografia.</span><span class="sxs-lookup"><span data-stu-id="0d46e-208">You can self-sign the certificate, since Microsoft Graph does not verify the certificate issuer, and uses the public key for only encryption.</span></span> 
    - <span data-ttu-id="0d46e-209">Use o [Cofre da Chave do Azure](/azure/key-vault/key-vault-whatis) como a solução para criar, girar e gerenciar certificados com segurança.</span><span class="sxs-lookup"><span data-stu-id="0d46e-209">Use [Azure Key Vault](/azure/key-vault/key-vault-whatis) as the solution to create, rotate, and securely manage certificates.</span></span> <span data-ttu-id="0d46e-210">Cerifique-se de que as chaves atendem aos seguintes critérios:</span><span class="sxs-lookup"><span data-stu-id="0d46e-210">Make sure the keys satisfy the following criteria:</span></span>

        - <span data-ttu-id="0d46e-211">A chave deve ser do tipo `RSA`</span><span class="sxs-lookup"><span data-stu-id="0d46e-211">The key must be of type `RSA`</span></span>
        - <span data-ttu-id="0d46e-212">O tamanho da chave deve estar entre 2048 e 4096 bits</span><span class="sxs-lookup"><span data-stu-id="0d46e-212">The key size must be between 2048 and 4096 bits</span></span>

2. <span data-ttu-id="0d46e-213">Exportar o certificar no formato base64-encoded X.509 e **incluir apenas a chave pública**.</span><span class="sxs-lookup"><span data-stu-id="0d46e-213">Export the certificate in base64-encoded X.509 format, and **include only the public key**.</span></span> 

3. <span data-ttu-id="0d46e-214">Ao criar uma assinatura:</span><span class="sxs-lookup"><span data-stu-id="0d46e-214">When creating a subscription:</span></span>

    - <span data-ttu-id="0d46e-215">Forneça o certificado na propriedade **encryptionCertificate** usando o conteúdo base64-encoded no qual o certificado foi exportado.</span><span class="sxs-lookup"><span data-stu-id="0d46e-215">Provide the certificate in the **encryptionCertificate** property, using the base64-encoded content that the certificate was exported in.</span></span>
    - <span data-ttu-id="0d46e-216">Forneça seu próprio identificador na propriedade **encryptionCertificateId**.</span><span class="sxs-lookup"><span data-stu-id="0d46e-216">Provide your own identifier in the **encryptionCertificateId** property.</span></span> 
  
        <span data-ttu-id="0d46e-p121">Esse identificador permite corresponder seus certificados às notificações de alterações recebidas e recuperar certificados do seu repositório de certificados. O identificador pode ter até 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="0d46e-p121">This identifier allows you to match your certificates to the change notifications you receive, and to retrieve certificates from your certificate store. The identifier can be up to 128 characters.</span></span>

4. <span data-ttu-id="0d46e-219">Gerencie com segurança a chave privada com para que seu código de processamento de notificação de alteração acesse a chave privada para decriptar os dados do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d46e-219">Manage the private key securely, so that your change notification processing code can access the private key to decrypt resource data.</span></span>

#### <a name="rotating-keys"></a><span data-ttu-id="0d46e-220">Chaves de rotação</span><span class="sxs-lookup"><span data-stu-id="0d46e-220">Rotating keys</span></span>

<span data-ttu-id="0d46e-221">Para minimizar o risco de uma chave privada ser comprometida, altere periodicamente suas chaves assimétricas.</span><span class="sxs-lookup"><span data-stu-id="0d46e-221">To minimize the risk of a private key becoming compromised, periodically change your asymmetric keys.</span></span> <span data-ttu-id="0d46e-222">Siga estas etapas para introduzir um novo par de chaves:</span><span class="sxs-lookup"><span data-stu-id="0d46e-222">Follow these steps to introduce a new pair of keys:</span></span>

1. <span data-ttu-id="0d46e-223">Obtenha um novo certificado com um novo par de chaves assimétricas.</span><span class="sxs-lookup"><span data-stu-id="0d46e-223">Obtain a new certificate with a new pair of asymmetric keys.</span></span> <span data-ttu-id="0d46e-224">Use-o para todas as novas assinaturas sendo criadas.</span><span class="sxs-lookup"><span data-stu-id="0d46e-224">Use it for all new subscriptions being created.</span></span>

2. <span data-ttu-id="0d46e-225">Atualize as assinaturas existentes com a nova chave de certificado.</span><span class="sxs-lookup"><span data-stu-id="0d46e-225">Update existing subscriptions with the new certificate key.</span></span>

    - <span data-ttu-id="0d46e-226">Faça isso como parte da renovação da assinatura regular.</span><span class="sxs-lookup"><span data-stu-id="0d46e-226">Do this as part of regular subscription renewal.</span></span> 
    - <span data-ttu-id="0d46e-227">Ou enumere todas as assinaturas e forneça a chave.</span><span class="sxs-lookup"><span data-stu-id="0d46e-227">Or, enumerate all subscriptions and provide the key.</span></span> <span data-ttu-id="0d46e-228">Use a [operação PATCH na assinatura](/graph/api/subscription-update) e atualize as propriedades **encryptionCertificate** e **encryptionCertificateId**.</span><span class="sxs-lookup"><span data-stu-id="0d46e-228">Use the [PATCH operation on the subscription](/graph/api/subscription-update) and update the **encryptionCertificate** and **encryptionCertificateId** properties.</span></span>

3. <span data-ttu-id="0d46e-229">Lembre-se do seguinte:</span><span class="sxs-lookup"><span data-stu-id="0d46e-229">Keep in mind the following:</span></span>
    - <span data-ttu-id="0d46e-230">Por um período de tempo, o certificado antigo ainda pode ser usado para criptografia.</span><span class="sxs-lookup"><span data-stu-id="0d46e-230">For a period of time, the old certificate may still be used for encryption.</span></span> <span data-ttu-id="0d46e-231">Seu aplicativo deve ter acesso a certificados novos e antigos para poder descriptografar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0d46e-231">Your app must have access to both old and new certificates to be able to decrypt content.</span></span>
    - <span data-ttu-id="0d46e-232">Use a propriedade **encryptionCertificateId** em cada notificação de alteração para identificar a chave correta a ser utilizada.</span><span class="sxs-lookup"><span data-stu-id="0d46e-232">Use the **encryptionCertificateId** property in each change notification to identify the correct key to use.</span></span>
    - <span data-ttu-id="0d46e-233">Descarte o certificado antigo somente quando não houver notificações de alterações recentes fazendo referência a ele.</span><span class="sxs-lookup"><span data-stu-id="0d46e-233">Discard of the old certificate only when you have seen no recent change notifications referencing it.</span></span>

### <a name="decrypting-resource-data"></a><span data-ttu-id="0d46e-234">Descriptografar dados de recursos</span><span class="sxs-lookup"><span data-stu-id="0d46e-234">Decrypting resource data</span></span>

<span data-ttu-id="0d46e-235">Para otimizar o desempenho, o Microsoft Graph usa um processo de criptografia de duas etapas:</span><span class="sxs-lookup"><span data-stu-id="0d46e-235">To optimize performance, Microsoft Graph uses a two-step encryption process:</span></span>
  - <span data-ttu-id="0d46e-236">Ele gera uma chave simétrica de uso único e a usa para criptografar os dados do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d46e-236">It generates a single use symmetric key, and uses it to encrypt resource data.</span></span>
  - <span data-ttu-id="0d46e-237">Ele usa a chave pública assimétrica (que você forneceu ao fazer a assinatura) para criptografar a chave simétrica e a incluir em cada notificação de alteração desta assinatura.</span><span class="sxs-lookup"><span data-stu-id="0d46e-237">It uses the public asymmetric key (that you provided when subscribing) to encrypt the symmetric key and includes it in each change notification of that subscription.</span></span>

<span data-ttu-id="0d46e-238">Sempre assuma que a chave simétrica é diferente para cada item na notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="0d46e-238">Always assume that the symmetric key is different for each item in the change notification.</span></span>

<span data-ttu-id="0d46e-239">Para decriptar os dados de recursos, o seu aplicativo deve executar as etapas inversas, usando as propriedades **encryptedContent** em cada notificação de alteração:</span><span class="sxs-lookup"><span data-stu-id="0d46e-239">To decrypt resource data, your app should perform the reverse steps, using the properties under **encryptedContent** in each change notification:</span></span>

1. <span data-ttu-id="0d46e-240">Use a propriedade **encryptionCertificateId** para identificar o certificado a ser usado.</span><span class="sxs-lookup"><span data-stu-id="0d46e-240">Use the **encryptionCertificateId** property to identify the certificate to use.</span></span>

2. <span data-ttu-id="0d46e-241">Inicialize um componente criptográfico da RSA (como o .NET [RSACryptoServiceProvider](/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) com a chave privada.</span><span class="sxs-lookup"><span data-stu-id="0d46e-241">Initialize an RSA cryptographic component (such as the .NET [RSACryptoServiceProvider](/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) with the private key.</span></span>

3. <span data-ttu-id="0d46e-242">Decripte a chave simétrica entregue na propriedade **dataKey** de cada item na notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="0d46e-242">Decrypt the symmetric key delivered in the **dataKey** property of each item in the change notification.</span></span>

    <span data-ttu-id="0d46e-243">Use o Preenchimento de Criptografia Assimétrica Ideal (OAEP) para o algoritmo de descriptografia.</span><span class="sxs-lookup"><span data-stu-id="0d46e-243">Use Optimal Asymmetric Encryption Padding (OAEP) for the decryption algorithm.</span></span>

4. <span data-ttu-id="0d46e-244">Use a chave simétrica para calcular a assinatura HMAC-SHA256 do valor em **dados**.</span><span class="sxs-lookup"><span data-stu-id="0d46e-244">Use the symmetric key to calculate the HMAC-SHA256 signature of the value in **data**.</span></span>
  
    <span data-ttu-id="0d46e-245">Compare-o com o valor em **dataSignature**.</span><span class="sxs-lookup"><span data-stu-id="0d46e-245">Compare it to the value in **dataSignature**.</span></span> <span data-ttu-id="0d46e-246">Se eles não corresponderem, considere que a carga foi adulterada e não a descriptografe.</span><span class="sxs-lookup"><span data-stu-id="0d46e-246">If they do not match, assume the payload has been tampered with and do not decrypt it.</span></span>

5. <span data-ttu-id="0d46e-247">Use a chave simétrica com a criptografia AES (como o .NET [AesCryptoServiceProvider](/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) para descriptografar o conteúdo em **dados**.</span><span class="sxs-lookup"><span data-stu-id="0d46e-247">Use the symmetric key with an Advanced Encryption Standard (AES) (such as the .NET [AesCryptoServiceProvider](/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) to decrypt the content in **data**.</span></span>

    - <span data-ttu-id="0d46e-248">Use os seguintes parâmetros de descriptografia para o algoritmo AES:</span><span class="sxs-lookup"><span data-stu-id="0d46e-248">Use the following decryption parameters for the AES algorithm:</span></span>

        - <span data-ttu-id="0d46e-249">Preenchimento: PKCS7</span><span class="sxs-lookup"><span data-stu-id="0d46e-249">Padding: PKCS7</span></span>
        - <span data-ttu-id="0d46e-250">Modo de criptografia: CBC</span><span class="sxs-lookup"><span data-stu-id="0d46e-250">Cipher mode: CBC</span></span>
    - <span data-ttu-id="0d46e-251">Defina o “vetor de inicialização” copiando os primeiros 16 bytes da chave simétrica usada para descriptografia.</span><span class="sxs-lookup"><span data-stu-id="0d46e-251">Set the "initialization vector" by copying the first 16 bytes of the symmetric key used for decryption.</span></span>

6. <span data-ttu-id="0d46e-252">O valor decriptado é uma sequência JSON que representa a instância do recurso na notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="0d46e-252">The decrypted value is a JSON string that represents the resource instance in the change notification.</span></span>


### <a name="example-decrypting-a-notification-with-encrypted-resource-data"></a><span data-ttu-id="0d46e-253">Exemplo: decriptando uma notificação com dados de recurso criptografados</span><span class="sxs-lookup"><span data-stu-id="0d46e-253">Example: decrypting a notification with encrypted resource data</span></span>

<span data-ttu-id="0d46e-254">A seguir, é apresentado um exemplo de notificação de alteração que inclui valores de propriedade criptografados de uma **chatMessage** instância em uma mensagem de canal.</span><span class="sxs-lookup"><span data-stu-id="0d46e-254">The following is an example change notification that includes encrypted property values of a **chatMessage** instance in a channel message.</span></span> <span data-ttu-id="0d46e-255">A instância é especificada pelo `@odata.id` valor.</span><span class="sxs-lookup"><span data-stu-id="0d46e-255">The instance is specified by the `@odata.id` value.</span></span>

```json
{
    "value": [
        {
            "subscriptionId": "76222963-cc7b-42d2-882d-8aaa69cb2ba3",
            "changeType": "created",
            // Other properties typical in a resource change notification
            "resource": "teams('d29828b8-c04d-4e2a-b2f6-07da6982f0f0')/channels('19:f127a8c55ad949d1a238464d22f0f99e@thread.skype')/messages('1565045424600')/replies('1565047490246')",
            "resourceData": {
                "id": "1565293727947",
                "@odata.type": "#Microsoft.Graph.ChatMessage",
                "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
            },
            "encryptedContent": {
                "data": "{encrypted data that produces a full resource}",
        "dataSignature": "<HMAC-SHA256 hash>",
                "dataKey": "{encrypted symmetric key from Microsoft Graph}",
                "encryptionCertificateId": "MySelfSignedCert/DDC9651A-D7BC-4D74-86BC-A8923584B0AB",
                "encryptionCertificateThumbprint": "07293748CC064953A3052FB978C735FB89E61C3D"
            }
        }
    ],
    "validationTokens": [
        "eyJ0eXAiOiJKV1QiLCJhbGciOiJSU..."
    ]
}
```

> <span data-ttu-id="0d46e-256">**Nota:** para obter uma descrição completa dos dados enviados quando as notificações de alterações são entregues, consulte [ changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="0d46e-256">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>


<span data-ttu-id="0d46e-257">A seção contém alguns trechos de código úteis que usam C# e .NET em cada etapa da descriptografia.</span><span class="sxs-lookup"><span data-stu-id="0d46e-257">This section contains some useful code snippets that use C# and .NET for each stage of decryption.</span></span>

#### <a name="decrypt-the-symmetric-key"></a><span data-ttu-id="0d46e-258">Descriptografar a chave simétrica</span><span class="sxs-lookup"><span data-stu-id="0d46e-258">Decrypt the symmetric key</span></span>

```csharp
// Initialize with the private key that matches the encryptionCertificateId.
RSACryptoServiceProvider rsaProvider = ...;        
byte[] encryptedSymmetricKey = Convert.FromBase64String(<value from dataKey property>);

// Decrypt using OAEP padding.
byte[] decryptedSymmetricKey = rsaProvider.Decrypt(encryptedSymmetricKey, fOAEP: true);

// Can now use decryptedSymmetricKey with the AES algorithm.
```
```Java
String storename = ""; //name/path of the jks store
String storepass = ""; //password used to open the jks store
String alias = ""; //alias of the certificate when store in the jks store, should be passed as encryptionCertificateId when subscribing and retrieved from the notification
KeyStore ks = KeyStore.getInstance("JKS");
ks.load(new FileInputStream(storename), storepass.toCharArray());
Key asymmetricKey = ks.getKey(alias, storepass.toCharArray());
byte[] encryptedSymetricKey = Base64.decodeBase64("<value from dataKey property>");
Cipher cipher = Cipher.getInstance("RSA/ECB/OAEPWithSHA1AndMGF1Padding");
cipher.init(Cipher.DECRYPT_MODE, asymmetricKey);
byte[] decryptedSymmetricKey = cipher.doFinal(encryptedSymetricKey);
// Can now use decryptedSymmetricKey with the AES algorithm.
```
```JavaScript
const base64encodedKey = 'base 64 encoded dataKey value';
const asymetricPrivateKey = 'pem encoded private key';
const decodedKey = Buffer.from(base64encodedKey, 'base64');
const decryptedSymetricKey = crypto.privateDecrypt(asymetricPrivateKey, decodedKey);
// Can now use decryptedSymmetricKey with the AES algorithm.
```

#### <a name="compare-data-signature-using-hmac-sha256"></a><span data-ttu-id="0d46e-259">Comparar assinatura de dados usando HMAC-SHA256</span><span class="sxs-lookup"><span data-stu-id="0d46e-259">Compare data signature using HMAC-SHA256</span></span>

```csharp
byte[] decryptedSymmetricKey = <the aes key decrypted in the previous step>;
byte[] encryptedPayload = <the value from the data property, still encrypted>;
byte[] expectedSignature = <the value from the dataSignature property>;
byte[] actualSignature;

using (HMACSHA256 hmac = new HMACSHA256(decryptedSymmetricKey))
{
    actualSignature = hmac.ComputeHash(encryptedPayload);
}
if (actualSignature.SequenceEqual(expectedSignature))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```
```Java
byte[] decryptedSymmetricKey = "<the aes key decrypted in the previous step>";
byte[] decodedEncryptedData = Base64.decodeBase64("data property from encryptedContent object");
Mac mac = Mac.getInstance("HMACSHA256");
SecretKey skey = new SecretKeySpec(decryptedSymmetricKey, "HMACSHA256");
mac.init(skey);
byte[] hashedData = mac.doFinal(decodedEncryptedData);
String encodedHashedData = new String(Base64.encodeBase64(hashedData));
if (comparisonSignature.equals(encodedHashedData))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```
```JavaScript
const decryptedSymetricKey = []; //Buffer provided by previous step
const base64encodedSignature = 'base64 encodded value from the dataSignature property';
const hmac = crypto.createHmac('sha256', decryptedSymetricKey);
hmac.write(base64encodedPayload, 'base64');
if(base64encodedSignature === hmac.digest('base64'))
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```

#### <a name="decrypt-the-resource-data-content"></a><span data-ttu-id="0d46e-260">Descriptografar o conteúdo dos dados de recursos</span><span class="sxs-lookup"><span data-stu-id="0d46e-260">Decrypt the resource data content</span></span>

```csharp
AesCryptoServiceProvider aesProvider = new AesCryptoServiceProvider();
aesProvider.Key = decryptedSymmetricKey;
aesProvider.Padding = PaddingMode.PKCS7;
aesProvider.Mode = CipherMode.CBC;

// Obtain the intialization vector from the symmetric key itself.
int vectorSize = 16;
byte[] iv = new byte[vectorSize];
Array.Copy(decryptedSymmetricKey, iv, vectorSize);
aesProvider.IV = iv;

byte[] encryptedPayload = Convert.FromBase64String(<value from dataKey property>);

string decryptedResourceData;
// Decrypt the resource data content.
using (var decryptor = aesProvider.CreateDecryptor())
{
  using (MemoryStream msDecrypt = new MemoryStream(encryptedPayload))
  {
      using (CryptoStream csDecrypt = new CryptoStream(msDecrypt, decryptor, CryptoStreamMode.Read))
      {
          using (StreamReader srDecrypt = new StreamReader(csDecrypt))
          {
              decryptedResourceData = srDecrypt.ReadToEnd();
          }
      }
  }
}

// decryptedResourceData now contains a JSON string that represents the resource.
```
```Java
SecretKey skey = new SecretKeySpec(decryptedSymmetricKey, "AES");
IvParameterSpec ivspec = new IvParameterSpec(Arrays.copyOf(decryptedSymmetricKey, 16));
Cipher cipher = Cipher.getInstance("AES/CBC/PKCS5PADDING");
cipher.init(Cipher.DECRYPT_MODE, skey, ivspec);
String decryptedResourceData = new String(cipher.doFinal(Base64.decodeBase64(encryptedData)));
```
```JavaScript
const base64encodedPayload = 'base64 encoded value from data property';
const decryptedSymetricKey = []; //Buffer provided by previous step
const iv = Buffer.alloc(16, 0);
decryptedSymetricKey.copy(iv, 0, 0, 16);
const decipher = crypto.createDecipheriv('aes-256-cbc', decryptedSymetricKey, iv);
let decryptedPayload = decipher.update(base64encodedPayload, 'base64', 'utf8');
decryptedPayload += decipher.final('utf8');
```

## <a name="see-also"></a><span data-ttu-id="0d46e-261">Confira também</span><span class="sxs-lookup"><span data-stu-id="0d46e-261">See also</span></span>

- [<span data-ttu-id="0d46e-262">Configurar notificações para alterações nos dados de usuário</span><span class="sxs-lookup"><span data-stu-id="0d46e-262">Set up notifications for changes in user data</span></span>](webhooks.md)
- [<span data-ttu-id="0d46e-263">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="0d46e-263">Subscription resource type</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="0d46e-264">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="0d46e-264">Get subscription</span></span>](/graph/api/subscription-get)
- [<span data-ttu-id="0d46e-265">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="0d46e-265">Create subscription</span></span>](/graph/api/subscription-post-subscriptions)
- [<span data-ttu-id="0d46e-266">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="0d46e-266">Update subscription</span></span>](/graph/api/subscription-update)
