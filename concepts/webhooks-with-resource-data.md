---
title: Configurar notificações de alteração que incluam dados de recursos (visualização)
description: O Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. As notificações de alteração podem incluir propriedades de recurso.
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.openlocfilehash: 9135a50f8dfa631ed85a23a12e2a146893b9994f
ms.sourcegitcommit: 4fa554d92a684d7720db1bd96befb9dea8d6ba5f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/30/2020
ms.locfileid: "44429555"
---
# <a name="set-up-change-notifications-that-include-resource-data-preview"></a><span data-ttu-id="1d631-104">Configurar notificações de alteração que incluam dados de recursos (visualização)</span><span class="sxs-lookup"><span data-stu-id="1d631-104">Set up change notifications that include resource data (preview)</span></span>

<span data-ttu-id="1d631-105">O Microsoft Graph permite que os aplicativos inscrevam-se para alterar as notificações de recursos através do [webhooks](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="1d631-105">Microsoft Graph allows apps to subscribe to change notifications for resources via [webhooks](webhooks.md).</span></span> <span data-ttu-id="1d631-106">Agora você pode configurar assinaturas para incluir os dados de recurso alterados (como o conteúdo de uma mensagem de chat do Microsoft Teams) em notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="1d631-106">You can now set up subscriptions to include the changed resource data (such as the content of a Microsoft Teams chat message) in change notifications.</span></span> <span data-ttu-id="1d631-107">Em seguida, seu aplicativo pode usar a lógica de negócios sem ter que fazer uma chamada à API separada para buscar o recurso alterado.</span><span class="sxs-lookup"><span data-stu-id="1d631-107">Your app can then run its business logic without having to make a separate API call to fetch the changed resource.</span></span> <span data-ttu-id="1d631-108">Como resultado, o aplicativo funciona melhor ao realizar menos chamadas da API, o que é benéfico em cenários de larga escala.</span><span class="sxs-lookup"><span data-stu-id="1d631-108">As a result, the app performs better by making fewer API calls, which is beneficial in large scale scenarios.</span></span>

<span data-ttu-id="1d631-109">Incluir dados de recurso como parte das notificações de alteração exige que você implemente a seguinte lógica adicional para satisfazer os requisitos de acesso e segurança de dados:</span><span class="sxs-lookup"><span data-stu-id="1d631-109">Including resource data as part of change notifications requires you to implement the following additional logic to satisfy data access and security requirements:</span></span> 

- <span data-ttu-id="1d631-110">[Lidar](#subscription-lifecycle-notifications) com notificações especiais de ciclo de vida de assinatura para manter um fluxo de dados sem interrupções.</span><span class="sxs-lookup"><span data-stu-id="1d631-110">[Handle](#subscription-lifecycle-notifications) special subscription lifecycle notifications to maintain an uninterrupted flow of data.</span></span> <span data-ttu-id="1d631-111">O Microsoft Graph envia notificações de ciclo de vida a tempo para exigir que um aplicativo seja reabilitado, para garantir que os problemas de acesso não foram cortados inesperadamente para incluir dados de recursos em notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="1d631-111">Microsoft Graph sends lifecycle notifications from time to time to require an app to re-authorize, to make sure access issues have not unexpectedly cropped up for including resource data in change notifications.</span></span>
- <span data-ttu-id="1d631-112">[Validar](#validating-the-authenticity-of-notifications) a autenticidade das notificações de alteração como tendo sido originadas no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1d631-112">[Validate](#validating-the-authenticity-of-notifications) the authenticity of change notifications as having originated from Microsoft Graph.</span></span>
- <span data-ttu-id="1d631-113">[Fornecer](#decrypting-resource-data-from-change-notifications) uma chave de criptografia pública e usar uma chave privada para descriptografar dados de recurso recebidos por meio de notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="1d631-113">[Provide](#decrypting-resource-data-from-change-notifications) a public encryption key and use a private key to decrypt resource data received through change notifications.</span></span>

## <a name="resource-data-in-notification-payload"></a><span data-ttu-id="1d631-114">Dados de recursos na carga de notificação </span><span class="sxs-lookup"><span data-stu-id="1d631-114">Resource data in notification payload</span></span>

<span data-ttu-id="1d631-115">Geralmente, esse tipo de notificação de alteração inclui os seguintes dados de recursos na carga:</span><span class="sxs-lookup"><span data-stu-id="1d631-115">In general, this type of change notifications include the following resource data in the payload:</span></span>

- <span data-ttu-id="1d631-116">ID e tipo de instância de recurso alterado, retornados na propriedade **resourceData**.</span><span class="sxs-lookup"><span data-stu-id="1d631-116">ID and type of the changed resource instance, returned in the **resourceData** property.</span></span>
- <span data-ttu-id="1d631-117">Todos os valores de propriedade da instância de recurso, criptografados conforme especificado na assinatura, retornados na propriedade **encryptedContent**.</span><span class="sxs-lookup"><span data-stu-id="1d631-117">All the property values of that resource instance, encrypted as specified in the subscription, returned in the **encryptedContent** property.</span></span>
- <span data-ttu-id="1d631-118">Or, dependendo do recurso, propriedades específicas retornadas na propriedade **resourceData**.</span><span class="sxs-lookup"><span data-stu-id="1d631-118">Or, depending on the resource, specific properties returned in the **resourceData** property.</span></span> <span data-ttu-id="1d631-119">Para obter somente propriedades específicas, especifique-as como parte da URL do **recurso** na assinatura, usando um parâmetro `$select`.</span><span class="sxs-lookup"><span data-stu-id="1d631-119">To get only specific properties, specify them as part of the **resource** URL in the subscription, using a `$select` parameter.</span></span>  


## <a name="supported-resources"></a><span data-ttu-id="1d631-120">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="1d631-120">Supported resources</span></span>

<span data-ttu-id="1d631-121">Atualmente, o recurso [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) (visualização) do Microsoft Teams oferece suporte a notificações de alteração que incluem dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="1d631-121">Currently, the Microsoft Teams [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) (preview) resource supports change notifications that include resource data.</span></span> <span data-ttu-id="1d631-122">Especificamente, você pode configurar uma assinatura que se aplique a uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="1d631-122">Specifically, you can set up a subscription that applies to one of the following:</span></span>

- <span data-ttu-id="1d631-123">Mensagens novas ou alteradas em um canal específico do Teams: `/teams/{id}/channels/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="1d631-123">New or changed messages in a specific Teams channel: `/teams/{id}/channels/{id}/messages`</span></span>
- <span data-ttu-id="1d631-124">Mensagens novas ou alteradas em um bate-papo específico do Teams: `/chats/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="1d631-124">New or changed messages in a specific Teams chat: `/chats/{id}/messages`</span></span>

<span data-ttu-id="1d631-125">O recurso **chat** oferece suporte incluindo todas as propriedades de uma instância alterada em uma notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="1d631-125">The **chatMessage** resource supports including all the properties of a changed instance in a change notification.</span></span> <span data-ttu-id="1d631-126">Não há suporte para retornar apenas propriedades seletivas da instância.</span><span class="sxs-lookup"><span data-stu-id="1d631-126">It does not support returning only selective properties of the instance.</span></span> 

<span data-ttu-id="1d631-127">Este artigo percorre um exemplo de assinatura de alteração de notificações de mensagens em um canal do Teams, com cada notificação de alteração, incluindo os dados completos de recurso da instância alterada do **chat** .</span><span class="sxs-lookup"><span data-stu-id="1d631-127">This article walks through an example of subscribing to change notifications of messages in a Teams channel, with each change notification including the full resource data of the changed **chatMessage** instance.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="1d631-128">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="1d631-128">Creating a subscription</span></span>

<span data-ttu-id="1d631-129">Para que os dados de recursos estejam incluídos nas notificações de alteração, você **deve** especificar as seguintes propriedades, além das que geralmente são especificadas ao [criar uma assinatura](webhooks.md#creating-a-subscription):</span><span class="sxs-lookup"><span data-stu-id="1d631-129">To have resource data included in change notifications, you **must** specify the following properties, in addition to those that are usually specified when [creating a subscription](webhooks.md#creating-a-subscription):</span></span>

- <span data-ttu-id="1d631-130">**includeResourceData** que deve ser definido como `true` para solicitar explicitamente os dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="1d631-130">**includeResourceData** which should be set to `true` to explicitly request resource data.</span></span>
- <span data-ttu-id="1d631-131">**lifecycleNotificationUrl** que é um ponto de extremidade onde as [notificações de ciclo de vida](#subscription-lifecycle-notifications) são entregues.</span><span class="sxs-lookup"><span data-stu-id="1d631-131">**lifecycleNotificationUrl** which is an endpoint where [lifecycle notifications](#subscription-lifecycle-notifications) are delivered.</span></span> <span data-ttu-id="1d631-132">Pode ser igual ou diferente de **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="1d631-132">This can be the same or different as **notificationUrl**.</span></span>
- <span data-ttu-id="1d631-133">**encryptionCertificate** que contém apenas a chave público que o Microsoft Graph usa para criptografar os dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="1d631-133">**encryptionCertificate** which contains only the public key that Microsoft Graph uses to encrypt resource data.</span></span> <span data-ttu-id="1d631-134">Mantenha a chave privada correspondente para [descriptografar o conteúdo](#decrypting-resource-data-from-change-notifications).</span><span class="sxs-lookup"><span data-stu-id="1d631-134">Keep the corresponding private key to [decrypt the content](#decrypting-resource-data-from-change-notifications).</span></span>
- <span data-ttu-id="1d631-135">**encryptionCertificateId** é o seu próprio identificador para o certificado.</span><span class="sxs-lookup"><span data-stu-id="1d631-135">**encryptionCertificateId** which is your own identifier for the certificate.</span></span> <span data-ttu-id="1d631-136">Use essa ID para corresponder a cada notificação de alteração, que certificado usar para descriptografia.</span><span class="sxs-lookup"><span data-stu-id="1d631-136">Use this ID to match in each change notification, which certificate to use for decryption.</span></span>

<span data-ttu-id="1d631-137">Lembre-se do seguinte:</span><span class="sxs-lookup"><span data-stu-id="1d631-137">Keep the following in mind:</span></span>

- <span data-ttu-id="1d631-138">Use o mesmo nome de host para os pontos de extremidade de notificação de alteração (**notificationUrl** e **lifecycleNotificationUrl**).</span><span class="sxs-lookup"><span data-stu-id="1d631-138">Use the same host name for both change notification endpoints (**notificationUrl** and **lifecycleNotificationUrl**).</span></span>
- <span data-ttu-id="1d631-139">Valide os dois pontos de extremidade conforme descrito [aqui](webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="1d631-139">Validate both endpoints as described [here](webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="1d631-140">Se você quiser usar a mesma URL para os dois pontos de extremidade, você receberá e responderá a duas solicitações de validação.</span><span class="sxs-lookup"><span data-stu-id="1d631-140">If you choose to use the same URL for both endpoints, you will receive and respond to two validation requests.</span></span>
- <span data-ttu-id="1d631-141">Não é possível atualizar (`PATCH`) uma assinatura existente para adicionar a propriedade **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="1d631-141">You cannot update (`PATCH`) an existing subscription to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="1d631-142">Você deve remover a assinatura existente e criar uma nova assinatura para incluir a propriedade **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="1d631-142">You should remove the existing subscription, and create a new subscription to include the **lifecycleNotificationUrl** property.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="1d631-143">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="1d631-143">Subscription request example</span></span>

<span data-ttu-id="1d631-144">O exemplo a seguir assina dois tipos de notificações:</span><span class="sxs-lookup"><span data-stu-id="1d631-144">The following example subscribes to two types of notifications:</span></span> 

- <span data-ttu-id="1d631-145">Alterações de recursos - canais de mensagens sendo criados ou atualizados no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="1d631-145">Resource changes - channel messages being created or updated in Microsoft Teams</span></span>
- <span data-ttu-id="1d631-146">Eventos de ciclo de vida de assinatura que podem afetar o fluxo de notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="1d631-146">Subscription lifecycle events which can affect the flow of change notifications.</span></span> <span data-ttu-id="1d631-147">Veja mais detalhes sobre as notificações do ciclo de vida na [próxima seção](#subscription-lifecycle-notifications).</span><span class="sxs-lookup"><span data-stu-id="1d631-147">See more details about lifecycle notifications in the [next section](#subscription-lifecycle-notifications).</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="subscription-response"></a><span data-ttu-id="1d631-148">Resposta de assinatura</span><span class="sxs-lookup"><span data-stu-id="1d631-148">Subscription response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificateId": "{custom ID}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secret client state}"
}
```

## <a name="subscription-lifecycle-notifications"></a><span data-ttu-id="1d631-149">Notificações de ciclo de vida de assinatura</span><span class="sxs-lookup"><span data-stu-id="1d631-149">Subscription lifecycle notifications</span></span>

<span data-ttu-id="1d631-150">Determinados eventos podem interferir no fluxo de notificação de alteração em uma assinatura existente.</span><span class="sxs-lookup"><span data-stu-id="1d631-150">Certain events can interfere with change notification flow in an existing subscription.</span></span> <span data-ttu-id="1d631-151">Notificações de ciclo de vida de assinatura informam ações a serem tomadas para manter um fluxo sem interrupção.</span><span class="sxs-lookup"><span data-stu-id="1d631-151">Subscription lifecycle notifications inform you actions to take in order to maintain an uninterrupted flow.</span></span> <span data-ttu-id="1d631-152">Ao contrário de uma notificação de alteração de recurso que informa uma alteração em uma instância de recurso, uma notificação de ciclo de vida é sobre a própria assinatura e seu estado atual no ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="1d631-152">Unlike a resource change notification which informs a change to a resource instance, a lifecycle notification is about the subscription itself, and its current state in the lifecycle.</span></span> 

<span data-ttu-id="1d631-153">As notificações de ciclo de vida são entregues no **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="1d631-153">Lifecycle notifications are delivered to the **lifecycleNotificationUrl**.</span></span> 

<span data-ttu-id="1d631-154">Nesta seção:</span><span class="sxs-lookup"><span data-stu-id="1d631-154">In this section:</span></span>

- [<span data-ttu-id="1d631-155">Notificação de ciclo de vida que desafia a autorização de assinatura</span><span class="sxs-lookup"><span data-stu-id="1d631-155">Lifecycle notification that challenges subscription authorization</span></span>](#lifecycle-notification-that-challenges-subscription-authorization)
- [<span data-ttu-id="1d631-156">Fluxo de desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="1d631-156">Authorization challenge flow</span></span>](#authorization-challenge-flow)
- [<span data-ttu-id="1d631-157">Exemplo de desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="1d631-157">Example authorization challenge</span></span>](#example-authorization-challenge)
- [<span data-ttu-id="1d631-158">Respondendo a um desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="1d631-158">Responding to an authorization challenge</span></span>](#responding-to-an-authorization-challenge)
- [<span data-ttu-id="1d631-159">Dicas</span><span class="sxs-lookup"><span data-stu-id="1d631-159">Tips</span></span>](#tips)
- [<span data-ttu-id="1d631-160">Tornar o seu código com o futuro à prova de lidar com outros tipos de notificações do ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="1d631-160">Future-proof your code to handle other types of lifecycle notifications</span></span>](#future-proof-your-code-to-handle-other-types-of-lifecycle-notifications)

### <a name="lifecycle-notification-that-challenges-subscription-authorization"></a><span data-ttu-id="1d631-161">Notificação de ciclo de vida que desafia a autorização de assinatura</span><span class="sxs-lookup"><span data-stu-id="1d631-161">Lifecycle notification that challenges subscription authorization</span></span>

<span data-ttu-id="1d631-162">Um tipo de notificação de ciclo de vida desafia o estado autorizado de uma assinatura ativa.</span><span class="sxs-lookup"><span data-stu-id="1d631-162">One type of lifecycle notifications challenges the authorized state of an active subscription.</span></span> <span data-ttu-id="1d631-163">Quando a propriedade **lifecycleEvent** em uma notificação indica `reauthorizationRequired`, você deve autorizar novamente a assinatura para manter o fluxo de dados.</span><span class="sxs-lookup"><span data-stu-id="1d631-163">When the **lifecycleEvent** property in a notification indicates `reauthorizationRequired`, you must re-authorize the subscription to maintain the data flow.</span></span>

<span data-ttu-id="1d631-164">Quando você cria uma assinatura de longa vida (por exemplo, uma que dura 3 dias), as notificações de alteração fluem para o local indicado em **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="1d631-164">When you create a long-lived subscription (for example, one that lasts for 3 days), change notifications flows to the location indicated in **notificationUrl**.</span></span> <span data-ttu-id="1d631-165">Entretanto, a qualquer momento, o Microsoft Graph pode exigir que você autorize novamente a assinatura para provar que ainda tem acesso aos dados de recursos, caso as condições de acesso tenham sido alteradas desde a criação da assinatura.</span><span class="sxs-lookup"><span data-stu-id="1d631-165">However, at any point in time, Microsoft Graph may require that you re-authorize the subscription to prove that you still have access to resource data, in case the conditions of access have changed since the subscription was created.</span></span> <span data-ttu-id="1d631-166">A seguir estão exemplos de alterações que afetam o acesso aos dados:</span><span class="sxs-lookup"><span data-stu-id="1d631-166">The following are examples of changes that affect your access to data:</span></span>

- <span data-ttu-id="1d631-167">Um administrador de locatários pode revogar as permissões do seu aplicativo para ler um recurso.</span><span class="sxs-lookup"><span data-stu-id="1d631-167">A tenant administrator may revoke your app's permissions to read a resource.</span></span>
- <span data-ttu-id="1d631-168">Em um cenário interativo, o usuário que fornece o token de autenticação ao seu aplicativo pode estar sujeito a políticas dinâmicas com base em vários fatores, como o local, o estado do dispositivo ou a avaliação de risco.</span><span class="sxs-lookup"><span data-stu-id="1d631-168">In an interactive scenario, the user who provides the authentication token to your app may be subject to dynamic policies based on various factors, such as their location, device state, or risk assesment.</span></span> <span data-ttu-id="1d631-169">Por exemplo, se o usuário alterar o seu local físico, pode ser que ele não tenha mais permissão para acessar os dados e seu aplicativo não conseguirá autorizar novamente a assinatura.</span><span class="sxs-lookup"><span data-stu-id="1d631-169">For example, if the user changes their physical location, the user may no longer be allowed to access the data, and your app will not be able to re-authorize the subscription.</span></span> <span data-ttu-id="1d631-170">Para saber mais sobre políticas dinâmicas que controlam o acesso, confira [políticas de acesso condicional do Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/overview).</span><span class="sxs-lookup"><span data-stu-id="1d631-170">For more information on dynamic policies that control access, see [Azure AD conditional access policies](https://docs.microsoft.com/azure/active-directory/conditional-access/overview).</span></span> 

### <a name="authorization-challenge-flow"></a><span data-ttu-id="1d631-171">Fluxo de desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="1d631-171">Authorization challenge flow</span></span>

<span data-ttu-id="1d631-172">O fluxo de um desafio de autorização para uma assinatura ativa e não expirada tem a seguinte aparência:</span><span class="sxs-lookup"><span data-stu-id="1d631-172">The flow of an authorization challenge for an active, non-expired subscription looks as follows:</span></span>

1. <span data-ttu-id="1d631-173">O Microsoft Graph exige que uma assinatura seja autorizada novamente.</span><span class="sxs-lookup"><span data-stu-id="1d631-173">Microsoft Graph requires a subscription to be re-authorized</span></span>
    
    <span data-ttu-id="1d631-174">Os motivos para isso podem variar de recurso para recurso e podem mudar com o tempo.</span><span class="sxs-lookup"><span data-stu-id="1d631-174">The reasons for this may vary from resource to resource, and may change over time.</span></span> <span data-ttu-id="1d631-175">Independentemente da causa do evento de reautorização, você precisará respondê-lo.</span><span class="sxs-lookup"><span data-stu-id="1d631-175">Regardless of the cause of the re-authorization event, you will need to respond to it.</span></span>

2. <span data-ttu-id="1d631-176">O Microsoft Graph envia uma notificação de desafio de autorização para **lifecycleNotificationUrl**</span><span class="sxs-lookup"><span data-stu-id="1d631-176">Microsoft Graph sends an authorization challenge notification to the **lifecycleNotificationUrl**</span></span>

    <span data-ttu-id="1d631-177">Observe que o fluxo de notificações de alteração pode continuar por algum tempo, dando a você um tempo adicional para responder.</span><span class="sxs-lookup"><span data-stu-id="1d631-177">Note that the flow of change notifications may continue for a while, giving you extra time to respond.</span></span> <span data-ttu-id="1d631-178">No entanto, eventualmente a entrega da notificação de alteração será pausada, até que você execute a ação necessária.</span><span class="sxs-lookup"><span data-stu-id="1d631-178">However, eventually change notification delivery will pause, until you take the required action.</span></span>

3. <span data-ttu-id="1d631-179">Responda a essa notificação de ciclo de vida de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="1d631-179">Respond to this lifecycle notification in one of two ways:</span></span>
    1. <span data-ttu-id="1d631-180">Autorize a assinatura novamente.</span><span class="sxs-lookup"><span data-stu-id="1d631-180">Re-authorize the subscription.</span></span> <span data-ttu-id="1d631-181">Isso não estende a data de vencimento da assinatura.</span><span class="sxs-lookup"><span data-stu-id="1d631-181">This does not extend the expiry date of the subscription.</span></span>
    2. <span data-ttu-id="1d631-182">Renove a assinatura.</span><span class="sxs-lookup"><span data-stu-id="1d631-182">Renew the subscription.</span></span> <span data-ttu-id="1d631-183">Isso reautoriza e estenda a data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="1d631-183">This both re-authorizes and extends the expiry date.</span></span>

    <span data-ttu-id="1d631-184">Observação: as duas ações exigem a apresentação de um token de autenticação válido, semelhante a [criar uma nova assinatura](webhooks.md#creating-a-subscription) ou [renova uma assinatura antes da sua expiração](webhooks.md#renewing-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="1d631-184">Note: Both actions require you to present a valid authentication token, similar to [creating a new subscription](webhooks.md#creating-a-subscription) or [renewing a subscription before its expiry](webhooks.md#renewing-a-subscription).</span></span>

4. <span data-ttu-id="1d631-185">Se você conseguir autorizar novamente ou renovar a assinatura, as notificações de alteração continuarão.</span><span class="sxs-lookup"><span data-stu-id="1d631-185">If you successfully re-authorize or renew the subscription, change notifications continue.</span></span> <span data-ttu-id="1d631-186">Caso contrário, as notificações de alteração permanecerão em pausa.</span><span class="sxs-lookup"><span data-stu-id="1d631-186">Otherwise, change notifications remain paused.</span></span>
    
### <a name="example-authorization-challenge"></a><span data-ttu-id="1d631-187">Exemplo de desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="1d631-187">Example authorization challenge</span></span>

<span data-ttu-id="1d631-188">Veja a seguir um exemplo de notificação de ciclo de vida que solicita a recriação de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="1d631-188">Below is an example lifecycle notification that requests re-authorizing a subscription.</span></span> 

<span data-ttu-id="1d631-189">Observe o seguinte:</span><span class="sxs-lookup"><span data-stu-id="1d631-189">Note the following:</span></span>

- <span data-ttu-id="1d631-190">O campo `"lifecycleEvent": "reauthorizationRequired"` identifica essa notificação como um desafio de autorização.</span><span class="sxs-lookup"><span data-stu-id="1d631-190">The `"lifecycleEvent": "reauthorizationRequired"` field identifies this notification as an authorization challenge.</span></span>
- <span data-ttu-id="1d631-191">A notificação de ciclo de vida não contém informações sobre um recurso específico, pois ela não está relacionada a uma alteração de recurso, mas à alteração de estado de assinatura.</span><span class="sxs-lookup"><span data-stu-id="1d631-191">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="1d631-192">Semelhante a notificações de alteração, você pode enviar notificações de ciclo de vida em lote (na coleção de **valor** ), cada uma com um valor possivelmente diferente de **lifecycleEvent** .</span><span class="sxs-lookup"><span data-stu-id="1d631-192">Similar to change notifications, you can batch lifecycle notifications together (in the **value** collection), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="1d631-193">Processe a cada notificação de ciclo de vida no lote.</span><span class="sxs-lookup"><span data-stu-id="1d631-193">Process each lifecycle notification in the batch accordingly.</span></span>

```json
{
  "value": [
    {
      "lifecycleEvent": "reauthorizationRequired",
      "subscriptionId": "e3898f08-5cd0-4a6a-80fc-6addbfb73b7b",
      "subscriptionExpirationDateTime": "2019-09-18T00:52:45.9696658+00:00",
      "clientState": "{secret client state}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95"
    }
  ]
}
```

> <span data-ttu-id="1d631-194">**Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração são entregues, consulte [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="1d631-194">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="responding-to-an-authorization-challenge"></a><span data-ttu-id="1d631-195">Respondendo a um desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="1d631-195">Responding to an authorization challenge</span></span>

<span data-ttu-id="1d631-196">Siga as etapas abaixo para processar uma notificação de ciclo de vida de desafio de autorização.</span><span class="sxs-lookup"><span data-stu-id="1d631-196">Take the following steps to process an authorization challenge lifecycle notification.</span></span> <span data-ttu-id="1d631-197">As duas primeiras etapas para confirmar e validar a notificação de ciclo de vida é semelhante a [responder a uma notificação de alteração de recurso](webhooks.md#processing-the-change-notification).</span><span class="sxs-lookup"><span data-stu-id="1d631-197">The first two steps of acknowledging and validating the lifecycle notification is similar to [responding to a resource change notification](webhooks.md#processing-the-change-notification).</span></span>

1. <span data-ttu-id="1d631-198">Confirme o recebimento da notificação de ciclo de vida, respondendo à chamada POST com `HTTP 202 Accepted` .</span><span class="sxs-lookup"><span data-stu-id="1d631-198">Acknowledge the receipt of the lifecycle notification, by responding to the POST call with `HTTP 202 Accepted`.</span></span>
2. <span data-ttu-id="1d631-199">Validar a autenticidade da notificação de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="1d631-199">Validate the authenticity of the lifecycle notification.</span></span> <span data-ttu-id="1d631-200">Mais detalhes [abaixo](#validating-the-authenticity-of-notifications).</span><span class="sxs-lookup"><span data-stu-id="1d631-200">Further details [below](#validating-the-authenticity-of-notifications).</span></span>
3. <span data-ttu-id="1d631-201">Certifique-se de que o aplicativo tenha um token de acesso válido para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="1d631-201">Ensure the app has a valid access token to take the next step.</span></span> 

    <span data-ttu-id="1d631-202">Se você estiver usando uma das [bibliotecas de autenticação](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), a biblioteca fará isso para você ao reutilizar um token de cache válido ou obtendo um novo token ao pedir ao usuário para fazer logon novamente com uma nova senha.</span><span class="sxs-lookup"><span data-stu-id="1d631-202">If you are using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), the library handles this for you by either reusing a valid cached token, or obtaining a new token from prompting the user to log in again with a new password.</span></span> <span data-ttu-id="1d631-203">Entretanto, a obtenção de um novo token pode falhar, pois as condições de acesso podem ser alteradas e o usuário não poderá mais acessar os dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="1d631-203">However, obtaining a new token may fail, since the conditions of access may have changed, and the user may no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="1d631-204">Chamar uma das duas APIs a seguir.</span><span class="sxs-lookup"><span data-stu-id="1d631-204">Call either of the following two APIs.</span></span> <span data-ttu-id="1d631-205">Se a chamada da API tiver êxito, o fluxo de notificação de alteração será retomado.</span><span class="sxs-lookup"><span data-stu-id="1d631-205">If the API call succeeds, the change notification flow resumes.</span></span>

    - <span data-ttu-id="1d631-206">Chame a ação `/reauthorize` para autorizar novamente a assinatura sem estender a data de vencimento:</span><span class="sxs-lookup"><span data-stu-id="1d631-206">Call the `/reauthorize` action to re-authorize the subscription without extending its expiration date:</span></span>
        ```http
        POST  https://graph.microsoft.com/beta/subscriptions/{id}/reauthorize
        Content-type: application/json
        ```
    - <span data-ttu-id="1d631-207">Execute uma ação de renovação regular para autorizar novamente e renova a assinatura ao mesmo tempo:</span><span class="sxs-lookup"><span data-stu-id="1d631-207">Perform a regular renew action to re-authorize and renew the subscription at the same time:</span></span>
        ```http
        PATCH https://graph.microsoft.com/beta/subscriptions/{id}
        Content-Type: application/json

        {
           "expirationDateTime": "2019-09-21T11:00:00.0000000Z"
        }
        ```

      <span data-ttu-id="1d631-208">A renovação pode falhar, porque as verificações de autorização realizadas pelo sistema podem recusar o aplicativo ou o acesso do usuário ao recurso.</span><span class="sxs-lookup"><span data-stu-id="1d631-208">Renewing may fail, because the authorization checks performed by the system may deny the app or the user access to the resource.</span></span> <span data-ttu-id="1d631-209">Pode ser necessário que o aplicativo obtenha um novo token de acesso do usuário para autorizar novamente com êxito uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="1d631-209">It may be necessary for the app to obtain a new access token from the user to successfully re-authorize a subscription.</span></span> 
      
      <span data-ttu-id="1d631-210">Você pode tentar essa ações mais tarde, a qualquer momento e obter êxito se as condições de acesso mudarem.</span><span class="sxs-lookup"><span data-stu-id="1d631-210">You may retry these actions later, at any time, and succeed if the conditions of access change.</span></span> <span data-ttu-id="1d631-211">Quaisquer notificações sobre as alterações de recursos que ocorrem entre o momento em que a notificação de ciclo de vida foi enviada e o momento em que o aplicativo recria a inscrição foi perdida com êxito.</span><span class="sxs-lookup"><span data-stu-id="1d631-211">Any notifications about resource changes that happen between the time the lifecycle notification was sent, and the time when the app eventually re-creates the subscription successfully, would be lost.</span></span> <span data-ttu-id="1d631-212">Nesses casos, o aplicativo deve buscar essas mudanças separadamente.</span><span class="sxs-lookup"><span data-stu-id="1d631-212">In such cases, the app should separately fetch those changes.</span></span>

### <a name="tips"></a><span data-ttu-id="1d631-213">Dicas </span><span class="sxs-lookup"><span data-stu-id="1d631-213">Tips</span></span>

<span data-ttu-id="1d631-214">Lembre-se do seguinte:</span><span class="sxs-lookup"><span data-stu-id="1d631-214">Keep the following in mind:</span></span>

1. <span data-ttu-id="1d631-215">Os desafios de autorização não substituem a necessidade de renova uma assinatura de alteração de recursos antes de expirar.</span><span class="sxs-lookup"><span data-stu-id="1d631-215">Authorization challenges do not replace the need to renew a resource change subscription before it expires.</span></span> 

    <span data-ttu-id="1d631-216">Embora você possa optar por renovar uma assinatura quando recebe um desafio de autorização, o Microsoft Graph pode não desafiar todas as suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="1d631-216">While you can choose to renew a subscription when you receive an authorization challenge, Microsoft Graph may not challenge all of your subscriptions.</span></span> <span data-ttu-id="1d631-217">Por exemplo, uma assinatura que não tem nenhuma atividade e não tem notificações de alteração pendentes pode não sinalizar quaisquer desafios de Reautorização para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1d631-217">For example, a subscription that does not have any activity and has no change notifications pending delivery may not signal any re-authorization challenges to your app.</span></span> <span data-ttu-id="1d631-218">Certifique-se de [renovar assinaturas](webhooks.md#renewing-a-subscription) antes de expirarem.</span><span class="sxs-lookup"><span data-stu-id="1d631-218">Make sure to [renew subscriptions](webhooks.md#renewing-a-subscription) before they expire.</span></span>

2. <span data-ttu-id="1d631-219">A frequência dos desafios de autorização está sujeita a mudanças.</span><span class="sxs-lookup"><span data-stu-id="1d631-219">The frequency of authorization challenges is subject to change.</span></span>

    <span data-ttu-id="1d631-220">Não faça suposições sobre a frequência dos desafios de autorização.</span><span class="sxs-lookup"><span data-stu-id="1d631-220">Do not make assumptions about the frequency of authorization challenges.</span></span> <span data-ttu-id="1d631-221">Essas notificações de ciclo de vida indicam quando realizar ações, poupando a necessidade de rastrear quais assinaturas exigem nova autorização.</span><span class="sxs-lookup"><span data-stu-id="1d631-221">These lifecycle notifications tell you when to take actions, saving you from having to track which subscriptions require re-authorization.</span></span> <span data-ttu-id="1d631-222">Esteja pronto para lidar com os desafios de autorização seja uma vez em alguns minutos para cada assinatura ou raramente para algumas das suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="1d631-222">Be ready to handle authorization challenges anywhere from once a few minutes for every subscription, to rarely for only some of your subscriptions.</span></span>

### <a name="future-proof-your-code-to-handle-other-types-of-lifecycle-notifications"></a><span data-ttu-id="1d631-223">Tornar o seu código com o futuro à prova de lidar com outros tipos de notificações do ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="1d631-223">Future-proof your code to handle other types of lifecycle notifications</span></span>

<span data-ttu-id="1d631-224">Espera que as notificações do ciclo de vida da assinatura sejam lançadas no mesmo ponto de extremidade especificado por **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="1d631-224">Expect subscription lifecycle notifications to be posted to the same endpoint specified by **lifecycleNotificationUrl**.</span></span> <span data-ttu-id="1d631-225">Elas são diferenciadas pela propriedade **lifecycleEvent** e podem conter um esquema e propriedades ligeiramente diferentes para atender aos cenários que resolvem.</span><span class="sxs-lookup"><span data-stu-id="1d631-225">They differentiate by the **lifecycleEvent** property and may contain slightly different schema and properties to serve the scenarios they address.</span></span>

<span data-ttu-id="1d631-226">Implementar o código na antecipação de novos tipos de notificações de ciclo de vida:</span><span class="sxs-lookup"><span data-stu-id="1d631-226">Implement your code in anticipation of new types of lifecycle notifications:</span></span>

1. <span data-ttu-id="1d631-227">Use a propriedade **lifecycleEvent** para identificar o tipo de notificação para determinar a resposta adequada.</span><span class="sxs-lookup"><span data-stu-id="1d631-227">Use the **lifecycleEvent** property to identify the type of notification so to determine the appropriate response.</span></span> <span data-ttu-id="1d631-228">Por exemplo, procure a `"lifecycleEvent": "reauthorizationRequired"` propriedade para identificar um evento específico e tratá-lo.</span><span class="sxs-lookup"><span data-stu-id="1d631-228">For example, look for the `"lifecycleEvent": "reauthorizationRequired"` property to identify a specific event, and handle it.</span></span>

1. <span data-ttu-id="1d631-229">Registre quaisquer eventos de ciclo de vida que seu aplicativo não reconhece para obter conscientização.</span><span class="sxs-lookup"><span data-stu-id="1d631-229">Log any lifecycle events that your app does not recognize to gain awareness.</span></span>

1. <span data-ttu-id="1d631-230">Assine o [blog do desenvolvedor do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) para observar anúncios de notificações de ciclo de vida para novos cenários.</span><span class="sxs-lookup"><span data-stu-id="1d631-230">Subscribe to the [Microsoft Graph Developer Blog](https://developer.microsoft.com/graph/blogs/) to watch for announcements of lifecycle notifications for new scenarios.</span></span>

1. <span data-ttu-id="1d631-231">Procure documentação relacionada para novas notificações de ciclo de vida e implemente o suporte para elas conforme apropriado.</span><span class="sxs-lookup"><span data-stu-id="1d631-231">Look up related documentation for new lifecycle notifications and implement support for them as appropriate.</span></span>

## <a name="validating-the-authenticity-of-notifications"></a><span data-ttu-id="1d631-232">Validar a autenticidade das notificações </span><span class="sxs-lookup"><span data-stu-id="1d631-232">Validating the authenticity of notifications</span></span>

<span data-ttu-id="1d631-233">Os aplicativos geralmente executam lógica de negócios com base nos dados de recurso incluídos nas notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="1d631-233">Apps often execute business logic based on resource data included in change notifications.</span></span> <span data-ttu-id="1d631-234">Verificamos primeiro a autenticidade de cada notificação de alteração é importante.</span><span class="sxs-lookup"><span data-stu-id="1d631-234">Having first verified the authenticity of each change notification is important.</span></span> <span data-ttu-id="1d631-235">Caso contrário, um terceiro pode falsificar seu aplicativo com notificações de alteração falsas, fazê-lo executar a lógica de negócios incorretamente e levar a um incidente de segurança.</span><span class="sxs-lookup"><span data-stu-id="1d631-235">Otherwise, a third party could spoof your app with false change notifications, make it execute its business logic incorrectly, and lead to a security incident.</span></span>

<span data-ttu-id="1d631-236">Para notificações de alteração básicas que não contêm dados de recurso, basta validá-los com base no valor de **ClientState** , conforme descrito [aqui](webhooks.md#processing-the-change-notification).</span><span class="sxs-lookup"><span data-stu-id="1d631-236">For basic change notifications which do not contain resource data, simply validate them based on the **clientState** value as described [here](webhooks.md#processing-the-change-notification).</span></span> <span data-ttu-id="1d631-237">Isso é aceitável, uma vez que você pode fazer chamadas confiáveis subsequentes do Microsoft Graph para obter acesso ao dados do recurso, portanto, o impacto das tentativas de falsificação é limitado.</span><span class="sxs-lookup"><span data-stu-id="1d631-237">This is acceptable, as you can make subsequent trusted Microsoft Graph calls to get access to resource data, and therefore the impact of any spoofing attempts is limited.</span></span> 

<span data-ttu-id="1d631-238">Para notificações de alteração que oferecem dados de recurso, execute uma validação mais completa antes de processar os dados.</span><span class="sxs-lookup"><span data-stu-id="1d631-238">For change notifications that deliver resource data, perform a more thorough validation before processing the data.</span></span>

<span data-ttu-id="1d631-239">Nesta seção:</span><span class="sxs-lookup"><span data-stu-id="1d631-239">In this section:</span></span>

- [<span data-ttu-id="1d631-240">Tokens de validação na notificação de alteração</span><span class="sxs-lookup"><span data-stu-id="1d631-240">Validation tokens in the change notification</span></span>](#validation-tokens-in-the-change-notification)
- [<span data-ttu-id="1d631-241">Como validar</span><span class="sxs-lookup"><span data-stu-id="1d631-241">How to validate</span></span>](#how-to-validate)
- [<span data-ttu-id="1d631-242">Exemplo de token JWT</span><span class="sxs-lookup"><span data-stu-id="1d631-242">Example JWT token</span></span>](#example-jwt-token)

### <a name="validation-tokens-in-the-change-notification"></a><span data-ttu-id="1d631-243">Tokens de validação na notificação de alteração</span><span class="sxs-lookup"><span data-stu-id="1d631-243">Validation tokens in the change notification</span></span>

<span data-ttu-id="1d631-244">Uma notificação de alteração com dados de recurso contém uma propriedade adicional, **validationTokens**, que contém uma matriz de tokens JWT gerados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1d631-244">A change notification with resource data contains an additional property, **validationTokens**, which contains an array of JWT tokens generated by Microsoft Graph.</span></span> <span data-ttu-id="1d631-245">O Microsoft Graph gera um único token para cada aplicativo distinto e par de locatários para os quais há um item na matriz **valor**.</span><span class="sxs-lookup"><span data-stu-id="1d631-245">Microsoft Graph generates a single token for each distinct app and tenant pair for whom there is an item in the **value** array.</span></span> <span data-ttu-id="1d631-246">Tenha em mente que as notificações de alteração podem conter uma mistura de itens para vários aplicativos e locatários que são inscritos usando o mesmo **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="1d631-246">Keep in mind that change notifications may contain a mix of items for various apps and tenants that subscribed using the same **notificationUrl**.</span></span>

<span data-ttu-id="1d631-247">No exemplo a seguir, a notificação de alteração contém dois itens para o mesmo aplicativo e dois locatários diferentes, portanto, a matriz **validationTokens** contém dois tokens que precisam ser validados.</span><span class="sxs-lookup"><span data-stu-id="1d631-247">In the following example, the change notification contains two items for the same app, and for two different tenants, therefore the **validationTokens** array contains two tokens that need to be validated.</span></span>

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

> <span data-ttu-id="1d631-248">**Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração são entregues, consulte [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="1d631-248">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="how-to-validate"></a><span data-ttu-id="1d631-249">Como validar</span><span class="sxs-lookup"><span data-stu-id="1d631-249">How to validate</span></span>

<span data-ttu-id="1d631-250">Se você for novo na validação do token, consulte [princípios de validação de token](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) para obter uma visão geral.</span><span class="sxs-lookup"><span data-stu-id="1d631-250">If you're new to token validation, see [Principles of Token Validation](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) for an overview.</span></span> <span data-ttu-id="1d631-251">Use um SDK, como a biblioteca [System. IdentityModel. Tokens. JWT](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) para .net ou uma biblioteca de terceiros para uma plataforma diferente.</span><span class="sxs-lookup"><span data-stu-id="1d631-251">Use an SDK, such as the [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) library for .NET, or a third-party library for a different platform.</span></span>

<span data-ttu-id="1d631-252">Fique atento ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="1d631-252">Be mindful of the following:</span></span> 

- <span data-ttu-id="1d631-253">Certifique-se de sempre enviar um `HTTP 202 Accepted` código de status como parte da resposta à notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="1d631-253">Make sure to always send an `HTTP 202 Accepted` status code as part of the response to the change notification.</span></span> 
- <span data-ttu-id="1d631-254">Faça isso antes de validar a notificação de alteração (por exemplo, se você armazenar notificações de alteração em filas para processamento posterior) ou após (se você processá-las imediatamente), mesmo se a validação falhar.</span><span class="sxs-lookup"><span data-stu-id="1d631-254">Do that before validating the change notification (for example, if you store change notifications in queues for later processing) or after (if you process them on the fly), even if validation failed.</span></span>
- <span data-ttu-id="1d631-255">A aceitação de uma notificação de alteração impede tentativas desnecessárias de entrega e também impede que possíveis atores não autorizados descubram se passaram ou falharam a validação.</span><span class="sxs-lookup"><span data-stu-id="1d631-255">Accepting a change notification prevents unnecessary delivery retries and it also prevents any potential rogue actors from finding out if they passed or failed validation.</span></span> <span data-ttu-id="1d631-256">Você sempre pode optar por ignorar uma notificação de alteração inválida após aceitá-la.</span><span class="sxs-lookup"><span data-stu-id="1d631-256">You can always choose to ignore an invalid change notification after you have accepted it.</span></span>

<span data-ttu-id="1d631-257">Especificamente, realize a validação em todos os tokens JWT na coleção **validationTokens**.</span><span class="sxs-lookup"><span data-stu-id="1d631-257">In particular, perform validation on every JWT token in the **validationTokens** collection.</span></span> <span data-ttu-id="1d631-258">Se algum token falhar, considere a notificação de alteração suspeita e investigue ainda mais.</span><span class="sxs-lookup"><span data-stu-id="1d631-258">If any tokens fail, consider the change notification suspicious and investigate further.</span></span> 

<span data-ttu-id="1d631-259">Use as etapas a seguir para validar tokens e aplicativos que geram tokens:</span><span class="sxs-lookup"><span data-stu-id="1d631-259">Use the following steps to validate tokens and apps that generate tokens:</span></span>

1. <span data-ttu-id="1d631-260">Valide se o token não expirou.</span><span class="sxs-lookup"><span data-stu-id="1d631-260">Validate that the token has not expired.</span></span>

2. <span data-ttu-id="1d631-261">Valide se o token não foi adulterado e foi emitido pela autoridade esperada, o Active Directory do Microsoft Azure:</span><span class="sxs-lookup"><span data-stu-id="1d631-261">Validate the token has not been tampered with and was issued by the expected authority, Microsoft Azure Active Directory:</span></span>

    - <span data-ttu-id="1d631-262">Obtenha as chaves de assinatura do ponto de extremidade de configuração comum: `https://login.microsoftonline.com/common/.well-known/openid-configuration`.</span><span class="sxs-lookup"><span data-stu-id="1d631-262">Obtain the signing keys from the common configuration endpoint: `https://login.microsoftonline.com/common/.well-known/openid-configuration`.</span></span> <span data-ttu-id="1d631-263">Essa configuração é armazenada em cache pelo aplicativo por um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="1d631-263">This configuration is cached by your app for a period of time.</span></span> <span data-ttu-id="1d631-264">Lembre-se de que a configuração é atualizada frequentemente, uma vez que as chaves de assinatura são giradas diariamente.</span><span class="sxs-lookup"><span data-stu-id="1d631-264">Be aware that the configuration is updated frequently as signing keys are rotated daily.</span></span>
    - <span data-ttu-id="1d631-265">Verifique a assinatura do token JWT usando essas chaves.</span><span class="sxs-lookup"><span data-stu-id="1d631-265">Verify the signature of the JWT token using those keys.</span></span>

    <span data-ttu-id="1d631-266">Não aceite tokens emitidos por outra autoridade.</span><span class="sxs-lookup"><span data-stu-id="1d631-266">Do not accept tokens issued by any other authority.</span></span>

3. <span data-ttu-id="1d631-267">Valide se o token foi emitido para o aplicativo que está inscrito para alterar as notificações.</span><span class="sxs-lookup"><span data-stu-id="1d631-267">Validate that the token was issued for your app that is subscribing to change notifications.</span></span>

    <span data-ttu-id="1d631-268">As etapas a seguir fazem parte da lógica de validação padrão nas bibliotecas de token JWT e podem ser tipicamente executadas como uma única chamada de função.</span><span class="sxs-lookup"><span data-stu-id="1d631-268">The following steps are part of standard validation logic in JWT token libraries and can typically be executed as a single function call.</span></span> 
    - <span data-ttu-id="1d631-269">Valide a “audiência” no token que corresponde à ID do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1d631-269">Validate the "audience" in the token matches your app ID.</span></span>
    - <span data-ttu-id="1d631-270">Se você tiver mais de um aplicativo recebendo notificações de alteração, verifique se há várias IDs.</span><span class="sxs-lookup"><span data-stu-id="1d631-270">If you have more than one app receiving change notifications, make sure to check for multiple IDs.</span></span>


4. <span data-ttu-id="1d631-271">**Crítico**: valide se o aplicativo que gerou o token representa o distribuidor de notificação de alteração do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1d631-271">**Critical**: Validate that the app that generated the token represents the Microsoft Graph change notification publisher.</span></span> 

    - <span data-ttu-id="1d631-272">Verifique se a propriedade **appid** no token corresponde ao valor esperado de `0bf30f3b-4a52-48df-9a82-234910c4a086`.</span><span class="sxs-lookup"><span data-stu-id="1d631-272">Check that the **appid** property in the token matches the expected value of `0bf30f3b-4a52-48df-9a82-234910c4a086`.</span></span>
    - <span data-ttu-id="1d631-273">Isso garante que as notificações de alteração não sejam enviadas por um aplicativo diferente que não seja o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1d631-273">This ensures that change notifications are not sent by a different app that is not Microsoft Graph.</span></span>


### <a name="example-jwt-token"></a><span data-ttu-id="1d631-274">Exemplo de Token JWT </span><span class="sxs-lookup"><span data-stu-id="1d631-274">Example JWT token</span></span>

<span data-ttu-id="1d631-275">Veja a seguir um exemplo das propriedades incluídas no token JWT necessárias para a validação.</span><span class="sxs-lookup"><span data-stu-id="1d631-275">The following is an example of the properties included in the JWT token that are needed for validation.</span></span>

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

### <a name="example-verifying-validation-tokens"></a><span data-ttu-id="1d631-276">Exemplo: verificação de tokens de validação</span><span class="sxs-lookup"><span data-stu-id="1d631-276">Example: Verifying validation tokens</span></span>

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
<span data-ttu-id="1d631-277">Para que o exemplo do Java funcione, também será necessário implementar o `JwkKeyResolver`.</span><span class="sxs-lookup"><span data-stu-id="1d631-277">For the Java sample to work, you will also need to implement the `JwkKeyResolver`.</span></span>  
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

## <a name="decrypting-resource-data-from-change-notifications"></a><span data-ttu-id="1d631-278">Descriptografar os dados de recursos de notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="1d631-278">Decrypting resource data from change notifications</span></span>

<span data-ttu-id="1d631-279">A propriedade **resourceData** de uma notificação de alteração inclui somente a ID básica e informações de tipo de uma instância de recurso.</span><span class="sxs-lookup"><span data-stu-id="1d631-279">The **resourceData** property of a change notification includes only the basic ID and type information of a resource instance.</span></span> <span data-ttu-id="1d631-280">A propriedade **encryptedData** contém os dados de recursos completos, criptografados pelo Microsoft Graph usando a chave pública fornecida na assinatura.</span><span class="sxs-lookup"><span data-stu-id="1d631-280">The **encryptedData** property contains the full resource data, encrypted by Microsoft Graph using the public key provided in the subscription.</span></span> <span data-ttu-id="1d631-281">A propriedade também contém valores necessários para verificação e descriptografia.</span><span class="sxs-lookup"><span data-stu-id="1d631-281">The property also contains values required for verification and decryption.</span></span> <span data-ttu-id="1d631-282">Isso é feito para aumentar a segurança dos dados do cliente acessados por meio de notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="1d631-282">This is done to increase the security of customer data accessed via change notifications.</span></span> <span data-ttu-id="1d631-283">É sua responsabilidade proteger a chave privada para garantir que os dados do cliente não possam ser descriptografados por terceiros, mesmo que eles sejam gerenciados para interceptar as notificações de alteração originais.</span><span class="sxs-lookup"><span data-stu-id="1d631-283">It is your responsibility to secure the private key to ensure that customer data cannot be decrypted by a third party, even if they manage to intercept the original change notifications.</span></span>

<span data-ttu-id="1d631-284">Nesta seção:</span><span class="sxs-lookup"><span data-stu-id="1d631-284">In this section:</span></span>

- [<span data-ttu-id="1d631-285">Gerenciar as chaves de criptografia</span><span class="sxs-lookup"><span data-stu-id="1d631-285">Managing encryption keys</span></span>](#managing-encryption-keys)
- [<span data-ttu-id="1d631-286">Descriptografar os dados de recursos</span><span class="sxs-lookup"><span data-stu-id="1d631-286">Decrypting resource data</span></span>](#decrypting-resource-data)
- [<span data-ttu-id="1d631-287">Exemplo: descriptografar uma notificação com dados de recursos criptografados</span><span class="sxs-lookup"><span data-stu-id="1d631-287">Example: decrypting a notification with encrypted resource data</span></span>](#example-decrypting-a-notification-with-encrypted-resource-data)

### <a name="managing-encryption-keys"></a><span data-ttu-id="1d631-288">Gerenciar as chaves de criptografia</span><span class="sxs-lookup"><span data-stu-id="1d631-288">Managing encryption keys</span></span>

1. <span data-ttu-id="1d631-289">Obtenha um certificado com um par de chaves assimétricas.</span><span class="sxs-lookup"><span data-stu-id="1d631-289">Obtain a certificate with a pair of asymmetric keys.</span></span>

    - <span data-ttu-id="1d631-290">Você pode assinatura o certificado sozinho, uma vez que o Microsoft Graph não verifica o emissor do certificado e usa a chave pública somente para criptografia.</span><span class="sxs-lookup"><span data-stu-id="1d631-290">You can self-sign the certificate, since Microsoft Graph does not verify the certificate issuer, and uses the public key for only encryption.</span></span> 
    - <span data-ttu-id="1d631-291">Use o [Cofre da Chave do Azure](https://docs.microsoft.com/azure/key-vault/key-vault-whatis) como a solução para criar, girar e gerenciar certificados com segurança.</span><span class="sxs-lookup"><span data-stu-id="1d631-291">Use [Azure Key Vault](https://docs.microsoft.com/azure/key-vault/key-vault-whatis) as the solution to create, rotate, and securely manage certificates.</span></span> <span data-ttu-id="1d631-292">Cerifique-se de que as chaves atendem aos seguintes critérios:</span><span class="sxs-lookup"><span data-stu-id="1d631-292">Make sure the keys satisfy the following criteria:</span></span>

        - <span data-ttu-id="1d631-293">A chave deve ser do tipo `RSA`</span><span class="sxs-lookup"><span data-stu-id="1d631-293">The key must be of type `RSA`</span></span>
        - <span data-ttu-id="1d631-294">O tamanho da chave deve estar entre 2048 e 4096 bits</span><span class="sxs-lookup"><span data-stu-id="1d631-294">The key size must be between 2048 and 4096 bits</span></span>

2. <span data-ttu-id="1d631-295">Exportar o certificar no formato base64-encoded X.509 e **incluir apenas a chave pública**.</span><span class="sxs-lookup"><span data-stu-id="1d631-295">Export the certificate in base64-encoded X.509 format, and **include only the public key**.</span></span> 

3. <span data-ttu-id="1d631-296">Ao criar uma assinatura:</span><span class="sxs-lookup"><span data-stu-id="1d631-296">When creating a subscription:</span></span>

    - <span data-ttu-id="1d631-297">Forneça o certificado na propriedade **encryptionCertificate** usando o conteúdo base64-encoded no qual o certificado foi exportado.</span><span class="sxs-lookup"><span data-stu-id="1d631-297">Provide the certificate in the **encryptionCertificate** property, using the base64-encoded content that the certificate was exported in.</span></span>
    - <span data-ttu-id="1d631-298">Forneça seu próprio identificador na propriedade **encryptionCertificateId**.</span><span class="sxs-lookup"><span data-stu-id="1d631-298">Provide your own identifier in the **encryptionCertificateId** property.</span></span> 
  
        <span data-ttu-id="1d631-299">Esse identificador permite que você corresponda seus certificados às notificações de alteração recebidas e recupere certificados do repositório de certificados.</span><span class="sxs-lookup"><span data-stu-id="1d631-299">This identifier allows you to match your certificates to the change notifications you receive, and to retrieve certificates from your certificate store.</span></span> <span data-ttu-id="1d631-300">O identificador pode ter no máximo 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="1d631-300">The identifier can be up to 128 characters.</span></span>

4. <span data-ttu-id="1d631-301">Gerencie a chave privada com segurança para que seu código de processamento de notificação de alteração possa acessar a chave privada para descriptografar dados de recurso.</span><span class="sxs-lookup"><span data-stu-id="1d631-301">Manage the private key securely, so that your change notification processing code can access the private key to decrypt resource data.</span></span>

#### <a name="rotating-keys"></a><span data-ttu-id="1d631-302">Chaves de rotação</span><span class="sxs-lookup"><span data-stu-id="1d631-302">Rotating keys</span></span>

<span data-ttu-id="1d631-303">Para minimizar o risco de uma chave privada ser comprometida, altere periodicamente suas chaves assimétricas.</span><span class="sxs-lookup"><span data-stu-id="1d631-303">To minimize the risk of a private key becoming compromised, periodically change your asymmetric keys.</span></span> <span data-ttu-id="1d631-304">Siga estas etapas para introduzir um novo par de chaves:</span><span class="sxs-lookup"><span data-stu-id="1d631-304">Follow these steps to introduce a new pair of keys:</span></span>

1. <span data-ttu-id="1d631-305">Obtenha um novo certificado com um novo par de chaves assimétricas.</span><span class="sxs-lookup"><span data-stu-id="1d631-305">Obtain a new certificate with a new pair of asymmetric keys.</span></span> <span data-ttu-id="1d631-306">Use-o para todas as novas assinaturas sendo criadas.</span><span class="sxs-lookup"><span data-stu-id="1d631-306">Use it for all new subscriptions being created.</span></span>

2. <span data-ttu-id="1d631-307">Atualize as assinaturas existentes com a nova chave de certificado.</span><span class="sxs-lookup"><span data-stu-id="1d631-307">Update existing subscriptions with the new certificate key.</span></span>

    - <span data-ttu-id="1d631-308">Faça isso como parte da renovação da assinatura regular.</span><span class="sxs-lookup"><span data-stu-id="1d631-308">Do this as part of regular subscription renewal.</span></span> 
    - <span data-ttu-id="1d631-309">Ou enumere todas as assinaturas e forneça a chave.</span><span class="sxs-lookup"><span data-stu-id="1d631-309">Or, enumerate all subscriptions and provide the key.</span></span> <span data-ttu-id="1d631-310">Use a [operação PATCH na assinatura](/graph/api/subscription-update?view=graph-rest-1.0) e atualize as propriedades **encryptionCertificate** e **encryptionCertificateId**.</span><span class="sxs-lookup"><span data-stu-id="1d631-310">Use the [PATCH operation on the subscription](/graph/api/subscription-update?view=graph-rest-1.0) and update the **encryptionCertificate** and **encryptionCertificateId** properties.</span></span>

3. <span data-ttu-id="1d631-311">Lembre-se do seguinte:</span><span class="sxs-lookup"><span data-stu-id="1d631-311">Keep in mind the following:</span></span>
    - <span data-ttu-id="1d631-312">Por um período de tempo, o certificado antigo ainda pode ser usado para criptografia.</span><span class="sxs-lookup"><span data-stu-id="1d631-312">For a period of time, the old certificate may still be used for encryption.</span></span> <span data-ttu-id="1d631-313">Seu aplicativo deve ter acesso a certificados novos e antigos para poder descriptografar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="1d631-313">Your app must have access to both old and new certificates to be able to decrypt content.</span></span>
    - <span data-ttu-id="1d631-314">Use a propriedade **encryptionCertificateId** em cada notificação de alteração para identificar a chave correta a ser usada.</span><span class="sxs-lookup"><span data-stu-id="1d631-314">Use the **encryptionCertificateId** property in each change notification to identify the correct key to use.</span></span>
    - <span data-ttu-id="1d631-315">Descarte do certificado antigo somente quando não tiver visto nenhuma notificação de alteração recente fazendo referência a ele.</span><span class="sxs-lookup"><span data-stu-id="1d631-315">Discard of the old certificate only when you have seen no recent change notifications referencing it.</span></span>

### <a name="decrypting-resource-data"></a><span data-ttu-id="1d631-316">Descriptografar dados de recursos</span><span class="sxs-lookup"><span data-stu-id="1d631-316">Decrypting resource data</span></span>

<span data-ttu-id="1d631-317">Para otimizar o desempenho, o Microsoft Graph usa um processo de criptografia de duas etapas:</span><span class="sxs-lookup"><span data-stu-id="1d631-317">To optimize performance, Microsoft Graph uses a two-step encryption process:</span></span>
  - <span data-ttu-id="1d631-318">Ele gera uma chave simétrica de uso único e a usa para criptografar os dados do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d631-318">It generates a single use symmetric key, and uses it to encrypt resource data.</span></span>
  - <span data-ttu-id="1d631-319">Ele usa a chave assimétrica pública (que você forneceu ao inscrever-se) para criptografar a chave simétrica e a inclui em cada notificação de alteração dessa assinatura.</span><span class="sxs-lookup"><span data-stu-id="1d631-319">It uses the public asymmetric key (that you provided when subscribing) to encrypt the symmetric key and includes it in each change notification of that subscription.</span></span>

<span data-ttu-id="1d631-320">Considere sempre que a chave simétrica é diferente para cada item na notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="1d631-320">Always assume that the symmetric key is different for each item in the change notification.</span></span>

<span data-ttu-id="1d631-321">Para descriptografar dados de recurso, seu aplicativo deve executar as etapas inversas usando as propriedades em **encryptedContent** em cada notificação de alteração:</span><span class="sxs-lookup"><span data-stu-id="1d631-321">To decrypt resource data, your app should perform the reverse steps, using the properties under **encryptedContent** in each change notification:</span></span>

1. <span data-ttu-id="1d631-322">Use a propriedade **encryptionCertificateId** para identificar o certificado a ser usado.</span><span class="sxs-lookup"><span data-stu-id="1d631-322">Use the **encryptionCertificateId** property to identify the certificate to use.</span></span>

2. <span data-ttu-id="1d631-323">Inicialize um componente criptográfico da RSA (como o .NET [RSACryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) com a chave privada.</span><span class="sxs-lookup"><span data-stu-id="1d631-323">Initialize an RSA cryptographic component (such as the .NET [RSACryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) with the private key.</span></span>

3. <span data-ttu-id="1d631-324">Descriptografe a chave simétrica entregue na propriedade **dataKey** de cada item na notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="1d631-324">Decrypt the symmetric key delivered in the **dataKey** property of each item in the change notification.</span></span>

    <span data-ttu-id="1d631-325">Use o Preenchimento de Criptografia Assimétrica Ideal (OAEP) para o algoritmo de descriptografia.</span><span class="sxs-lookup"><span data-stu-id="1d631-325">Use Optimal Asymmetric Encryption Padding (OAEP) for the decryption algorithm.</span></span>

4. <span data-ttu-id="1d631-326">Use a chave simétrica para calcular a assinatura HMAC-SHA256 do valor em **dados**.</span><span class="sxs-lookup"><span data-stu-id="1d631-326">Use the symmetric key to calculate the HMAC-SHA256 signature of the value in **data**.</span></span>
  
    <span data-ttu-id="1d631-327">Compare-o com o valor em **dataSignature**.</span><span class="sxs-lookup"><span data-stu-id="1d631-327">Compare it to the value in **dataSignature**.</span></span> <span data-ttu-id="1d631-328">Se eles não corresponderem, considere que a carga foi adulterada e não a descriptografe.</span><span class="sxs-lookup"><span data-stu-id="1d631-328">If they do not match, assume the payload has been tampered with and do not decrypt it.</span></span>

5. <span data-ttu-id="1d631-329">Use a chave simétrica com a criptografia AES (como o .NET [AesCryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) para descriptografar o conteúdo em **dados**.</span><span class="sxs-lookup"><span data-stu-id="1d631-329">Use the symmetric key with an Advanced Encryption Standard (AES) (such as the .NET [AesCryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) to decrypt the content in **data**.</span></span>

    - <span data-ttu-id="1d631-330">Use os seguintes parâmetros de descriptografia para o algoritmo AES:</span><span class="sxs-lookup"><span data-stu-id="1d631-330">Use the following decryption parameters for the AES algorithm:</span></span>

        - <span data-ttu-id="1d631-331">Preenchimento: PKCS7</span><span class="sxs-lookup"><span data-stu-id="1d631-331">Padding: PKCS7</span></span>
        - <span data-ttu-id="1d631-332">Modo de criptografia: CBC</span><span class="sxs-lookup"><span data-stu-id="1d631-332">Cipher mode: CBC</span></span>
    - <span data-ttu-id="1d631-333">Defina o “vetor de inicialização” copiando os primeiros 16 bytes da chave simétrica usada para descriptografia.</span><span class="sxs-lookup"><span data-stu-id="1d631-333">Set the "initialization vector" by copying the first 16 bytes of the symmetric key used for decryption.</span></span>

6. <span data-ttu-id="1d631-334">O valor descriptografado é uma cadeia de caracteres JSON que representa a instância de recurso na notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="1d631-334">The decrypted value is a JSON string that represents the resource instance in the change notification.</span></span>


### <a name="example-decrypting-a-notification-with-encrypted-resource-data"></a><span data-ttu-id="1d631-335">Exemplo: descriptografar uma notificação com dados de recurso criptografados</span><span class="sxs-lookup"><span data-stu-id="1d631-335">Example: decrypting a notification with encrypted resource data</span></span>

<span data-ttu-id="1d631-336">A seguir está um exemplo de notificação de alteração que inclui valores de propriedade criptografados de uma instância do **chat** em uma mensagem de canal.</span><span class="sxs-lookup"><span data-stu-id="1d631-336">The following is an example change notification that includes encrypted property values of a **chatMessage** instance in a channel message.</span></span> <span data-ttu-id="1d631-337">A instância é especificada pelo valor `@odata.id`.</span><span class="sxs-lookup"><span data-stu-id="1d631-337">The instance is specified by the `@odata.id` value.</span></span>

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

> <span data-ttu-id="1d631-338">**Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração são entregues, consulte [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="1d631-338">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>


<span data-ttu-id="1d631-339">A seção contém alguns trechos de código úteis que usam C# e .NET em cada etapa da descriptografia.</span><span class="sxs-lookup"><span data-stu-id="1d631-339">This section contains some useful code snippets that use C# and .NET for each stage of decryption.</span></span>

#### <a name="decrypt-the-symmetric-key"></a><span data-ttu-id="1d631-340">Descriptografar a chave simétrica</span><span class="sxs-lookup"><span data-stu-id="1d631-340">Decrypt the symmetric key</span></span>

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

#### <a name="compare-data-signature-using-hmac-sha256"></a><span data-ttu-id="1d631-341">Comparar assinatura de dados usando HMAC-SHA256</span><span class="sxs-lookup"><span data-stu-id="1d631-341">Compare data signature using HMAC-SHA256</span></span>

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

#### <a name="decrypt-the-resource-data-content"></a><span data-ttu-id="1d631-342">Descriptografar o conteúdo dos dados de recursos</span><span class="sxs-lookup"><span data-stu-id="1d631-342">Decrypt the resource data content</span></span>

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

## <a name="see-also"></a><span data-ttu-id="1d631-343">Confira também</span><span class="sxs-lookup"><span data-stu-id="1d631-343">See also</span></span>

- [<span data-ttu-id="1d631-344">Configurar notificações para alterações nos dados de usuário</span><span class="sxs-lookup"><span data-stu-id="1d631-344">Set up notifications for changes in user data</span></span>](webhooks.md)
- [<span data-ttu-id="1d631-345">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="1d631-345">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-beta)
- [<span data-ttu-id="1d631-346">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="1d631-346">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="1d631-347">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="1d631-347">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="1d631-348">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="1d631-348">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
