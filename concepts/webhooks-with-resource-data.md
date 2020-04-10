---
title: Configurar notificações de alteração que incluam dados de recursos (visualização)
description: O Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. As notificações podem incluir propriedades do recurso.
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.openlocfilehash: 41cf03e94bef399142135c899d812820651338b7
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200212"
---
# <a name="set-up-change-notifications-that-include-resource-data-preview"></a><span data-ttu-id="cec80-104">Configurar notificações de alteração que incluam dados de recursos (visualização)</span><span class="sxs-lookup"><span data-stu-id="cec80-104">Set up change notifications that include resource data (preview)</span></span>

<span data-ttu-id="cec80-105">O Microsoft Graph permite que os aplicativos inscrevam-se para alterar as notificações de recursos através do [webhooks](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="cec80-105">Microsoft Graph allows apps to subscribe to change notifications for resources via [webhooks](webhooks.md).</span></span> <span data-ttu-id="cec80-106">Agora você pode configurar assinaturas para incluir os dados de recursos alterados (como o conteúdo de uma mensagem de bate-papo do Microsoft Teams) em notificações.</span><span class="sxs-lookup"><span data-stu-id="cec80-106">You can now set up subscriptions to include the changed resource data (such as the content of a Microsoft Teams chat message) in notifications.</span></span> <span data-ttu-id="cec80-107">Em seguida, seu aplicativo pode usar a lógica de negócios sem ter que fazer uma chamada à API separada para buscar o recurso alterado.</span><span class="sxs-lookup"><span data-stu-id="cec80-107">Your app can then run its business logic without having to make a separate API call to fetch the changed resource.</span></span> <span data-ttu-id="cec80-108">Como resultado, o aplicativo funciona melhor ao realizar menos chamadas da API, o que é benéfico em cenários de larga escala.</span><span class="sxs-lookup"><span data-stu-id="cec80-108">As a result, the app performs better by making fewer API calls, which is beneficial in large scale scenarios.</span></span>

<span data-ttu-id="cec80-109">Incluir dados de recursos como parte de notificações exige que você implemente a seguinte lógica adicional para atender aos requisitos de acesso e segurança de dados:</span><span class="sxs-lookup"><span data-stu-id="cec80-109">Including resource data as part of notifications requires you to implement the following additional logic to satisfy data access and security requirements:</span></span> 

- <span data-ttu-id="cec80-110">[Lidar com](#subscription-life-cycle-notifications) as notificações do _ciclo de vida_ de assinatura especial para manter um fluxo ininterrupto de dados.</span><span class="sxs-lookup"><span data-stu-id="cec80-110">[Handle](#subscription-life-cycle-notifications) special subscription _life cycle_ notifications to maintain an uninterrupted flow of data.</span></span> <span data-ttu-id="cec80-111">O Microsoft Graph envia notificações do ciclo de vida de vez em quando para exigir que um aplicativo seja autorizado novamente, para garantir que os problemas de acesso não tenham sido cortados inesperadamente para incluir dados de recursos em notificações.</span><span class="sxs-lookup"><span data-stu-id="cec80-111">Microsoft Graph sends life cycle notifications from time to time to require an app to re-authorize, to make sure access issues have not unexpectedly cropped up for including resource data in notifications.</span></span>
- <span data-ttu-id="cec80-112">[Valide](#validating-the-authenticity-of-notifications) a autenticidade das notificações como tendo sido originadas no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cec80-112">[Validate](#validating-the-authenticity-of-notifications) the authenticity of notifications as having originated from Microsoft Graph.</span></span>
- <span data-ttu-id="cec80-113">[Forneça](#decrypting-resource-data-from-change-notifications) uma chave de criptografia pública e use uma chave privada para descriptografar os dados de recursos recebidos através de notificações.</span><span class="sxs-lookup"><span data-stu-id="cec80-113">[Provide](#decrypting-resource-data-from-change-notifications) a public encryption key and use a private key to decrypt resource data received through notifications.</span></span>

## <a name="resource-data-in-notification-payload"></a><span data-ttu-id="cec80-114">Dados de recursos na carga de notificação </span><span class="sxs-lookup"><span data-stu-id="cec80-114">Resource data in notification payload</span></span>

<span data-ttu-id="cec80-115">Geralmente, esse tipo de notificação de alteração inclui os seguintes dados de recursos na carga:</span><span class="sxs-lookup"><span data-stu-id="cec80-115">In general, this type of change notifications include the following resource data in the payload:</span></span>

- <span data-ttu-id="cec80-116">ID e tipo de instância de recurso alterado, retornados na propriedade **resourceData**.</span><span class="sxs-lookup"><span data-stu-id="cec80-116">ID and type of the changed resource instance, returned in the **resourceData** property.</span></span>
- <span data-ttu-id="cec80-117">Todos os valores de propriedade da instância de recurso, criptografados conforme especificado na assinatura, retornados na propriedade **encryptedContent**.</span><span class="sxs-lookup"><span data-stu-id="cec80-117">All the property values of that resource instance, encrypted as specified in the subscription, returned in the **encryptedContent** property.</span></span>
- <span data-ttu-id="cec80-118">Or, dependendo do recurso, propriedades específicas retornadas na propriedade **resourceData**.</span><span class="sxs-lookup"><span data-stu-id="cec80-118">Or, depending on the resource, specific properties returned in the **resourceData** property.</span></span> <span data-ttu-id="cec80-119">Para obter somente propriedades específicas, especifique-as como parte da URL do **recurso** na assinatura, usando um parâmetro `$select`.</span><span class="sxs-lookup"><span data-stu-id="cec80-119">To get only specific properties, specify them as part of the **resource** URL in the subscription, using a `$select` parameter.</span></span>  


## <a name="supported-resources"></a><span data-ttu-id="cec80-120">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="cec80-120">Supported resources</span></span>

<span data-ttu-id="cec80-121">Atualmente, o recurso [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) (visualização) do Microsoft Teams oferece suporte a notificações de alteração que incluem dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="cec80-121">Currently, the Microsoft Teams [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) (preview) resource supports change notifications that include resource data.</span></span> <span data-ttu-id="cec80-122">Especificamente, você pode configurar uma assinatura que se aplique a uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="cec80-122">Specifically, you can set up a subscription that applies to one of the following:</span></span>

- <span data-ttu-id="cec80-123">Mensagens novas ou alteradas em um canal específico do Teams: `/teams/{id}/channels/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="cec80-123">New or changed messages in a specific Teams channel: `/teams/{id}/channels/{id}/messages`</span></span>
- <span data-ttu-id="cec80-124">Mensagens novas ou alteradas em um bate-papo específico do Teams: `/chats/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="cec80-124">New or changed messages in a specific Teams chat: `/chats/{id}/messages`</span></span>

<span data-ttu-id="cec80-125">O recurso **chatMessage** permite incluir todas as propriedades de uma instância alterada em uma notificação.</span><span class="sxs-lookup"><span data-stu-id="cec80-125">The **chatMessage** resource supports including all the properties of a changed instance in a notification.</span></span> <span data-ttu-id="cec80-126">Não há suporte para retornar apenas propriedades seletivas da instância.</span><span class="sxs-lookup"><span data-stu-id="cec80-126">It does not support returning only selective properties of the instance.</span></span> 

<span data-ttu-id="cec80-127">Este artigo mostra um exemplo de assinatura de alteração de notificações de mensagens em um canal do Teams, com cada notificação incluindo os dados de recursos totais da instância alterada **chatMessage**.</span><span class="sxs-lookup"><span data-stu-id="cec80-127">This article walks through an example of subscribing to change notifications of messages in a Teams channel, with each notification including the full resource data of the changed **chatMessage** instance.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="cec80-128">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="cec80-128">Creating a subscription</span></span>

<span data-ttu-id="cec80-129">Para que os dados de recursos estejam incluídos nas notificações de alteração, você **deve** especificar as seguintes propriedades, além das que geralmente são especificadas ao [criar uma assinatura](webhooks.md#creating-a-subscription):</span><span class="sxs-lookup"><span data-stu-id="cec80-129">To have resource data included in change notifications, you **must** specify the following properties, in addition to those that are usually specified when [creating a subscription](webhooks.md#creating-a-subscription):</span></span>

- <span data-ttu-id="cec80-130">**includeResourceData** que deve ser definido como `true` para solicitar explicitamente os dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="cec80-130">**includeResourceData** which should be set to `true` to explicitly request resource data.</span></span>
- <span data-ttu-id="cec80-131">**lifecycleNotificationUrl** é um ponto de extremidade onde as [notificações do ciclo de vida](#subscription-life-cycle-notifications) são fornecidas.</span><span class="sxs-lookup"><span data-stu-id="cec80-131">**lifecycleNotificationUrl** which is an endpoint where [life cycle notifications](#subscription-life-cycle-notifications) are delivered.</span></span> <span data-ttu-id="cec80-132">Pode ser igual ou diferente de **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="cec80-132">This can be the same or different as **notificationUrl**.</span></span>
- <span data-ttu-id="cec80-133">**encryptionCertificate** que contém apenas a chave público que o Microsoft Graph usa para criptografar os dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="cec80-133">**encryptionCertificate** which contains only the public key that Microsoft Graph uses to encrypt resource data.</span></span> <span data-ttu-id="cec80-134">Mantenha a chave privada correspondente para [descriptografar o conteúdo](#decrypting-resource-data-from-change-notifications).</span><span class="sxs-lookup"><span data-stu-id="cec80-134">Keep the corresponding private key to [decrypt the content](#decrypting-resource-data-from-change-notifications).</span></span>
- <span data-ttu-id="cec80-135">**encryptionCertificateId** é o seu próprio identificador para o certificado.</span><span class="sxs-lookup"><span data-stu-id="cec80-135">**encryptionCertificateId** which is your own identifier for the certificate.</span></span> <span data-ttu-id="cec80-136">Use essa ID para corresponder a cada notificação, qual certificado usar para descriptografia.</span><span class="sxs-lookup"><span data-stu-id="cec80-136">Use this ID to match in each notification, which certificate to use for decryption.</span></span>

<span data-ttu-id="cec80-137">Lembre-se do seguinte:</span><span class="sxs-lookup"><span data-stu-id="cec80-137">Keep the following in mind:</span></span>

- <span data-ttu-id="cec80-138">Use o mesmo nome de host para os pontos de extremidade de notificação (**notificationUrl** e **lifecycleNotificationUrl**).</span><span class="sxs-lookup"><span data-stu-id="cec80-138">Use the same host name for both notification endpoints (**notificationUrl** and **lifecycleNotificationUrl**).</span></span>
- <span data-ttu-id="cec80-139">Valide os dois pontos de extremidade de notificação conforme descrito [aqui](webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="cec80-139">Validate both notification endpoints as described [here](webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="cec80-140">Se você quiser usar a mesma URL para os dois pontos de extremidade, você receberá e responderá a duas solicitações de validação.</span><span class="sxs-lookup"><span data-stu-id="cec80-140">If you choose to use the same URL for both endpoints, you will receive and respond to two validation requests.</span></span>
- <span data-ttu-id="cec80-141">Não é possível atualizar (`PATCH`) uma assinatura existente para adicionar a propriedade **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="cec80-141">You cannot update (`PATCH`) an existing subscription to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="cec80-142">Você deve remover a assinatura existente e criar uma nova assinatura para incluir a propriedade **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="cec80-142">You should remove the existing subscription, and create a new subscription to include the **lifecycleNotificationUrl** property.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="cec80-143">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="cec80-143">Subscription request example</span></span>

<span data-ttu-id="cec80-144">O exemplo a seguir assina dois tipos de notificações:</span><span class="sxs-lookup"><span data-stu-id="cec80-144">The following example subscribes to two types of notifications:</span></span> 

- <span data-ttu-id="cec80-145">Alterações de recursos - canais de mensagens sendo criados ou atualizados no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="cec80-145">Resource changes - channel messages being created or updated in Microsoft Teams</span></span>
- <span data-ttu-id="cec80-146">Eventos do ciclo de vida da assinatura que podem afetar o fluxo das notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="cec80-146">Subscription life cycle events which can affect the flow of change notifications.</span></span> <span data-ttu-id="cec80-147">Veja mais detalhes sobre as notificações do ciclo de vida na [próxima seção](#subscription-life-cycle-notifications).</span><span class="sxs-lookup"><span data-stu-id="cec80-147">See more details about life cycle notifications in the [next section](#subscription-life-cycle-notifications).</span></span>

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

### <a name="subscription-response"></a><span data-ttu-id="cec80-148">Resposta de assinatura</span><span class="sxs-lookup"><span data-stu-id="cec80-148">Subscription response</span></span>
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

## <a name="subscription-life-cycle-notifications"></a><span data-ttu-id="cec80-149">Notificações do ciclo de vida da assinatura</span><span class="sxs-lookup"><span data-stu-id="cec80-149">Subscription life cycle notifications</span></span>

<span data-ttu-id="cec80-150">Determinados eventos podem interferir no fluxo de notificação normal de uma assinatura existente.</span><span class="sxs-lookup"><span data-stu-id="cec80-150">Certain events can interfere with normal notification flow in an existing subscription.</span></span> <span data-ttu-id="cec80-151">As _notificações do ciclo de vida_ da assinatura informam as ações necessárias para manter um fluxo ininterrupto.</span><span class="sxs-lookup"><span data-stu-id="cec80-151">Subscription _life cycle notifications_ inform you actions to take in order to maintain an uninterrupted flow.</span></span> <span data-ttu-id="cec80-152">Ao contrário de uma notificação de alteração de recurso que informa uma alteração a uma instância de recurso, uma notificação do ciclo de vida trata-se da própria assinatura e seu estado atual no ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="cec80-152">Unlike a resource change notification which informs a change to a resource instance, a life cycle notification is about the subscription itself, and its current state in the life cycle.</span></span> 

<span data-ttu-id="cec80-153">As notificações do ciclo de vida são fornecidas a **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="cec80-153">Life cycle notifications are delivered to the **lifecycleNotificationUrl**.</span></span> 

<span data-ttu-id="cec80-154">Nesta seção:</span><span class="sxs-lookup"><span data-stu-id="cec80-154">In this section:</span></span>

- [<span data-ttu-id="cec80-155">Notificação do ciclo de vida que desafia a autorização de assinatura</span><span class="sxs-lookup"><span data-stu-id="cec80-155">Life cycle notification that challenges subscription authorization</span></span>](#life-cycle-notification-that-challenges-subscription-authorization)
- [<span data-ttu-id="cec80-156">Fluxo de desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="cec80-156">Authorization challenge flow</span></span>](#authorization-challenge-flow)
- [<span data-ttu-id="cec80-157">Exemplo de desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="cec80-157">Example authorization challenge</span></span>](#example-authorization-challenge)
- [<span data-ttu-id="cec80-158">Respondendo a um desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="cec80-158">Responding to an authorization challenge</span></span>](#responding-to-an-authorization-challenge)
- [<span data-ttu-id="cec80-159">Dicas</span><span class="sxs-lookup"><span data-stu-id="cec80-159">Tips</span></span>](#tips)
- [<span data-ttu-id="cec80-160">Proteja o seu código para lidar com outros tipos de notificações do ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="cec80-160">Future-proof your code to handle other types of life cycle notifications</span></span>](#future-proof-your-code-to-handle-other-types-of-life-cycle-notifications)

### <a name="life-cycle-notification-that-challenges-subscription-authorization"></a><span data-ttu-id="cec80-161">Notificação do ciclo de vida que desafia a autorização de assinatura </span><span class="sxs-lookup"><span data-stu-id="cec80-161">Life cycle notification that challenges subscription authorization</span></span>

<span data-ttu-id="cec80-162">Um tipo de notificações do ciclo de vida desafia o estado autorizado de uma assinatura ativa.</span><span class="sxs-lookup"><span data-stu-id="cec80-162">One type of life cycle notifications challenges the authorized state of an active subscription.</span></span> <span data-ttu-id="cec80-163">Quando a propriedade **lifecycleEvent** em uma notificação indica `reauthorizationRequired`, você deve autorizar novamente a assinatura para manter o fluxo de dados.</span><span class="sxs-lookup"><span data-stu-id="cec80-163">When the **lifecycleEvent** property in a notification indicates `reauthorizationRequired`, you must re-authorize the subscription to maintain the data flow.</span></span>

<span data-ttu-id="cec80-164">Quando você cria uma assinatura de vida longa (por exemplo, uma que dura três dias), as notificações de dados de recursos fluem para o local indicado em **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="cec80-164">When you create a long-lived subscription (for example, one that lasts for 3 days), resource data notifications flows to the location indicated in **notificationUrl**.</span></span> <span data-ttu-id="cec80-165">Entretanto, a qualquer momento, o Microsoft Graph pode exigir que você autorize novamente a assinatura para provar que ainda tem acesso aos dados de recursos, caso as condições de acesso tenham sido alteradas desde a criação da assinatura.</span><span class="sxs-lookup"><span data-stu-id="cec80-165">However, at any point in time, Microsoft Graph may require that you re-authorize the subscription to prove that you still have access to resource data, in case the conditions of access have changed since the subscription was created.</span></span> <span data-ttu-id="cec80-166">A seguir estão exemplos de alterações que afetam o acesso aos dados:</span><span class="sxs-lookup"><span data-stu-id="cec80-166">The following are examples of changes that affect your access to data:</span></span>

- <span data-ttu-id="cec80-167">Um administrador de locatários pode revogar as permissões do seu aplicativo para ler um recurso.</span><span class="sxs-lookup"><span data-stu-id="cec80-167">A tenant administrator may revoke your app's permissions to read a resource.</span></span>
- <span data-ttu-id="cec80-168">Em um cenário interativo, o usuário que fornece o token de autenticação ao seu aplicativo pode estar sujeito a políticas dinâmicas com base em vários fatores, como o local, o estado do dispositivo ou a avaliação de risco.</span><span class="sxs-lookup"><span data-stu-id="cec80-168">In an interactive scenario, the user who provides the authentication token to your app may be subject to dynamic policies based on various factors, such as their location, device state, or risk assesment.</span></span> <span data-ttu-id="cec80-169">Por exemplo, se o usuário alterar o seu local físico, pode ser que ele não tenha mais permissão para acessar os dados e seu aplicativo não conseguirá autorizar novamente a assinatura.</span><span class="sxs-lookup"><span data-stu-id="cec80-169">For example, if the user changes their physical location, the user may no longer be allowed to access the data, and your app will not be able to re-authorize the subscription.</span></span> <span data-ttu-id="cec80-170">Para saber mais sobre políticas dinâmicas que controlam o acesso, confira [políticas de acesso condicional do Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/overview).</span><span class="sxs-lookup"><span data-stu-id="cec80-170">For more information on dynamic policies that control access, see [Azure AD conditional access policies](https://docs.microsoft.com/azure/active-directory/conditional-access/overview).</span></span> 

### <a name="authorization-challenge-flow"></a><span data-ttu-id="cec80-171">Fluxo de desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="cec80-171">Authorization challenge flow</span></span>

<span data-ttu-id="cec80-172">O fluxo de um desafio de autorização para uma assinatura ativa e não expirada tem a seguinte aparência:</span><span class="sxs-lookup"><span data-stu-id="cec80-172">The flow of an authorization challenge for an active, non-expired subscription looks as follows:</span></span>

1. <span data-ttu-id="cec80-173">O Microsoft Graph exige que uma assinatura seja autorizada novamente.</span><span class="sxs-lookup"><span data-stu-id="cec80-173">Microsoft Graph requires a subscription to be re-authorized</span></span>
    
    <span data-ttu-id="cec80-174">Os motivos para isso podem variar de recurso para recurso e podem mudar com o tempo.</span><span class="sxs-lookup"><span data-stu-id="cec80-174">The reasons for this may vary from resource to resource, and may change over time.</span></span> <span data-ttu-id="cec80-175">Independentemente da causa do evento de reautorização, você precisará respondê-lo.</span><span class="sxs-lookup"><span data-stu-id="cec80-175">Regardless of the cause of the re-authorization event, you will need to respond to it.</span></span>

2. <span data-ttu-id="cec80-176">O Microsoft Graph envia uma notificação de desafio de autorização para **lifecycleNotificationUrl**</span><span class="sxs-lookup"><span data-stu-id="cec80-176">Microsoft Graph sends an authorization challenge notification to the **lifecycleNotificationUrl**</span></span>

    <span data-ttu-id="cec80-177">Observe que o fluxo de notificações de recursos pode continuar por algum tempo, dando a você mais tempo para responder.</span><span class="sxs-lookup"><span data-stu-id="cec80-177">Note that the flow of resource notifications may continue for a while, giving you extra time to respond.</span></span> <span data-ttu-id="cec80-178">Entretanto, eventualmente a entrega da notificação de recursos será pausada, até que você execute a ação necessária.</span><span class="sxs-lookup"><span data-stu-id="cec80-178">However, eventually resource notification delivery will pause, until you take the required action.</span></span>

3. <span data-ttu-id="cec80-179">Responda a essa notificação de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="cec80-179">Respond to this notification in one of two ways:</span></span>
    1. <span data-ttu-id="cec80-180">Autorize a assinatura novamente.</span><span class="sxs-lookup"><span data-stu-id="cec80-180">Re-authorize the subscription.</span></span> <span data-ttu-id="cec80-181">Isso não estende a data de vencimento da assinatura.</span><span class="sxs-lookup"><span data-stu-id="cec80-181">This does not extend the expiry date of the subscription.</span></span>
    2. <span data-ttu-id="cec80-182">Renove a assinatura.</span><span class="sxs-lookup"><span data-stu-id="cec80-182">Renew the subscription.</span></span> <span data-ttu-id="cec80-183">Isso reautoriza e estenda a data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="cec80-183">This both re-authorizes and extends the expiry date.</span></span>

    <span data-ttu-id="cec80-184">Observação: as duas ações exigem a apresentação de um token de autenticação válido, semelhante a [criar uma nova assinatura](webhooks.md#creating-a-subscription) ou [renova uma assinatura antes da sua expiração](webhooks.md#renewing-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="cec80-184">Note: Both actions require you to present a valid authentication token, similar to [creating a new subscription](webhooks.md#creating-a-subscription) or [renewing a subscription before its expiry](webhooks.md#renewing-a-subscription).</span></span>

4. <span data-ttu-id="cec80-185">Se você conseguir autorizar novamente ou renovar a assinatura, as notificações de recursos continuarão.</span><span class="sxs-lookup"><span data-stu-id="cec80-185">If you successfully re-authorize or renew the subscription, resource notifications continue.</span></span> <span data-ttu-id="cec80-186">Caso contrário, as notificações de recursos permanecem em pausa.</span><span class="sxs-lookup"><span data-stu-id="cec80-186">Otherwise, resource notifications remain paused.</span></span>
    
### <a name="example-authorization-challenge"></a><span data-ttu-id="cec80-187">Exemplo de desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="cec80-187">Example authorization challenge</span></span>

<span data-ttu-id="cec80-188">Veja um exemplo de notificação de ciclo de vida que solicita a reautorização de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="cec80-188">Below is an example life cycle notification that requests re-authorizing a subscription.</span></span> 

<span data-ttu-id="cec80-189">Observe o seguinte:</span><span class="sxs-lookup"><span data-stu-id="cec80-189">Note the following:</span></span>

- <span data-ttu-id="cec80-190">O campo `"lifecycleEvent": "reauthorizationRequired"` identifica essa notificação como um desafio de autorização.</span><span class="sxs-lookup"><span data-stu-id="cec80-190">The `"lifecycleEvent": "reauthorizationRequired"` field identifies this notification as an authorization challenge.</span></span>
- <span data-ttu-id="cec80-191">A notificação não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.</span><span class="sxs-lookup"><span data-stu-id="cec80-191">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="cec80-192">Assim como as notificações de recursos, as notificações do ciclo de vida podem estar em lote juntas (na coleção **valor**), cada uma com valores possivelmente diferentes **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="cec80-192">Similar to resource notifications, you can batch life cycle notifications together (in the **value** collection), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="cec80-193">Processe cada notificação no lote de acordo.</span><span class="sxs-lookup"><span data-stu-id="cec80-193">Process each notification in the batch accordingly.</span></span>

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

### <a name="responding-to-an-authorization-challenge"></a><span data-ttu-id="cec80-194">Respondendo a um desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="cec80-194">Responding to an authorization challenge</span></span>

<span data-ttu-id="cec80-195">Execute as etapas a seguir para processar uma notificação do ciclo de vida de desafio de autorização.</span><span class="sxs-lookup"><span data-stu-id="cec80-195">Take the following steps to process an authorization challenge life cycle notification.</span></span> <span data-ttu-id="cec80-196">As duas primeiras etapas de reconhecimento e validação da notificação do ciclo de vida são semelhantes a [responder a uma notificação de alteração de recursos](webhooks.md#processing-the-notification).</span><span class="sxs-lookup"><span data-stu-id="cec80-196">The first two steps of acknowledging and validating the life cycle notification is similar to [responding to a resource change notification](webhooks.md#processing-the-notification).</span></span>

1. <span data-ttu-id="cec80-197">Aceite o recebimento da notificação respondendo a chamada POSTAGEM com `HTTP 202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="cec80-197">Acknowledge the receipt of the notification, by responding to the POST call with `HTTP 202 Accepted`.</span></span>
2. <span data-ttu-id="cec80-198">Validar a autenticidade da notificação.</span><span class="sxs-lookup"><span data-stu-id="cec80-198">Validate the authenticity of the notification.</span></span> <span data-ttu-id="cec80-199">Mais detalhes [abaixo](#validating-the-authenticity-of-notifications).</span><span class="sxs-lookup"><span data-stu-id="cec80-199">Further details [below](#validating-the-authenticity-of-notifications).</span></span>
3. <span data-ttu-id="cec80-200">Certifique-se de que o aplicativo tenha um token de acesso válido para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="cec80-200">Ensure the app has a valid access token to take the next step.</span></span> 

    <span data-ttu-id="cec80-201">Se você estiver usando uma das [bibliotecas de autenticação](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), a biblioteca fará isso para você ao reutilizar um token de cache válido ou obtendo um novo token ao pedir ao usuário para fazer logon novamente com uma nova senha.</span><span class="sxs-lookup"><span data-stu-id="cec80-201">If you are using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), the library handles this for you by either reusing a valid cached token, or obtaining a new token from prompting the user to log in again with a new password.</span></span> <span data-ttu-id="cec80-202">Entretanto, a obtenção de um novo token pode falhar, pois as condições de acesso podem ser alteradas e o usuário não poderá mais acessar os dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="cec80-202">However, obtaining a new token may fail, since the conditions of access may have changed, and the user may no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="cec80-203">Chamar uma das duas APIs a seguir.</span><span class="sxs-lookup"><span data-stu-id="cec80-203">Call either of the following two APIs.</span></span> <span data-ttu-id="cec80-204">Se a chamada da API tiver êxito, o fluxo de notificação de recurso será retomado.</span><span class="sxs-lookup"><span data-stu-id="cec80-204">If the API call succeeds, the resource notification flow resumes.</span></span>

    - <span data-ttu-id="cec80-205">Chame a ação `/reauthorize` para autorizar novamente a assinatura sem estender a data de vencimento:</span><span class="sxs-lookup"><span data-stu-id="cec80-205">Call the `/reauthorize` action to re-authorize the subscription without extending its expiration date:</span></span>
        ```http
        POST  https://graph.microsoft.com/beta/subscriptions/{id}/reauthorize
        Content-type: application/json
        ```
    - <span data-ttu-id="cec80-206">Execute uma ação de renovação regular para autorizar novamente e renova a assinatura ao mesmo tempo:</span><span class="sxs-lookup"><span data-stu-id="cec80-206">Perform a regular renew action to re-authorize and renew the subscription at the same time:</span></span>
        ```http
        PATCH https://graph.microsoft.com/beta/subscriptions/{id}
        Content-Type: application/json

        {
           "expirationDateTime": "2019-09-21T11:00:00.0000000Z"
        }
        ```

      <span data-ttu-id="cec80-207">A renovação pode falhar, porque as verificações de autorização realizadas pelo sistema podem recusar o aplicativo ou o acesso do usuário ao recurso.</span><span class="sxs-lookup"><span data-stu-id="cec80-207">Renewing may fail, because the authorization checks performed by the system may deny the app or the user access to the resource.</span></span> <span data-ttu-id="cec80-208">Pode ser necessário que o aplicativo obtenha um novo token de acesso do usuário para autorizar novamente com êxito uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="cec80-208">It may be necessary for the app to obtain a new access token from the user to successfully re-authorize a subscription.</span></span> 
      
      <span data-ttu-id="cec80-209">Você pode tentar essa ações mais tarde, a qualquer momento e obter êxito se as condições de acesso mudarem.</span><span class="sxs-lookup"><span data-stu-id="cec80-209">You may retry these actions later, at any time, and succeed if the conditions of access change.</span></span> <span data-ttu-id="cec80-210">Todas as notificações sobre as alterações de recursos que ocorrem entre o tempo de envio da notificação do ciclo de vida e o tempo em que o aplicativo eventualmente recria a assinatura com êxito, seriam perdidas.</span><span class="sxs-lookup"><span data-stu-id="cec80-210">Any notifications about resource changes that happen between the time the life cycle notification was sent, and the time when the app eventually re-creates the subscription successfully, would be lost.</span></span> <span data-ttu-id="cec80-211">Nesses casos, o aplicativo deve buscar essas mudanças separadamente.</span><span class="sxs-lookup"><span data-stu-id="cec80-211">In such cases, the app should separately fetch those changes.</span></span>

### <a name="tips"></a><span data-ttu-id="cec80-212">Dicas </span><span class="sxs-lookup"><span data-stu-id="cec80-212">Tips</span></span>

<span data-ttu-id="cec80-213">Lembre-se do seguinte:</span><span class="sxs-lookup"><span data-stu-id="cec80-213">Keep the following in mind:</span></span>

1. <span data-ttu-id="cec80-214">Os desafios de autorização não substituem a necessidade de renova uma assinatura de alteração de recursos antes de expirar.</span><span class="sxs-lookup"><span data-stu-id="cec80-214">Authorization challenges do not replace the need to renew a resource change subscription before it expires.</span></span> 

    <span data-ttu-id="cec80-215">Embora você possa optar por renovar uma assinatura quando recebe um desafio de autorização, o Microsoft Graph pode não desafiar todas as suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="cec80-215">While you can choose to renew a subscription when you receive an authorization challenge, Microsoft Graph may not challenge all of your subscriptions.</span></span> <span data-ttu-id="cec80-216">Por exemplo, uma assinatura que não tem atividade e não tem notificações de recursos com entrega pendente pode não sinalizar desafios de reautorização para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cec80-216">For example, a subscription that does not have any activity and has no resource notifications pending delivery may not signal any re-authorization challenges to your app.</span></span> <span data-ttu-id="cec80-217">Certifique-se de [renovar assinaturas](webhooks.md#renewing-a-subscription) antes de expirarem.</span><span class="sxs-lookup"><span data-stu-id="cec80-217">Make sure to [renew subscriptions](webhooks.md#renewing-a-subscription) before they expire.</span></span>

2. <span data-ttu-id="cec80-218">A frequência dos desafios de autorização está sujeita a mudanças.</span><span class="sxs-lookup"><span data-stu-id="cec80-218">The frequency of authorization challenges is subject to change.</span></span>

    <span data-ttu-id="cec80-219">Não faça suposições sobre a frequência dos desafios de autorização.</span><span class="sxs-lookup"><span data-stu-id="cec80-219">Do not make assumptions about the frequency of authorization challenges.</span></span> <span data-ttu-id="cec80-220">Essas notificações informam quando executar ações, evitando que você tenha que acompanhar quais assinaturas devem ser autorizadas novamente.</span><span class="sxs-lookup"><span data-stu-id="cec80-220">These notifications tell you when to take actions, saving you from having to track which subscriptions require re-authorization.</span></span> <span data-ttu-id="cec80-221">Esteja pronto para lidar com os desafios de autorização seja uma vez em alguns minutos para cada assinatura ou raramente para algumas das suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="cec80-221">Be ready to handle authorization challenges anywhere from once a few minutes for every subscription, to rarely for only some of your subscriptions.</span></span>

### <a name="future-proof-your-code-to-handle-other-types-of-life-cycle-notifications"></a><span data-ttu-id="cec80-222">Proteja o seu código para lidar com outros tipos de notificações do ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="cec80-222">Future-proof your code to handle other types of life cycle notifications</span></span>

<span data-ttu-id="cec80-223">Espere que as notificações do ciclo de vida de assinatura sejam publicadas no mesmo ponto de extremidade especificado por **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="cec80-223">Expect subscription life cycle notifications to be posted to the same endpoint specified by **lifecycleNotificationUrl**.</span></span> <span data-ttu-id="cec80-224">Elas são diferenciadas pela propriedade **lifecycleEvent** e podem conter um esquema e propriedades ligeiramente diferentes para atender aos cenários que resolvem.</span><span class="sxs-lookup"><span data-stu-id="cec80-224">They differentiate by the **lifecycleEvent** property and may contain slightly different schema and properties to serve the scenarios they address.</span></span>

<span data-ttu-id="cec80-225">Implemente seu código em antecipação dos novos tipos de notificações do ciclo de vida:</span><span class="sxs-lookup"><span data-stu-id="cec80-225">Implement your code in anticipation of new types of life cycle notifications:</span></span>

1. <span data-ttu-id="cec80-226">Use a propriedade **lifecycleEvent** para identificar o tipo de notificação para determinar a resposta adequada.</span><span class="sxs-lookup"><span data-stu-id="cec80-226">Use the **lifecycleEvent** property to identify the type of notification so to determine the appropriate response.</span></span> <span data-ttu-id="cec80-227">Por exemplo, procure a `"lifecycleEvent": "reauthorizationRequired"` propriedade para identificar um evento específico e tratá-lo.</span><span class="sxs-lookup"><span data-stu-id="cec80-227">For example, look for the `"lifecycleEvent": "reauthorizationRequired"` property to identify a specific event, and handle it.</span></span>

1. <span data-ttu-id="cec80-228">Registre todos os eventos do ciclo de vida que seu aplicativo não reconhece para obter conhecimento.</span><span class="sxs-lookup"><span data-stu-id="cec80-228">Log any life cycle events that your app does not recognize to gain awareness.</span></span>

1. <span data-ttu-id="cec80-229">Inscreva-se no [Blog do Desenvolvedor do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) para assistir aos comunicados de notificações do ciclo de vida dos novos cenários.</span><span class="sxs-lookup"><span data-stu-id="cec80-229">Subscribe to the [Microsoft Graph Developer Blog](https://developer.microsoft.com/graph/blogs/) to watch for announcements of life cycle notifications for new scenarios.</span></span>

1. <span data-ttu-id="cec80-230">Procure a documentação relacionada às novas notificações do ciclo de vida e implemente o suporte para elas conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="cec80-230">Look up related documentation for new life cycle notifications and implement support for them as appropriate.</span></span>

## <a name="validating-the-authenticity-of-notifications"></a><span data-ttu-id="cec80-231">Validar a autenticidade das notificações </span><span class="sxs-lookup"><span data-stu-id="cec80-231">Validating the authenticity of notifications</span></span>

<span data-ttu-id="cec80-232">Os aplicativos geralmente executam lógica de negócios com base nos dados de recursos incluídos nas notificações.</span><span class="sxs-lookup"><span data-stu-id="cec80-232">Apps often execute business logic based on resource data included in notifications.</span></span> <span data-ttu-id="cec80-233">Verificar primeiro a autenticidade de cada notificação é importante.</span><span class="sxs-lookup"><span data-stu-id="cec80-233">Having first verified the authenticity of each notification is important.</span></span> <span data-ttu-id="cec80-234">Caso contrário, um terceiro poderia simular seu aplicativo com notificações falsas, fazê-lo executa a lógica de negócios incorretamente e levar a um incidente de segurança.</span><span class="sxs-lookup"><span data-stu-id="cec80-234">Otherwise, a third party could spoof your app with false notifications, make it execute its business logic incorrectly, and lead to a security incident.</span></span>

<span data-ttu-id="cec80-235">Para obter notificações básicas que não contenham dados de recursos, basta validá-las com base no valor **clientState** conforme descrito [aqui](webhooks.md#processing-the-notification).</span><span class="sxs-lookup"><span data-stu-id="cec80-235">For basic notifications which do not contain resource data, simply validate them based on the **clientState** value as described [here](webhooks.md#processing-the-notification).</span></span> <span data-ttu-id="cec80-236">Isso é aceitável, uma vez que você pode fazer chamadas confiáveis subsequentes do Microsoft Graph para obter acesso ao dados do recurso, portanto, o impacto das tentativas de falsificação é limitado.</span><span class="sxs-lookup"><span data-stu-id="cec80-236">This is acceptable, as you can make subsequent trusted Microsoft Graph calls to get access to resource data, and therefore the impact of any spoofing attempts is limited.</span></span> 

<span data-ttu-id="cec80-237">Para obter notificações que fornecem dados de recursos, realize uma validação mais completa antes de processar os dados.</span><span class="sxs-lookup"><span data-stu-id="cec80-237">For notifications that deliver resource data, perform a more thorough validation before processing the data.</span></span>

<span data-ttu-id="cec80-238">Nesta seção:</span><span class="sxs-lookup"><span data-stu-id="cec80-238">In this section:</span></span>

- [<span data-ttu-id="cec80-239">Tokens de validação na notificação</span><span class="sxs-lookup"><span data-stu-id="cec80-239">Validation tokens in the notification</span></span>](#validation-tokens-in-the-notification)
- [<span data-ttu-id="cec80-240">Como validar</span><span class="sxs-lookup"><span data-stu-id="cec80-240">How to validate</span></span>](#how-to-validate)
- [<span data-ttu-id="cec80-241">Exemplo de token JWT</span><span class="sxs-lookup"><span data-stu-id="cec80-241">Example JWT token</span></span>](#example-jwt-token)

### <a name="validation-tokens-in-the-notification"></a><span data-ttu-id="cec80-242">Tokens de validação na notificação</span><span class="sxs-lookup"><span data-stu-id="cec80-242">Validation tokens in the notification</span></span>

<span data-ttu-id="cec80-243">Uma notificação com dados de recursos contém uma propriedade adicional, **validationTokens**, que contém uma matriz de tokens JWT gerados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cec80-243">A notification with resource data contains an additional property, **validationTokens**, which contains an array of JWT tokens generated by Microsoft Graph.</span></span> <span data-ttu-id="cec80-244">O Microsoft Graph gera um único token para cada aplicativo distinto e par de locatários para os quais há um item na matriz **valor**.</span><span class="sxs-lookup"><span data-stu-id="cec80-244">Microsoft Graph generates a single token for each distinct app and tenant pair for whom there is an item in the **value** array.</span></span> <span data-ttu-id="cec80-245">Lembre-se de que as notificações podem conter uma mistura de itens para vários aplicativos e locatários que se inscreveram usando os mesmo **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="cec80-245">Keep in mind that notifications may contain a mix of items for various apps and tenants that subscribed using the same **notificationUrl**.</span></span>

<span data-ttu-id="cec80-246">No exemplo a seguir, a notificação contém dois itens para o mesmo aplicativo e para dois locatários diferentes, portanto, a matriz **validationTokens** contém dois tokens que precisam ser validados.</span><span class="sxs-lookup"><span data-stu-id="cec80-246">In the following example, the notification contains two items for the same app, and for two different tenants, therefore the **validationTokens** array contains two tokens that need to be validated.</span></span>

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
### <a name="how-to-validate"></a><span data-ttu-id="cec80-247">Como validar</span><span class="sxs-lookup"><span data-stu-id="cec80-247">How to validate</span></span>

<span data-ttu-id="cec80-248">Se você não está familiarizado com a validação de tokens, confira este [artigo do blog](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) para obter uma visão geral.</span><span class="sxs-lookup"><span data-stu-id="cec80-248">If you are new to token validation, refer to this [blog article](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) for a useful overview.</span></span> <span data-ttu-id="cec80-249">Use um SDK, como o [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) da biblioteca da Microsoft para .NET ou uma biblioteca de terceiros para uma plataforma diferente.</span><span class="sxs-lookup"><span data-stu-id="cec80-249">Use an SDK, such as Microsoft's [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) library for .NET, or a third party library for a different platform.</span></span>

<span data-ttu-id="cec80-250">Fique atento ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="cec80-250">Be mindful of the following:</span></span> 

- <span data-ttu-id="cec80-251">Certifique-se de sempre mandar um código de status `HTTP 202 Accepted` como parte da resposta à notificação.</span><span class="sxs-lookup"><span data-stu-id="cec80-251">Make sure to always send an `HTTP 202 Accepted` status code as part of the response to the notification.</span></span> 
- <span data-ttu-id="cec80-252">Faça isso antes de validar a notificação (por exemplo, se você armazenar notificações em filas para processamento posterior) ou depois (se você as processar em tempo real), mesmo se a validação falhar.</span><span class="sxs-lookup"><span data-stu-id="cec80-252">Do that before validating the notification (for example, if you store notifications in queues for later processing) or after (if you process them on the fly), even if validation failed.</span></span>
- <span data-ttu-id="cec80-253">A aceitação de uma notificação evita tentativas de entrega desnecessárias e também impede que possíveis atores invasores descubram se passaram ou falharam na validação.</span><span class="sxs-lookup"><span data-stu-id="cec80-253">Accepting a notification prevents unnecessary delivery retries and it also prevents any potential rogue actors from finding out if they passed or failed validation.</span></span> <span data-ttu-id="cec80-254">Você sempre pode optar por ignorar uma notificação inválida após aceitá-la.</span><span class="sxs-lookup"><span data-stu-id="cec80-254">You can always choose to ignore an invalid notification after you have accepted it.</span></span>

<span data-ttu-id="cec80-255">Especificamente, realize a validação em todos os tokens JWT na coleção **validationTokens**.</span><span class="sxs-lookup"><span data-stu-id="cec80-255">In particular, perform validation on every JWT token in the **validationTokens** collection.</span></span> <span data-ttu-id="cec80-256">Se os tokens falharem, considere a notificação como suspeita e continue investigando.</span><span class="sxs-lookup"><span data-stu-id="cec80-256">If any tokens fail, consider the notification suspicious and investigate further.</span></span> 

<span data-ttu-id="cec80-257">Use as etapas a seguir para validar tokens e aplicativos que geram tokens:</span><span class="sxs-lookup"><span data-stu-id="cec80-257">Use the following steps to validate tokens and apps that generate tokens:</span></span>

1. <span data-ttu-id="cec80-258">Valide se o token não expirou.</span><span class="sxs-lookup"><span data-stu-id="cec80-258">Validate that the token has not expired.</span></span>

2. <span data-ttu-id="cec80-259">Valide se o token não foi adulterado e foi emitido pela autoridade esperada, o Active Directory do Microsoft Azure:</span><span class="sxs-lookup"><span data-stu-id="cec80-259">Validate the token has not been tampered with and was issued by the expected authority, Microsoft Azure Active Directory:</span></span>

    - <span data-ttu-id="cec80-260">Obtenha as chaves de assinatura do ponto de extremidade de configuração comum: `https://login.microsoftonline.com/common/.well-known/openid-configuration`.</span><span class="sxs-lookup"><span data-stu-id="cec80-260">Obtain the signing keys from the common configuration endpoint: `https://login.microsoftonline.com/common/.well-known/openid-configuration`.</span></span> <span data-ttu-id="cec80-261">Essa configuração é armazenada em cache pelo aplicativo por um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="cec80-261">This configuration is cached by your app for a period of time.</span></span> <span data-ttu-id="cec80-262">Lembre-se de que a configuração é atualizada frequentemente, uma vez que as chaves de assinatura são giradas diariamente.</span><span class="sxs-lookup"><span data-stu-id="cec80-262">Be aware that the configuration is updated frequently as signing keys are rotated daily.</span></span>
    - <span data-ttu-id="cec80-263">Verifique a assinatura do token JWT usando essas chaves.</span><span class="sxs-lookup"><span data-stu-id="cec80-263">Verify the signature of the JWT token using those keys.</span></span>

    <span data-ttu-id="cec80-264">Não aceite tokens emitidos por outra autoridade.</span><span class="sxs-lookup"><span data-stu-id="cec80-264">Do not accept tokens issued by any other authority.</span></span>

3. <span data-ttu-id="cec80-265">Valide se o token foi emitido para o aplicativo que está inscrito para alterar as notificações.</span><span class="sxs-lookup"><span data-stu-id="cec80-265">Validate that the token was issued for your app that is subscribing to change notifications.</span></span>

    <span data-ttu-id="cec80-266">As etapas a seguir fazem parte da lógica de validação padrão nas bibliotecas de token JWT e podem ser tipicamente executadas como uma única chamada de função.</span><span class="sxs-lookup"><span data-stu-id="cec80-266">The following steps are part of standard validation logic in JWT token libraries and can typically be executed as a single function call.</span></span> 
    - <span data-ttu-id="cec80-267">Valide a “audiência” no token que corresponde à ID do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cec80-267">Validate the "audience" in the token matches your app ID.</span></span>
    - <span data-ttu-id="cec80-268">Se você tiver mais de um aplicativo recebendo notificações, certifique-se de verificar várias IDs.</span><span class="sxs-lookup"><span data-stu-id="cec80-268">If you have more than one app receiving notifications, make sure to check for multiple IDs.</span></span>


4. <span data-ttu-id="cec80-269">**Crítico**: valide se o aplicativo que gerou o token representa o distribuidor de notificação de alteração do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cec80-269">**Critical**: Validate that the app that generated the token represents the Microsoft Graph change notification publisher.</span></span> 

    - <span data-ttu-id="cec80-270">Verifique se a propriedade **appid** no token corresponde ao valor esperado de `0bf30f3b-4a52-48df-9a82-234910c4a086`.</span><span class="sxs-lookup"><span data-stu-id="cec80-270">Check that the **appid** property in the token matches the expected value of `0bf30f3b-4a52-48df-9a82-234910c4a086`.</span></span>
    - <span data-ttu-id="cec80-271">Isso garante que as notificações não sejam enviadas por um aplicativo diferente que não seja o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="cec80-271">This ensures that notifications are not sent by a different app that is not Microsoft Graph.</span></span>


### <a name="example-jwt-token"></a><span data-ttu-id="cec80-272">Exemplo de Token JWT </span><span class="sxs-lookup"><span data-stu-id="cec80-272">Example JWT token</span></span>

<span data-ttu-id="cec80-273">Veja um exemplo das propriedades incluídas no token JWT que são necessárias para a validação:</span><span class="sxs-lookup"><span data-stu-id="cec80-273">Here is an example of the properties included in the JWT token that are needed for validation:</span></span>

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

### <a name="example-verifying-validation-tokens"></a><span data-ttu-id="cec80-274">Exemplo: verificação de tokens de validação</span><span class="sxs-lookup"><span data-stu-id="cec80-274">Example: Verifying validation tokens</span></span>

```csharp
// add Microsoft.IdentityModel.Protocols.OpenIdConnect and System.IdentityModel.Tokens.Jwt nuget packages to your project
public async Task<bool> ValidateToken(string token, string tenantId, IEnumerable<string> appIds)
{
    var configurationManager = new ConfigurationManager<OpenIdConnectConfiguration>("https://login.microsoftonline.com/common/.well-known/openid-configuration", new OpenIdConnectConfigurationRetriever());
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
<span data-ttu-id="cec80-275">Para que o exemplo do Java funcione, também será necessário implementar o `JwkKeyResolver`.</span><span class="sxs-lookup"><span data-stu-id="cec80-275">For the Java sample to work, you will also need to implement the `JwkKeyResolver`.</span></span>  
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

## <a name="decrypting-resource-data-from-change-notifications"></a><span data-ttu-id="cec80-276">Descriptografar os dados de recursos de notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="cec80-276">Decrypting resource data from change notifications</span></span>

<span data-ttu-id="cec80-277">A propriedade **resourceData** de uma notificação inclui apenas as informações de ID básico e tipo de uma instância de recurso.</span><span class="sxs-lookup"><span data-stu-id="cec80-277">The **resourceData** property of a notification includes only the basic ID and type information of a resource instance.</span></span> <span data-ttu-id="cec80-278">A propriedade **encryptedData** contém os dados de recursos completos, criptografados pelo Microsoft Graph usando a chave pública fornecida na assinatura.</span><span class="sxs-lookup"><span data-stu-id="cec80-278">The **encryptedData** property contains the full resource data, encrypted by Microsoft Graph using the public key provided in the subscription.</span></span> <span data-ttu-id="cec80-279">A propriedade também contém valores necessários para verificação e descriptografia.</span><span class="sxs-lookup"><span data-stu-id="cec80-279">The property also contains values required for verification and decryption.</span></span> <span data-ttu-id="cec80-280">Isso é feito para aumentar a segurança dos dados do cliente acessados através de notificações.</span><span class="sxs-lookup"><span data-stu-id="cec80-280">This is done to increase the security of customer data accessed via notifications.</span></span> <span data-ttu-id="cec80-281">É a sua responsabilidade proteger a chave privada para garantir que os dados do cliente não possam ser descriptografados por terceiros, mesmo que eles consigam interceptar as notificações originais.</span><span class="sxs-lookup"><span data-stu-id="cec80-281">It is your responsibility to secure the private key to ensure that customer data cannot be decrypted by a third party, even if they manage to intercept the original notifications.</span></span>

<span data-ttu-id="cec80-282">Nesta seção:</span><span class="sxs-lookup"><span data-stu-id="cec80-282">In this section:</span></span>

- [<span data-ttu-id="cec80-283">Gerenciar as chaves de criptografia</span><span class="sxs-lookup"><span data-stu-id="cec80-283">Managing encryption keys</span></span>](#managing-encryption-keys)
- [<span data-ttu-id="cec80-284">Descriptografar os dados de recursos</span><span class="sxs-lookup"><span data-stu-id="cec80-284">Decrypting resource data</span></span>](#decrypting-resource-data)
- [<span data-ttu-id="cec80-285">Exemplo: descriptografar uma notificação com dados de recursos criptografados</span><span class="sxs-lookup"><span data-stu-id="cec80-285">Example: decrypting a notification with encrypted resource data</span></span>](#example-decrypting-a-notification-with-encrypted-resource-data)

### <a name="managing-encryption-keys"></a><span data-ttu-id="cec80-286">Gerenciar as chaves de criptografia</span><span class="sxs-lookup"><span data-stu-id="cec80-286">Managing encryption keys</span></span>

1. <span data-ttu-id="cec80-287">Obtenha um certificado com um par de chaves assimétricas.</span><span class="sxs-lookup"><span data-stu-id="cec80-287">Obtain a certificate with a pair of asymmetric keys.</span></span>

    - <span data-ttu-id="cec80-288">Você pode assinatura o certificado sozinho, uma vez que o Microsoft Graph não verifica o emissor do certificado e usa a chave pública somente para criptografia.</span><span class="sxs-lookup"><span data-stu-id="cec80-288">You can self-sign the certificate, since Microsoft Graph does not verify the certificate issuer, and uses the public key for only encryption.</span></span> 
    - <span data-ttu-id="cec80-289">Use o [Cofre da Chave do Azure](https://docs.microsoft.com/azure/key-vault/key-vault-whatis) como a solução para criar, girar e gerenciar certificados com segurança.</span><span class="sxs-lookup"><span data-stu-id="cec80-289">Use [Azure Key Vault](https://docs.microsoft.com/azure/key-vault/key-vault-whatis) as the solution to create, rotate, and securely manage certificates.</span></span> <span data-ttu-id="cec80-290">Cerifique-se de que as chaves atendem aos seguintes critérios:</span><span class="sxs-lookup"><span data-stu-id="cec80-290">Make sure the keys satisfy the following criteria:</span></span>

        - <span data-ttu-id="cec80-291">A chave deve ser do tipo `RSA`</span><span class="sxs-lookup"><span data-stu-id="cec80-291">The key must be of type `RSA`</span></span>
        - <span data-ttu-id="cec80-292">O tamanho da chave deve estar entre 2048 e 4096 bits</span><span class="sxs-lookup"><span data-stu-id="cec80-292">The key size must be between 2048 and 4096 bits</span></span>

2. <span data-ttu-id="cec80-293">Exportar o certificar no formato base64-encoded X.509 e **incluir apenas a chave pública**.</span><span class="sxs-lookup"><span data-stu-id="cec80-293">Export the certificate in base64-encoded X.509 format, and **include only the public key**.</span></span> 

3. <span data-ttu-id="cec80-294">Ao criar uma assinatura:</span><span class="sxs-lookup"><span data-stu-id="cec80-294">When creating a subscription:</span></span>

    - <span data-ttu-id="cec80-295">Forneça o certificado na propriedade **encryptionCertificate** usando o conteúdo base64-encoded no qual o certificado foi exportado.</span><span class="sxs-lookup"><span data-stu-id="cec80-295">Provide the certificate in the **encryptionCertificate** property, using the base64-encoded content that the certificate was exported in.</span></span>
    - <span data-ttu-id="cec80-296">Forneça seu próprio identificador na propriedade **encryptionCertificateId**.</span><span class="sxs-lookup"><span data-stu-id="cec80-296">Provide your own identifier in the **encryptionCertificateId** property.</span></span> 
  
        <span data-ttu-id="cec80-297">Esse identificador permite que você combine seus certificados com as notificações recebidas e que você recupere os certificados do seu repositório de certificados.</span><span class="sxs-lookup"><span data-stu-id="cec80-297">This identifier allows you to match your certificates to the notifications you receive, and to retrieve certificates from your certificate store.</span></span> <span data-ttu-id="cec80-298">O identificador pode ter no máximo 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="cec80-298">The identifier can be up to 128 characters.</span></span>

4. <span data-ttu-id="cec80-299">Gerencie a chave privada de forma segura para que seu código de processamento de notificação possa acessar a chave privada para descriptografar os dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="cec80-299">Manage the private key securely, so that your notification processing code can access the private key to decrypt resource data.</span></span>

#### <a name="rotating-keys"></a><span data-ttu-id="cec80-300">Chaves de rotação</span><span class="sxs-lookup"><span data-stu-id="cec80-300">Rotating keys</span></span>

<span data-ttu-id="cec80-301">Para minimizar o risco de uma chave privada ser comprometida, altere periodicamente suas chaves assimétricas.</span><span class="sxs-lookup"><span data-stu-id="cec80-301">To minimize the risk of a private key becoming compromised, periodically change your asymmetric keys.</span></span> <span data-ttu-id="cec80-302">Siga estas etapas para introduzir um novo par de chaves:</span><span class="sxs-lookup"><span data-stu-id="cec80-302">Follow these steps to introduce a new pair of keys:</span></span>

1. <span data-ttu-id="cec80-303">Obtenha um novo certificado com um novo par de chaves assimétricas.</span><span class="sxs-lookup"><span data-stu-id="cec80-303">Obtain a new certificate with a new pair of asymmetric keys.</span></span> <span data-ttu-id="cec80-304">Use-o para todas as novas assinaturas sendo criadas.</span><span class="sxs-lookup"><span data-stu-id="cec80-304">Use it for all new subscriptions being created.</span></span>

2. <span data-ttu-id="cec80-305">Atualize as assinaturas existentes com a nova chave de certificado.</span><span class="sxs-lookup"><span data-stu-id="cec80-305">Update existing subscriptions with the new certificate key.</span></span>

    - <span data-ttu-id="cec80-306">Faça isso como parte da renovação da assinatura regular.</span><span class="sxs-lookup"><span data-stu-id="cec80-306">Do this as part of regular subscription renewal.</span></span> 
    - <span data-ttu-id="cec80-307">Ou enumere todas as assinaturas e forneça a chave.</span><span class="sxs-lookup"><span data-stu-id="cec80-307">Or, enumerate all subscriptions and provide the key.</span></span> <span data-ttu-id="cec80-308">Use a [operação PATCH na assinatura](/graph/api/subscription-update?view=graph-rest-1.0) e atualize as propriedades **encryptionCertificate** e **encryptionCertificateId**.</span><span class="sxs-lookup"><span data-stu-id="cec80-308">Use the [PATCH operation on the subscription](/graph/api/subscription-update?view=graph-rest-1.0) and update the **encryptionCertificate** and **encryptionCertificateId** properties.</span></span>

3. <span data-ttu-id="cec80-309">Lembre-se do seguinte:</span><span class="sxs-lookup"><span data-stu-id="cec80-309">Keep in mind the following:</span></span>
    - <span data-ttu-id="cec80-310">Por um período de tempo, o certificado antigo ainda pode ser usado para criptografia.</span><span class="sxs-lookup"><span data-stu-id="cec80-310">For a period of time, the old certificate may still be used for encryption.</span></span> <span data-ttu-id="cec80-311">Seu aplicativo deve ter acesso a certificados novos e antigos para poder descriptografar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="cec80-311">Your app must have access to both old and new certificates to be able to decrypt content.</span></span>
    - <span data-ttu-id="cec80-312">Use a propriedade **encryptionCertificateId** em cada notificação para identificar a chave correta a ser usada.</span><span class="sxs-lookup"><span data-stu-id="cec80-312">Use the **encryptionCertificateId** property in each notification to identify the correct key to use.</span></span>
    - <span data-ttu-id="cec80-313">Descarte o certificado antigo somente quando não tiver visto nenhuma notificação recente referenciando-o.</span><span class="sxs-lookup"><span data-stu-id="cec80-313">Discard of the old certificate only when you have seen no recent notifications referencing it.</span></span>

### <a name="decrypting-resource-data"></a><span data-ttu-id="cec80-314">Descriptografar dados de recursos</span><span class="sxs-lookup"><span data-stu-id="cec80-314">Decrypting resource data</span></span>

<span data-ttu-id="cec80-315">Para otimizar o desempenho, o Microsoft Graph usa um processo de criptografia de duas etapas:</span><span class="sxs-lookup"><span data-stu-id="cec80-315">To optimize performance, Microsoft Graph uses a two-step encryption process:</span></span>
  - <span data-ttu-id="cec80-316">Ele gera uma chave simétrica de uso único e a usa para criptografar os dados do recurso.</span><span class="sxs-lookup"><span data-stu-id="cec80-316">It generates a single use symmetric key, and uses it to encrypt resource data.</span></span>
  - <span data-ttu-id="cec80-317">Ele usa a chave pública assimétrica (que você forneceu ao se inscrever) para criptografar a chave simétrica e inclui-la em cada notificação dessa assinatura.</span><span class="sxs-lookup"><span data-stu-id="cec80-317">It uses the public asymmetric key (that you provided when subscribing) to encrypt the symmetric key and includes it in each notification of that subscription.</span></span>

<span data-ttu-id="cec80-318">Presuma sempre que a chave simétrica é diferente para cada item na notificação.</span><span class="sxs-lookup"><span data-stu-id="cec80-318">Always assume that the symmetric key is different for each item in the notification.</span></span>

<span data-ttu-id="cec80-319">Para descriptografar os dados do recurso, seu aplicativo deve executar as etapas inversas usando as propriedades em **encryptedContent** em cada notificação:</span><span class="sxs-lookup"><span data-stu-id="cec80-319">To decrypt resource data, your app should perform the reverse steps, using the properties under **encryptedContent** in each notification:</span></span>

1. <span data-ttu-id="cec80-320">Use a propriedade **encryptionCertificateId** para identificar o certificado a ser usado.</span><span class="sxs-lookup"><span data-stu-id="cec80-320">Use the **encryptionCertificateId** property to identify the certificate to use.</span></span>

2. <span data-ttu-id="cec80-321">Inicialize um componente criptográfico da RSA (como o .NET [RSACryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) com a chave privada.</span><span class="sxs-lookup"><span data-stu-id="cec80-321">Initialize an RSA cryptographic component (such as the .NET [RSACryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) with the private key.</span></span>

3. <span data-ttu-id="cec80-322">Descriptografe a chave simétrica entregue na propriedade **dataKey** de cada item na notificação.</span><span class="sxs-lookup"><span data-stu-id="cec80-322">Decrypt the symmetric key delivered in the **dataKey** property of each item in the notification.</span></span>

    <span data-ttu-id="cec80-323">Use o Preenchimento de Criptografia Assimétrica Ideal (OAEP) para o algoritmo de descriptografia.</span><span class="sxs-lookup"><span data-stu-id="cec80-323">Use Optimal Asymmetric Encryption Padding (OAEP) for the decryption algorithm.</span></span>

4. <span data-ttu-id="cec80-324">Use a chave simétrica para calcular a assinatura HMAC-SHA256 do valor em **dados**.</span><span class="sxs-lookup"><span data-stu-id="cec80-324">Use the symmetric key to calculate the HMAC-SHA256 signature of the value in **data**.</span></span>
  
    <span data-ttu-id="cec80-325">Compare-o com o valor em **dataSignature**.</span><span class="sxs-lookup"><span data-stu-id="cec80-325">Compare it to the value in **dataSignature**.</span></span> <span data-ttu-id="cec80-326">Se eles não corresponderem, considere que a carga foi adulterada e não a descriptografe.</span><span class="sxs-lookup"><span data-stu-id="cec80-326">If they do not match, assume the payload has been tampered with and do not decrypt it.</span></span>

5. <span data-ttu-id="cec80-327">Use a chave simétrica com a criptografia AES (como o .NET [AesCryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) para descriptografar o conteúdo em **dados**.</span><span class="sxs-lookup"><span data-stu-id="cec80-327">Use the symmetric key with an Advanced Encryption Standard (AES) (such as the .NET [AesCryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) to decrypt the content in **data**.</span></span>

    - <span data-ttu-id="cec80-328">Use os seguintes parâmetros de descriptografia para o algoritmo AES:</span><span class="sxs-lookup"><span data-stu-id="cec80-328">Use the following decryption parameters for the AES algorithm:</span></span>

        - <span data-ttu-id="cec80-329">Preenchimento: PKCS7</span><span class="sxs-lookup"><span data-stu-id="cec80-329">Padding: PKCS7</span></span>
        - <span data-ttu-id="cec80-330">Modo de criptografia: CBC</span><span class="sxs-lookup"><span data-stu-id="cec80-330">Cipher mode: CBC</span></span>
    - <span data-ttu-id="cec80-331">Defina o “vetor de inicialização” copiando os primeiros 16 bytes da chave simétrica usada para descriptografia.</span><span class="sxs-lookup"><span data-stu-id="cec80-331">Set the "initialization vector" by copying the first 16 bytes of the symmetric key used for decryption.</span></span>

6. <span data-ttu-id="cec80-332">O valor descriptografado é uma cadeia de caracteres JSON que representa a instância do recurso na notificação.</span><span class="sxs-lookup"><span data-stu-id="cec80-332">The decrypted value is a JSON string that represents the resource instance in the notification.</span></span>


### <a name="example-decrypting-a-notification-with-encrypted-resource-data"></a><span data-ttu-id="cec80-333">Exemplo: descriptografar uma notificação com dados de recurso criptografados</span><span class="sxs-lookup"><span data-stu-id="cec80-333">Example: decrypting a notification with encrypted resource data</span></span>

<span data-ttu-id="cec80-334">Veja a seguir um exemplo de notificação que inclui valores de propriedade criptografados de uma instância **chatMessage** em uma mensagem do canal.</span><span class="sxs-lookup"><span data-stu-id="cec80-334">The following is an example notification that includes encrypted property values of a **chatMessage** instance in a channel message.</span></span> <span data-ttu-id="cec80-335">A instância é especificada pelo valor `@odata.id`.</span><span class="sxs-lookup"><span data-stu-id="cec80-335">The instance is specified by the `@odata.id` value.</span></span>

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

<span data-ttu-id="cec80-336">A seção contém alguns trechos de código úteis que usam C# e .NET em cada etapa da descriptografia.</span><span class="sxs-lookup"><span data-stu-id="cec80-336">This section contains some useful code snippets that use C# and .NET for each stage of decryption.</span></span>

#### <a name="decrypt-the-symmetric-key"></a><span data-ttu-id="cec80-337">Descriptografar a chave simétrica</span><span class="sxs-lookup"><span data-stu-id="cec80-337">Decrypt the symmetric key</span></span>

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

#### <a name="compare-data-signature-using-hmac-sha256"></a><span data-ttu-id="cec80-338">Comparar assinatura de dados usando HMAC-SHA256</span><span class="sxs-lookup"><span data-stu-id="cec80-338">Compare data signature using HMAC-SHA256</span></span>

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
if (comparisonSignature.equals(encodedHashedData);)
{
    // Continue with decryption of the encryptedPayload.
}
else
{
    // Do not attempt to decrypt encryptedPayload. Assume notification payload has been tampered with and investigate.
}
```

#### <a name="decrypt-the-resource-data-content"></a><span data-ttu-id="cec80-339">Descriptografar o conteúdo dos dados de recursos</span><span class="sxs-lookup"><span data-stu-id="cec80-339">Decrypt the resource data content</span></span>

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

## <a name="see-also"></a><span data-ttu-id="cec80-340">Confira também</span><span class="sxs-lookup"><span data-stu-id="cec80-340">See also</span></span>

- [<span data-ttu-id="cec80-341">Configurar notificações para alterações nos dados de usuário</span><span class="sxs-lookup"><span data-stu-id="cec80-341">Set up notifications for changes in user data</span></span>](webhooks.md)
- [<span data-ttu-id="cec80-342">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="cec80-342">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-beta)
- [<span data-ttu-id="cec80-343">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="cec80-343">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="cec80-344">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="cec80-344">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="cec80-345">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="cec80-345">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
