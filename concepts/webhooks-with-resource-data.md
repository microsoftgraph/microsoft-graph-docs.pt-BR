---
title: Configurar notificações de alteração que incluam dados de recursos (visualização)
description: O Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. As notificações de alteração podem incluir propriedades de recursos.
author: davidmu1
ms.prod: non-product-specific
localization_priority: Priority
ms.openlocfilehash: eeff200c14b2da9039fecba39d7834c419e8caec
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598518"
---
# <a name="set-up-change-notifications-that-include-resource-data-preview"></a><span data-ttu-id="7931a-104">Configurar notificações de alteração que incluam dados de recursos (visualização)</span><span class="sxs-lookup"><span data-stu-id="7931a-104">Set up change notifications that include resource data (preview)</span></span>

<span data-ttu-id="7931a-105">O Microsoft Graph permite que os aplicativos inscrevam-se para alterar as notificações de recursos através do [webhooks](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="7931a-105">Microsoft Graph allows apps to subscribe to change notifications for resources via [webhooks](webhooks.md).</span></span> <span data-ttu-id="7931a-106">É possíve configurar as assinaturas para incluir os dados alterados dos recursos (como o conteúdo de uma mensagem de bate-papo ou informações de presença do Microsoft Teams) nas notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="7931a-106">You can set up subscriptions to include the changed resource data (such as the content of a Microsoft Teams chat message or Microsoft Teams presence information) in change notifications.</span></span> <span data-ttu-id="7931a-107">Em seguida, seu aplicativo pode usar a lógica de negócios sem ter que fazer uma chamada à API separada para buscar o recurso alterado.</span><span class="sxs-lookup"><span data-stu-id="7931a-107">Your app can then run its business logic without having to make a separate API call to fetch the changed resource.</span></span> <span data-ttu-id="7931a-108">Como resultado, o aplicativo funciona melhor ao realizar menos chamadas da API, o que é benéfico em cenários de larga escala.</span><span class="sxs-lookup"><span data-stu-id="7931a-108">As a result, the app performs better by making fewer API calls, which is beneficial in large scale scenarios.</span></span>

<span data-ttu-id="7931a-109">A inclusão de dados de recursos como parte das notificações de alteração exige que, para atender aos requisitos de acesso e segurança de dados, você implemente a seguinte lógica adicional :</span><span class="sxs-lookup"><span data-stu-id="7931a-109">Including resource data as part of change notifications requires you to implement the following additional logic to satisfy data access and security requirements:</span></span> 

- <span data-ttu-id="7931a-110">[Lide com](#subscription-lifecycle-notifications) as notificações especiais sobre o ciclo de vida da assinatura para manter um fluxo ininterrupto de dados.</span><span class="sxs-lookup"><span data-stu-id="7931a-110">[Handle](#subscription-lifecycle-notifications) special subscription lifecycle notifications to maintain an uninterrupted flow of data.</span></span> <span data-ttu-id="7931a-111">O Microsoft Graph envia notificações sobre o ciclo de vida de tempos em tempos para exigir que um aplicativo seja autorizado novamente e para garantir que os problemas de acesso não ocorram inesperadamente, incluindo dados de recursos nas notificações de alterações.</span><span class="sxs-lookup"><span data-stu-id="7931a-111">Microsoft Graph sends lifecycle notifications from time to time to require an app to re-authorize, to make sure access issues have not unexpectedly cropped up for including resource data in change notifications.</span></span>
- <span data-ttu-id="7931a-112">[Confirme](#validating-the-authenticity-of-notifications) a autenticidade das notificações de alteração como originárias do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7931a-112">[Validate](#validating-the-authenticity-of-notifications) the authenticity of change notifications as having originated from Microsoft Graph.</span></span>
- <span data-ttu-id="7931a-113">[Forneça](#decrypting-resource-data-from-change-notifications) uma chave de criptografia pública e utilize uma chave privada para decriptar os dados de recursos recebidos por meio das notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="7931a-113">[Provide](#decrypting-resource-data-from-change-notifications) a public encryption key and use a private key to decrypt resource data received through change notifications.</span></span>

## <a name="resource-data-in-notification-payload"></a><span data-ttu-id="7931a-114">Dados de recursos na carga de notificação </span><span class="sxs-lookup"><span data-stu-id="7931a-114">Resource data in notification payload</span></span>

<span data-ttu-id="7931a-115">Geralmente, esse tipo de notificação de alteração inclui os seguintes dados de recursos na carga:</span><span class="sxs-lookup"><span data-stu-id="7931a-115">In general, this type of change notifications include the following resource data in the payload:</span></span>

- <span data-ttu-id="7931a-116">ID e tipo de instância de recurso alterado, retornados na propriedade **resourceData**.</span><span class="sxs-lookup"><span data-stu-id="7931a-116">ID and type of the changed resource instance, returned in the **resourceData** property.</span></span>
- <span data-ttu-id="7931a-117">Todos os valores de propriedade da instância de recurso, criptografados conforme especificado na assinatura, retornados na propriedade **encryptedContent**.</span><span class="sxs-lookup"><span data-stu-id="7931a-117">All the property values of that resource instance, encrypted as specified in the subscription, returned in the **encryptedContent** property.</span></span>
- <span data-ttu-id="7931a-118">Or, dependendo do recurso, propriedades específicas retornadas na propriedade **resourceData**.</span><span class="sxs-lookup"><span data-stu-id="7931a-118">Or, depending on the resource, specific properties returned in the **resourceData** property.</span></span> <span data-ttu-id="7931a-119">Para obter somente propriedades específicas, especifique-as como parte da URL do **recurso** na assinatura, usando um parâmetro `$select`.</span><span class="sxs-lookup"><span data-stu-id="7931a-119">To get only specific properties, specify them as part of the **resource** URL in the subscription, using a `$select` parameter.</span></span>  


## <a name="supported-resources"></a><span data-ttu-id="7931a-120">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="7931a-120">Supported resources</span></span>

<span data-ttu-id="7931a-121">Atualmente, o recurso do Microsoft Teams [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) (visualização), bem como o recurso do Microsoft Teams [presence](/graph/api/resources/presence?view=graph-rest-beta) (visualização) oferecem suporte a notificações de alterações que incluem dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="7931a-121">Currently, the Microsoft Teams [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) (preview) as well as the Microsoft Teams [presence](/graph/api/resources/presence?view=graph-rest-beta) (preview) resources supports change notifications that include resource data.</span></span> <span data-ttu-id="7931a-122">Especificamente, você pode configurar uma assinatura que se aplique a uma das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="7931a-122">Specifically, you can set up a subscription that applies to one of the following:</span></span>

- <span data-ttu-id="7931a-123">Mensagens novas ou alteradas em um canal específico do Teams: `/teams/{id}/channels/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="7931a-123">New or changed messages in a specific Teams channel: `/teams/{id}/channels/{id}/messages`</span></span>
- <span data-ttu-id="7931a-124">Mensagens novas ou alteradas em um bate-papo específico do Teams: `/chats/{id}/messages`</span><span class="sxs-lookup"><span data-stu-id="7931a-124">New or changed messages in a specific Teams chat: `/chats/{id}/messages`</span></span>
- <span data-ttu-id="7931a-125">Atualização das informações de presença do usuário: `/communications/presences/{id}`</span><span class="sxs-lookup"><span data-stu-id="7931a-125">User's presence information update: `/communications/presences/{id}`</span></span>

<span data-ttu-id="7931a-126">Os recursos **chatMessage** e **presence** suportam, incluindo todas as propriedades de uma instância modificada em uma notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="7931a-126">The **chatMessage** and the **presence** resources support including all the properties of a changed instance in a change notification.</span></span> <span data-ttu-id="7931a-127">Eles não suportam o retorno de apenas propriedades seletivas da instância.</span><span class="sxs-lookup"><span data-stu-id="7931a-127">They do not support returning only selective properties of the instance.</span></span> 

<span data-ttu-id="7931a-128">Este artigo mostra um exemplo de assinatura para alterar as notificações de mensagens em um canal do Teams, com cada notificação de alteração incluindo todos os dados do recurso da instância \*\* chatMessage \*\* alterada.</span><span class="sxs-lookup"><span data-stu-id="7931a-128">This article walks through an example of subscribing to change notifications of messages in a Teams channel, with each change notification including the full resource data of the changed **chatMessage** instance.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="7931a-129">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="7931a-129">Creating a subscription</span></span>

<span data-ttu-id="7931a-130">Para que os dados de recursos estejam incluídos nas notificações de alteração, você **deve** especificar as seguintes propriedades, além das que geralmente são especificadas ao [criar uma assinatura](webhooks.md#creating-a-subscription):</span><span class="sxs-lookup"><span data-stu-id="7931a-130">To have resource data included in change notifications, you **must** specify the following properties, in addition to those that are usually specified when [creating a subscription](webhooks.md#creating-a-subscription):</span></span>

- <span data-ttu-id="7931a-131">**includeResourceData** que deve ser definido como `true` para solicitar explicitamente os dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="7931a-131">**includeResourceData** which should be set to `true` to explicitly request resource data.</span></span>
- <span data-ttu-id="7931a-132">\*\* lifecycleNotificationUrl \*\*, que é um terminal em que [ notificações sobre o ciclo de vida ](#subscription-lifecycle-notifications) são entregues.</span><span class="sxs-lookup"><span data-stu-id="7931a-132">**lifecycleNotificationUrl** which is an endpoint where [lifecycle notifications](#subscription-lifecycle-notifications) are delivered.</span></span> <span data-ttu-id="7931a-133">Pode ser igual ou diferente de **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7931a-133">This can be the same or different as **notificationUrl**.</span></span>
- <span data-ttu-id="7931a-134">**encryptionCertificate** que contém apenas a chave público que o Microsoft Graph usa para criptografar os dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="7931a-134">**encryptionCertificate** which contains only the public key that Microsoft Graph uses to encrypt resource data.</span></span> <span data-ttu-id="7931a-135">Mantenha a chave privada correspondente para [descriptografar o conteúdo](#decrypting-resource-data-from-change-notifications).</span><span class="sxs-lookup"><span data-stu-id="7931a-135">Keep the corresponding private key to [decrypt the content](#decrypting-resource-data-from-change-notifications).</span></span>
- <span data-ttu-id="7931a-136">**encryptionCertificateId** é o seu próprio identificador para o certificado.</span><span class="sxs-lookup"><span data-stu-id="7931a-136">**encryptionCertificateId** which is your own identifier for the certificate.</span></span> <span data-ttu-id="7931a-137">Use esse ID para corresponder a cada notificação de alteração cujo certificado foi utilizado para descriptografia.</span><span class="sxs-lookup"><span data-stu-id="7931a-137">Use this ID to match in each change notification, which certificate to use for decryption.</span></span>

<span data-ttu-id="7931a-138">Tenha em mente o seguinte:</span><span class="sxs-lookup"><span data-stu-id="7931a-138">Keep the following in mind:</span></span>

- <span data-ttu-id="7931a-139">Utilize o mesmo nome de host para as notificação de alteração dos terminais (**notificationUrl** e **lifecycleNotificationUrl**).</span><span class="sxs-lookup"><span data-stu-id="7931a-139">Use the same host name for both change notification endpoints (**notificationUrl** and **lifecycleNotificationUrl**).</span></span>
- <span data-ttu-id="7931a-140">Valide os dois terminais conforme descrito [ aqui ](webhooks.md#notification-endpoint-validation).</span><span class="sxs-lookup"><span data-stu-id="7931a-140">Validate both endpoints as described [here](webhooks.md#notification-endpoint-validation).</span></span> <span data-ttu-id="7931a-141">Se você quiser usar a mesma URL para os dois pontos de extremidade, você receberá e responderá a duas solicitações de validação.</span><span class="sxs-lookup"><span data-stu-id="7931a-141">If you choose to use the same URL for both endpoints, you will receive and respond to two validation requests.</span></span>
- <span data-ttu-id="7931a-142">Não é possível atualizar (`PATCH`) uma assinatura existente para adicionar a propriedade **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7931a-142">You cannot update (`PATCH`) an existing subscription to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="7931a-143">Você deve remover a assinatura existente e criar uma nova assinatura para incluir a propriedade **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7931a-143">You should remove the existing subscription, and create a new subscription to include the **lifecycleNotificationUrl** property.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="7931a-144">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="7931a-144">Subscription request example</span></span>

<span data-ttu-id="7931a-145">O exemplo a seguir assina dois tipos de notificações:</span><span class="sxs-lookup"><span data-stu-id="7931a-145">The following example subscribes to two types of notifications:</span></span> 

- <span data-ttu-id="7931a-146">Alterações de recursos - canais de mensagens sendo criados ou atualizados no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="7931a-146">Resource changes - channel messages being created or updated in Microsoft Teams</span></span>
- <span data-ttu-id="7931a-147">Eventos do ciclo de vida da assinatura que podem afetar o fluxo de notificações de alterações.</span><span class="sxs-lookup"><span data-stu-id="7931a-147">Subscription lifecycle events which can affect the flow of change notifications.</span></span> <span data-ttu-id="7931a-148">Veja mais detalhes sobre as notificações do ciclo de vida na [próxima seção](#subscription-lifecycle-notifications).</span><span class="sxs-lookup"><span data-stu-id="7931a-148">See more details about lifecycle notifications in the [next section](#subscription-lifecycle-notifications).</span></span>

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

### <a name="subscription-response"></a><span data-ttu-id="7931a-149">Resposta de assinatura</span><span class="sxs-lookup"><span data-stu-id="7931a-149">Subscription response</span></span>
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

## <a name="subscription-lifecycle-notifications"></a><span data-ttu-id="7931a-150">Notificações do ciclo de vida da assinatura</span><span class="sxs-lookup"><span data-stu-id="7931a-150">Subscription lifecycle notifications</span></span>

<span data-ttu-id="7931a-151">Certos eventos podem interferir no fluxo de notificação de alterações em uma assinatura existente.</span><span class="sxs-lookup"><span data-stu-id="7931a-151">Certain events can interfere with change notification flow in an existing subscription.</span></span> <span data-ttu-id="7931a-152">As notificações sobre o ciclo de vida da assinatura informam as ações a serem tomadas para manter um fluxo ininterrupto.</span><span class="sxs-lookup"><span data-stu-id="7931a-152">Subscription lifecycle notifications inform you actions to take in order to maintain an uninterrupted flow.</span></span> <span data-ttu-id="7931a-153">Ao contrário de uma notificação de alteração de recurso que informa uma alteração em uma instância de recurso, uma notificação do ciclo de vida é sobre a própria assinatura e seu estado atual no ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="7931a-153">Unlike a resource change notification which informs a change to a resource instance, a lifecycle notification is about the subscription itself, and its current state in the lifecycle.</span></span> 

<span data-ttu-id="7931a-154">As notificações sobre o ciclo de vida são entregues no **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7931a-154">Lifecycle notifications are delivered to the **lifecycleNotificationUrl**.</span></span> 

<span data-ttu-id="7931a-155">Nesta seção:</span><span class="sxs-lookup"><span data-stu-id="7931a-155">In this section:</span></span>

- [<span data-ttu-id="7931a-156">Notificação de vida útil que desafia a autorização da assinatura</span><span class="sxs-lookup"><span data-stu-id="7931a-156">Lifecycle notification that challenges subscription authorization</span></span>](#lifecycle-notification-that-challenges-subscription-authorization)
- [<span data-ttu-id="7931a-157">Fluxo de desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="7931a-157">Authorization challenge flow</span></span>](#authorization-challenge-flow)
- [<span data-ttu-id="7931a-158">Exemplo de desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="7931a-158">Example authorization challenge</span></span>](#example-authorization-challenge)
- [<span data-ttu-id="7931a-159">Respondendo a um desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="7931a-159">Responding to an authorization challenge</span></span>](#responding-to-an-authorization-challenge)
- [<span data-ttu-id="7931a-160">Dicas</span><span class="sxs-lookup"><span data-stu-id="7931a-160">Tips</span></span>](#tips)
- [<span data-ttu-id="7931a-161">Planeje seu código para lidar com outros tipos de notificações do ciclo de vida no futuro</span><span class="sxs-lookup"><span data-stu-id="7931a-161">Future-proof your code to handle other types of lifecycle notifications</span></span>](#future-proof-your-code-to-handle-other-types-of-lifecycle-notifications)

### <a name="lifecycle-notification-that-challenges-subscription-authorization"></a><span data-ttu-id="7931a-162">Notificação do ciclo de vida que desafia a autorização da assinatura</span><span class="sxs-lookup"><span data-stu-id="7931a-162">Lifecycle notification that challenges subscription authorization</span></span>

<span data-ttu-id="7931a-163">Um tipo de notificação do ciclo de vida que desafia o estado autorizado de uma assinatura ativa.</span><span class="sxs-lookup"><span data-stu-id="7931a-163">One type of lifecycle notifications challenges the authorized state of an active subscription.</span></span> <span data-ttu-id="7931a-164">Quando a propriedade **lifecycleEvent** em uma notificação indica `reauthorizationRequired`, que você deve autorizar novamente a assinatura para manter o fluxo de dados.</span><span class="sxs-lookup"><span data-stu-id="7931a-164">When the **lifecycleEvent** property in a notification indicates `reauthorizationRequired`, you must re-authorize the subscription to maintain the data flow.</span></span>

<span data-ttu-id="7931a-165">Quando você cria uma assinatura de longa duração (por exemplo, uma que dura 3 dias), altere os fluxos de notificações para o local indicado em **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7931a-165">When you create a long-lived subscription (for example, one that lasts for 3 days), change notifications flows to the location indicated in **notificationUrl**.</span></span> <span data-ttu-id="7931a-166">Entretanto, a qualquer momento, o Microsoft Graph pode exigir que você autorize novamente a assinatura para provar que ainda tem acesso aos dados de recursos, caso as condições de acesso tenham sido alteradas desde a criação da assinatura.</span><span class="sxs-lookup"><span data-stu-id="7931a-166">However, at any point in time, Microsoft Graph may require that you re-authorize the subscription to prove that you still have access to resource data, in case the conditions of access have changed since the subscription was created.</span></span> <span data-ttu-id="7931a-167">A seguir estão exemplos de alterações que afetam o acesso aos dados:</span><span class="sxs-lookup"><span data-stu-id="7931a-167">The following are examples of changes that affect your access to data:</span></span>

- <span data-ttu-id="7931a-168">Um administrador de locatários pode revogar as permissões do seu aplicativo para ler um recurso.</span><span class="sxs-lookup"><span data-stu-id="7931a-168">A tenant administrator may revoke your app's permissions to read a resource.</span></span>
- <span data-ttu-id="7931a-169">Em um cenário interativo, o usuário que fornece o token de autenticação ao seu aplicativo pode estar sujeito a políticas dinâmicas com base em vários fatores, como o local, o estado do dispositivo ou a avaliação de risco.</span><span class="sxs-lookup"><span data-stu-id="7931a-169">In an interactive scenario, the user who provides the authentication token to your app may be subject to dynamic policies based on various factors, such as their location, device state, or risk assesment.</span></span> <span data-ttu-id="7931a-170">Por exemplo, se o usuário alterar o seu local físico, pode ser que ele não tenha mais permissão para acessar os dados e seu aplicativo não conseguirá autorizar novamente a assinatura.</span><span class="sxs-lookup"><span data-stu-id="7931a-170">For example, if the user changes their physical location, the user may no longer be allowed to access the data, and your app will not be able to re-authorize the subscription.</span></span> <span data-ttu-id="7931a-171">Para saber mais sobre políticas dinâmicas que controlam o acesso, confira [políticas de acesso condicional do Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/overview).</span><span class="sxs-lookup"><span data-stu-id="7931a-171">For more information on dynamic policies that control access, see [Azure AD conditional access policies](https://docs.microsoft.com/azure/active-directory/conditional-access/overview).</span></span> 

### <a name="authorization-challenge-flow"></a><span data-ttu-id="7931a-172">Fluxo de desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="7931a-172">Authorization challenge flow</span></span>

<span data-ttu-id="7931a-173">O fluxo de um desafio de autorização para uma assinatura ativa e não expirada tem a seguinte aparência:</span><span class="sxs-lookup"><span data-stu-id="7931a-173">The flow of an authorization challenge for an active, non-expired subscription looks as follows:</span></span>

1. <span data-ttu-id="7931a-174">O Microsoft Graph exige que uma assinatura seja autorizada novamente.</span><span class="sxs-lookup"><span data-stu-id="7931a-174">Microsoft Graph requires a subscription to be re-authorized</span></span>
    
    <span data-ttu-id="7931a-175">Os motivos para isso podem variar de recurso para recurso e podem mudar com o tempo.</span><span class="sxs-lookup"><span data-stu-id="7931a-175">The reasons for this may vary from resource to resource, and may change over time.</span></span> <span data-ttu-id="7931a-176">Independentemente da causa do evento de reautorização, você precisará respondê-lo.</span><span class="sxs-lookup"><span data-stu-id="7931a-176">Regardless of the cause of the re-authorization event, you will need to respond to it.</span></span>

2. <span data-ttu-id="7931a-177">O Microsoft Graph envia uma notificação de desafio de autorização para **lifecycleNotificationUrl**</span><span class="sxs-lookup"><span data-stu-id="7931a-177">Microsoft Graph sends an authorization challenge notification to the **lifecycleNotificationUrl**</span></span>

    <span data-ttu-id="7931a-178">Observe que o fluxo de notificações de alterações pode continuar por um tempo, dando a você tempo extra para responder.</span><span class="sxs-lookup"><span data-stu-id="7931a-178">Note that the flow of change notifications may continue for a while, giving you extra time to respond.</span></span> <span data-ttu-id="7931a-179">No entanto, eventualmente, a entrega da notificação de alteração será pausada até que você tome as medidas necessárias.</span><span class="sxs-lookup"><span data-stu-id="7931a-179">However, eventually change notification delivery will pause, until you take the required action.</span></span>

3. <span data-ttu-id="7931a-180">Responda a esta notificação do ciclo de vida com uma das duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="7931a-180">Respond to this lifecycle notification in one of two ways:</span></span>
    1. <span data-ttu-id="7931a-181">Autorize a assinatura novamente.</span><span class="sxs-lookup"><span data-stu-id="7931a-181">Re-authorize the subscription.</span></span> <span data-ttu-id="7931a-182">Isso não estende a data de vencimento da assinatura.</span><span class="sxs-lookup"><span data-stu-id="7931a-182">This does not extend the expiry date of the subscription.</span></span>
    2. <span data-ttu-id="7931a-183">Renove a assinatura.</span><span class="sxs-lookup"><span data-stu-id="7931a-183">Renew the subscription.</span></span> <span data-ttu-id="7931a-184">Isso reautoriza e estenda a data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="7931a-184">This both re-authorizes and extends the expiry date.</span></span>

    <span data-ttu-id="7931a-185">Observação: as duas ações exigem a apresentação de um token de autenticação válido, semelhante a [criar uma nova assinatura](webhooks.md#creating-a-subscription) ou [renova uma assinatura antes da sua expiração](webhooks.md#renewing-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="7931a-185">Note: Both actions require you to present a valid authentication token, similar to [creating a new subscription](webhooks.md#creating-a-subscription) or [renewing a subscription before its expiry](webhooks.md#renewing-a-subscription).</span></span>

4. <span data-ttu-id="7931a-186">Se você autorizar ou renovar com êxito a assinatura, as notificações de alteração continuarão.</span><span class="sxs-lookup"><span data-stu-id="7931a-186">If you successfully re-authorize or renew the subscription, change notifications continue.</span></span> <span data-ttu-id="7931a-187">Caso contrário, as notificações de alteração permanecerão pausadas.</span><span class="sxs-lookup"><span data-stu-id="7931a-187">Otherwise, change notifications remain paused.</span></span>
    
### <a name="example-authorization-challenge"></a><span data-ttu-id="7931a-188">Exemplo de desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="7931a-188">Example authorization challenge</span></span>

<span data-ttu-id="7931a-189">Abaixo está um exemplo de notificação do ciclo de vida que solicita a autorização de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="7931a-189">Below is an example lifecycle notification that requests re-authorizing a subscription.</span></span> 

<span data-ttu-id="7931a-190">Observe o seguinte:</span><span class="sxs-lookup"><span data-stu-id="7931a-190">Note the following:</span></span>

- <span data-ttu-id="7931a-191">O campo `"lifecycleEvent": "reauthorizationRequired"` identifica essa notificação como um desafio de autorização.</span><span class="sxs-lookup"><span data-stu-id="7931a-191">The `"lifecycleEvent": "reauthorizationRequired"` field identifies this notification as an authorization challenge.</span></span>
- <span data-ttu-id="7931a-192">A notificação de ciclo de vida não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.</span><span class="sxs-lookup"><span data-stu-id="7931a-192">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="7931a-193">Semelhante às notificações de alteração, você pode agrupar as notificações do ciclo de vida em conjunto (na coleção de**valores**), cada uma com um valor possivelmente diferente do **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="7931a-193">Similar to change notifications, you can batch lifecycle notifications together (in the **value** collection), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="7931a-194">Processe cada notificação de ciclo de vida no lote adequadamente.</span><span class="sxs-lookup"><span data-stu-id="7931a-194">Process each lifecycle notification in the batch accordingly.</span></span>

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

> <span data-ttu-id="7931a-195">**Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração forem entregues, confira [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="7931a-195">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="responding-to-an-authorization-challenge"></a><span data-ttu-id="7931a-196">Respondendo a um desafio de autorização</span><span class="sxs-lookup"><span data-stu-id="7931a-196">Responding to an authorization challenge</span></span>

<span data-ttu-id="7931a-197">Siga as etapas a seguir para processar uma notificação do ciclo de vida do desafio de autorização.</span><span class="sxs-lookup"><span data-stu-id="7931a-197">Take the following steps to process an authorization challenge lifecycle notification.</span></span> <span data-ttu-id="7931a-198">As duas primeiras etapas de reconhecimento e validação da notificação do ciclo de vida são semelhantes a [resposta a uma notificação de alteração de recursos](webhooks.md#processing-the-change-notification).</span><span class="sxs-lookup"><span data-stu-id="7931a-198">The first two steps of acknowledging and validating the lifecycle notification is similar to [responding to a resource change notification](webhooks.md#processing-the-change-notification).</span></span>

1. <span data-ttu-id="7931a-199">Confirme o recebimento da notificação do ciclo de vida, respondendo à chamada para POSTAGEM com `HTTP 202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="7931a-199">Acknowledge the receipt of the lifecycle notification, by responding to the POST call with `HTTP 202 Accepted`.</span></span>
2. <span data-ttu-id="7931a-200">Valide a autenticidade da notificação do ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="7931a-200">Validate the authenticity of the lifecycle notification.</span></span> <span data-ttu-id="7931a-201">Mais detalhes [abaixo](#validating-the-authenticity-of-notifications).</span><span class="sxs-lookup"><span data-stu-id="7931a-201">Further details [below](#validating-the-authenticity-of-notifications).</span></span>
3. <span data-ttu-id="7931a-202">Certifique-se de que o aplicativo tenha um token de acesso válido para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="7931a-202">Ensure the app has a valid access token to take the next step.</span></span> 

    <span data-ttu-id="7931a-203">Se você estiver usando uma das [bibliotecas de autenticação](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), a biblioteca fará isso para você ao reutilizar um token de cache válido ou obtendo um novo token ao pedir ao usuário para fazer logon novamente com uma nova senha.</span><span class="sxs-lookup"><span data-stu-id="7931a-203">If you are using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), the library handles this for you by either reusing a valid cached token, or obtaining a new token from prompting the user to log in again with a new password.</span></span> <span data-ttu-id="7931a-204">Entretanto, a obtenção de um novo token pode falhar, pois as condições de acesso podem ser alteradas e o usuário não poderá mais acessar os dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="7931a-204">However, obtaining a new token may fail, since the conditions of access may have changed, and the user may no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="7931a-205">Chamar uma das duas APIs a seguir.</span><span class="sxs-lookup"><span data-stu-id="7931a-205">Call either of the following two APIs.</span></span> <span data-ttu-id="7931a-206">Se a chamada da API for bem-sucedida, o fluxo de notificação de mudança será retomado.</span><span class="sxs-lookup"><span data-stu-id="7931a-206">If the API call succeeds, the change notification flow resumes.</span></span>

    - <span data-ttu-id="7931a-207">Chame a ação `/reauthorize` para autorizar novamente a assinatura sem estender a data de vencimento:</span><span class="sxs-lookup"><span data-stu-id="7931a-207">Call the `/reauthorize` action to re-authorize the subscription without extending its expiration date:</span></span>
        ```http
        POST  https://graph.microsoft.com/beta/subscriptions/{id}/reauthorize
        Content-type: application/json
        ```
    - <span data-ttu-id="7931a-208">Execute uma ação de renovação regular para autorizar novamente e renova a assinatura ao mesmo tempo:</span><span class="sxs-lookup"><span data-stu-id="7931a-208">Perform a regular renew action to re-authorize and renew the subscription at the same time:</span></span>
        ```http
        PATCH https://graph.microsoft.com/beta/subscriptions/{id}
        Content-Type: application/json

        {
           "expirationDateTime": "2019-09-21T11:00:00.0000000Z"
        }
        ```

      <span data-ttu-id="7931a-209">A renovação pode falhar, porque as verificações de autorização realizadas pelo sistema podem recusar o aplicativo ou o acesso do usuário ao recurso.</span><span class="sxs-lookup"><span data-stu-id="7931a-209">Renewing may fail, because the authorization checks performed by the system may deny the app or the user access to the resource.</span></span> <span data-ttu-id="7931a-210">Pode ser necessário que o aplicativo obtenha um novo token de acesso do usuário para autorizar novamente com êxito uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="7931a-210">It may be necessary for the app to obtain a new access token from the user to successfully re-authorize a subscription.</span></span> 
      
      <span data-ttu-id="7931a-211">Você pode tentar essa ações mais tarde, a qualquer momento e obter êxito se as condições de acesso mudarem.</span><span class="sxs-lookup"><span data-stu-id="7931a-211">You may retry these actions later, at any time, and succeed if the conditions of access change.</span></span> <span data-ttu-id="7931a-212">Quaisquer notificações sobre alterações de recursos que ocorram entre o momento em que a notificação do ciclo de vida foi enviada e o momento em que o aplicativo eventualmente recria a assinatura com êxito serão perdidas.</span><span class="sxs-lookup"><span data-stu-id="7931a-212">Any notifications about resource changes that happen between the time the lifecycle notification was sent, and the time when the app eventually re-creates the subscription successfully, would be lost.</span></span> <span data-ttu-id="7931a-213">Nesses casos, o aplicativo deve buscar essas mudanças separadamente.</span><span class="sxs-lookup"><span data-stu-id="7931a-213">In such cases, the app should separately fetch those changes.</span></span>

### <a name="tips"></a><span data-ttu-id="7931a-214">Dicas </span><span class="sxs-lookup"><span data-stu-id="7931a-214">Tips</span></span>

<span data-ttu-id="7931a-215">Lembre-se do seguinte:</span><span class="sxs-lookup"><span data-stu-id="7931a-215">Keep the following in mind:</span></span>

1. <span data-ttu-id="7931a-216">Os desafios de autorização não substituem a necessidade de renova uma assinatura de alteração de recursos antes de expirar.</span><span class="sxs-lookup"><span data-stu-id="7931a-216">Authorization challenges do not replace the need to renew a resource change subscription before it expires.</span></span> 

    <span data-ttu-id="7931a-217">Embora você possa optar por renovar uma assinatura quando recebe um desafio de autorização, o Microsoft Graph pode não desafiar todas as suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="7931a-217">While you can choose to renew a subscription when you receive an authorization challenge, Microsoft Graph may not challenge all of your subscriptions.</span></span> <span data-ttu-id="7931a-218">Por exemplo, uma assinatura que não possui nenhuma atividade e não possui notificações de alterações com entrega pendente pode não sinalizar nenhum desafio para uma nova autorização do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7931a-218">For example, a subscription that does not have any activity and has no change notifications pending delivery may not signal any re-authorization challenges to your app.</span></span> <span data-ttu-id="7931a-219">Certifique-se de [renovar assinaturas](webhooks.md#renewing-a-subscription) antes de expirarem.</span><span class="sxs-lookup"><span data-stu-id="7931a-219">Make sure to [renew subscriptions](webhooks.md#renewing-a-subscription) before they expire.</span></span>

2. <span data-ttu-id="7931a-220">A frequência dos desafios de autorização está sujeita a mudanças.</span><span class="sxs-lookup"><span data-stu-id="7931a-220">The frequency of authorization challenges is subject to change.</span></span>

    <span data-ttu-id="7931a-221">Não faça suposições sobre a frequência dos desafios de autorização.</span><span class="sxs-lookup"><span data-stu-id="7931a-221">Do not make assumptions about the frequency of authorization challenges.</span></span> <span data-ttu-id="7931a-222">Essas notificações do ciclo de vida informam quando você deve executar as ações, evitando que você precise rastrear quais assinaturas requerem uma nova autorização.</span><span class="sxs-lookup"><span data-stu-id="7931a-222">These lifecycle notifications tell you when to take actions, saving you from having to track which subscriptions require re-authorization.</span></span> <span data-ttu-id="7931a-223">Esteja pronto para lidar com os desafios de autorização, desde uma vez a cada minuto para cada assinatura, até raramente apenas para algumas de suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="7931a-223">Be ready to handle authorization challenges anywhere from once a few minutes for every subscription, to rarely for only some of your subscriptions.</span></span>

### <a name="future-proof-your-code-to-handle-other-types-of-lifecycle-notifications"></a><span data-ttu-id="7931a-224">Planeje seu código para lidar com outros tipos de notificações do ciclo de vida no futuro</span><span class="sxs-lookup"><span data-stu-id="7931a-224">Future-proof your code to handle other types of lifecycle notifications</span></span>

<span data-ttu-id="7931a-225">Espere que as notificações do ciclo de vida da assinatura sejam postadas no mesmo terminal especificado por **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7931a-225">Expect subscription lifecycle notifications to be posted to the same endpoint specified by **lifecycleNotificationUrl**.</span></span> <span data-ttu-id="7931a-226">Elas são diferenciadas pela propriedade **lifecycleEvent** e podem conter um esquema e propriedades ligeiramente diferentes para atender aos cenários que resolvem.</span><span class="sxs-lookup"><span data-stu-id="7931a-226">They differentiate by the **lifecycleEvent** property and may contain slightly different schema and properties to serve the scenarios they address.</span></span>

<span data-ttu-id="7931a-227">Implemente seu código antecipando novos tipos de notificações do ciclo de vida:</span><span class="sxs-lookup"><span data-stu-id="7931a-227">Implement your code in anticipation of new types of lifecycle notifications:</span></span>

1. <span data-ttu-id="7931a-228">Use a propriedade **lifecycleEvent** para identificar o tipo de notificação para determinar a resposta adequada.</span><span class="sxs-lookup"><span data-stu-id="7931a-228">Use the **lifecycleEvent** property to identify the type of notification so to determine the appropriate response.</span></span> <span data-ttu-id="7931a-229">Por exemplo, procure a `"lifecycleEvent": "reauthorizationRequired"` propriedade para identificar um evento específico e tratá-lo.</span><span class="sxs-lookup"><span data-stu-id="7931a-229">For example, look for the `"lifecycleEvent": "reauthorizationRequired"` property to identify a specific event, and handle it.</span></span>

1. <span data-ttu-id="7931a-230">Registre todos os eventos do ciclo de vida que o seu aplicativo não reconheça para tomar conhecimento.</span><span class="sxs-lookup"><span data-stu-id="7931a-230">Log any lifecycle events that your app does not recognize to gain awareness.</span></span>

1. <span data-ttu-id="7931a-231">Assine o [Blog do Microsoft Graph Developer](https://developer.microsoft.com/graph/blogs/) para assistir a anúncios de notificações do ciclo de vida de novos cenários.</span><span class="sxs-lookup"><span data-stu-id="7931a-231">Subscribe to the [Microsoft Graph Developer Blog](https://developer.microsoft.com/graph/blogs/) to watch for announcements of lifecycle notifications for new scenarios.</span></span>

1. <span data-ttu-id="7931a-232">Consulte a documentação relacionada para obter as novas notificações do ciclo de vida e implemente o suporte para elas, conforme apropriado.</span><span class="sxs-lookup"><span data-stu-id="7931a-232">Look up related documentation for new lifecycle notifications and implement support for them as appropriate.</span></span>

## <a name="validating-the-authenticity-of-notifications"></a><span data-ttu-id="7931a-233">Validando a autenticidade das notificações</span><span class="sxs-lookup"><span data-stu-id="7931a-233">Validating the authenticity of notifications</span></span>

<span data-ttu-id="7931a-234">Os aplicativos geralmente executam a lógica comercial com base nos dados de recursos incluídos nas notificações de alterações.</span><span class="sxs-lookup"><span data-stu-id="7931a-234">Apps often execute business logic based on resource data included in change notifications.</span></span> <span data-ttu-id="7931a-235">Em primeiro lugar é importante verificar a autenticidade de cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="7931a-235">Having first verified the authenticity of each change notification is important.</span></span> <span data-ttu-id="7931a-236">Caso contrário, um terceiro poderá forjar o seu aplicativo com falsas notificações de alteração, fazê-lo executar sua lógica comercial incorretamente e levá-lo a um problema de segurança.</span><span class="sxs-lookup"><span data-stu-id="7931a-236">Otherwise, a third party could spoof your app with false change notifications, make it execute its business logic incorrectly, and lead to a security incident.</span></span>

<span data-ttu-id="7931a-237">Para notificações básicas de alterações que não contêm dados de recursos, simplesmente valide-as com base no valor **clientState** conforme descrito [aqui](webhooks.md#processing-the-change-notification).</span><span class="sxs-lookup"><span data-stu-id="7931a-237">For basic change notifications which do not contain resource data, simply validate them based on the **clientState** value as described [here](webhooks.md#processing-the-change-notification).</span></span> <span data-ttu-id="7931a-238">Isso é aceitável, uma vez que você pode fazer chamadas confiáveis subsequentes do Microsoft Graph para obter acesso ao dados do recurso, portanto, o impacto das tentativas de falsificação é limitado.</span><span class="sxs-lookup"><span data-stu-id="7931a-238">This is acceptable, as you can make subsequent trusted Microsoft Graph calls to get access to resource data, and therefore the impact of any spoofing attempts is limited.</span></span> 

<span data-ttu-id="7931a-239">Para notificações de alteração que entregam dados de recursos, execute uma validação mais completa antes de processar os dados.</span><span class="sxs-lookup"><span data-stu-id="7931a-239">For change notifications that deliver resource data, perform a more thorough validation before processing the data.</span></span>

<span data-ttu-id="7931a-240">Nesta seção:</span><span class="sxs-lookup"><span data-stu-id="7931a-240">In this section:</span></span>

- [<span data-ttu-id="7931a-241">Tokens de validação na notificação de alteração</span><span class="sxs-lookup"><span data-stu-id="7931a-241">Validation tokens in the change notification</span></span>](#validation-tokens-in-the-change-notification)
- [<span data-ttu-id="7931a-242">Como validar</span><span class="sxs-lookup"><span data-stu-id="7931a-242">How to validate</span></span>](#how-to-validate)
- [<span data-ttu-id="7931a-243">Exemplo de token JWT</span><span class="sxs-lookup"><span data-stu-id="7931a-243">Example JWT token</span></span>](#example-jwt-token)

### <a name="validation-tokens-in-the-change-notification"></a><span data-ttu-id="7931a-244">Tokens de validação na notificação de alteração</span><span class="sxs-lookup"><span data-stu-id="7931a-244">Validation tokens in the change notification</span></span>

<span data-ttu-id="7931a-245">Uma notificação de alteração com os dados do recurso contém uma propriedade adicional, \*\* validationTokens \*\*, com uma matriz de tokens JWT gerados pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7931a-245">A change notification with resource data contains an additional property, **validationTokens**, which contains an array of JWT tokens generated by Microsoft Graph.</span></span> <span data-ttu-id="7931a-246">O Microsoft Graph gera um token único para cada aplicativo distinto e um par de locatários onde existe um item no conunto **valor**.</span><span class="sxs-lookup"><span data-stu-id="7931a-246">Microsoft Graph generates a single token for each distinct app and tenant pair for whom there is an item in the **value** array.</span></span> <span data-ttu-id="7931a-247">Tenha em mente que as notificações de alterações podem conter uma mistura de itens para vários aplicativos e locatários que fizeram assinatura usando o mesmo **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7931a-247">Keep in mind that change notifications may contain a mix of items for various apps and tenants that subscribed using the same **notificationUrl**.</span></span>

<span data-ttu-id="7931a-248">No exemplo a seguir, a notificação de alteração contém dois itens para o mesmo aplicativo e para dois locatários diferentes, portanto, o conjunto **validationTokens** contém dois tokens que precisam ser validados.</span><span class="sxs-lookup"><span data-stu-id="7931a-248">In the following example, the change notification contains two items for the same app, and for two different tenants, therefore the **validationTokens** array contains two tokens that need to be validated.</span></span>

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

> <span data-ttu-id="7931a-249">**Nota:** para obter uma descrição completa dos dados enviados quando as notificações de alterações são entregues, consulte [ changeNotificationCollection ](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="7931a-249">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="how-to-validate"></a><span data-ttu-id="7931a-250">Como validar</span><span class="sxs-lookup"><span data-stu-id="7931a-250">How to validate</span></span>

<span data-ttu-id="7931a-251">Se você não conhece a validação de token, consulte [Princípios de Validação de Token](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) para obter uma visão geral.</span><span class="sxs-lookup"><span data-stu-id="7931a-251">If you're new to token validation, see [Principles of Token Validation](http://www.cloudidentity.com/blog/2014/03/03/principles-of-token-validation/) for an overview.</span></span> <span data-ttu-id="7931a-252">Use um SDK, como a [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) biblioteca para .NET ou uma biblioteca de terceiros para uma plataforma diferente.</span><span class="sxs-lookup"><span data-stu-id="7931a-252">Use an SDK, such as the [System.IdentityModel.Tokens.Jwt](https://www.nuget.org/packages/System.IdentityModel.Tokens.Jwt/) library for .NET, or a third-party library for a different platform.</span></span>

<span data-ttu-id="7931a-253">Fique atento ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="7931a-253">Be mindful of the following:</span></span> 

- <span data-ttu-id="7931a-254">Certifique-se de sempre enviar um `HTTP 202 Accepted` código de status como parte da resposta à notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="7931a-254">Make sure to always send an `HTTP 202 Accepted` status code as part of the response to the change notification.</span></span> 
- <span data-ttu-id="7931a-255">Faça isso antes da validação da notificações de alteração (por exemplo, se você armazena as notificações de alteração em filas para processamento posterior) ou depois (se você processá-las em tempo real), mesmo se a validação falhar.</span><span class="sxs-lookup"><span data-stu-id="7931a-255">Do that before validating the change notification (for example, if you store change notifications in queues for later processing) or after (if you process them on the fly), even if validation failed.</span></span>
- <span data-ttu-id="7931a-256">A aceitação de uma notificação de alteração evita novas tentativas desnecessárias de entrega e também impede que possíveis atores invasores descubram se foram ou não aprovados na validação.</span><span class="sxs-lookup"><span data-stu-id="7931a-256">Accepting a change notification prevents unnecessary delivery retries and it also prevents any potential rogue actors from finding out if they passed or failed validation.</span></span> <span data-ttu-id="7931a-257">Você sempre pode optar por ignorar uma notificação de alteração inválida após aceitá-la.</span><span class="sxs-lookup"><span data-stu-id="7931a-257">You can always choose to ignore an invalid change notification after you have accepted it.</span></span>

<span data-ttu-id="7931a-258">Especificamente, realize a validação em todos os tokens JWT na coleção **validationTokens**.</span><span class="sxs-lookup"><span data-stu-id="7931a-258">In particular, perform validation on every JWT token in the **validationTokens** collection.</span></span> <span data-ttu-id="7931a-259">Se algum token falhar, considere a notificação de alteração suspeita e investigue mais.</span><span class="sxs-lookup"><span data-stu-id="7931a-259">If any tokens fail, consider the change notification suspicious and investigate further.</span></span> 

<span data-ttu-id="7931a-260">Use as etapas a seguir para validar tokens e aplicativos que geram tokens:</span><span class="sxs-lookup"><span data-stu-id="7931a-260">Use the following steps to validate tokens and apps that generate tokens:</span></span>

1. <span data-ttu-id="7931a-261">Valide se o token não expirou.</span><span class="sxs-lookup"><span data-stu-id="7931a-261">Validate that the token has not expired.</span></span>

2. <span data-ttu-id="7931a-262">Valide se o token não foi adulterado e foi emitido pela autoridade esperada, o Active Directory do Microsoft Azure:</span><span class="sxs-lookup"><span data-stu-id="7931a-262">Validate the token has not been tampered with and was issued by the expected authority, Microsoft Azure Active Directory:</span></span>

    - <span data-ttu-id="7931a-263">Obtenha as chaves de assinatura do ponto de extremidade de configuração comum: `https://login.microsoftonline.com/common/.well-known/openid-configuration`.</span><span class="sxs-lookup"><span data-stu-id="7931a-263">Obtain the signing keys from the common configuration endpoint: `https://login.microsoftonline.com/common/.well-known/openid-configuration`.</span></span> <span data-ttu-id="7931a-264">Essa configuração é armazenada em cache pelo aplicativo por um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="7931a-264">This configuration is cached by your app for a period of time.</span></span> <span data-ttu-id="7931a-265">Lembre-se de que a configuração é atualizada frequentemente, uma vez que as chaves de assinatura são giradas diariamente.</span><span class="sxs-lookup"><span data-stu-id="7931a-265">Be aware that the configuration is updated frequently as signing keys are rotated daily.</span></span>
    - <span data-ttu-id="7931a-266">Verifique a assinatura do token JWT usando essas chaves.</span><span class="sxs-lookup"><span data-stu-id="7931a-266">Verify the signature of the JWT token using those keys.</span></span>

    <span data-ttu-id="7931a-267">Não aceite tokens emitidos por outra autoridade.</span><span class="sxs-lookup"><span data-stu-id="7931a-267">Do not accept tokens issued by any other authority.</span></span>

3. <span data-ttu-id="7931a-268">Valide se o token foi emitido para o aplicativo que está inscrito para alterar as notificações.</span><span class="sxs-lookup"><span data-stu-id="7931a-268">Validate that the token was issued for your app that is subscribing to change notifications.</span></span>

    <span data-ttu-id="7931a-269">As etapas a seguir fazem parte da lógica de validação padrão nas bibliotecas de token JWT e podem ser tipicamente executadas como uma única chamada de função.</span><span class="sxs-lookup"><span data-stu-id="7931a-269">The following steps are part of standard validation logic in JWT token libraries and can typically be executed as a single function call.</span></span> 
    - <span data-ttu-id="7931a-270">Valide a “audiência” no token que corresponde à ID do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7931a-270">Validate the "audience" in the token matches your app ID.</span></span>
    - <span data-ttu-id="7931a-271">Se você tiver mais de um aplicativo recebendo notificações de alterações, verifique a existencia de vários IDs.</span><span class="sxs-lookup"><span data-stu-id="7931a-271">If you have more than one app receiving change notifications, make sure to check for multiple IDs.</span></span>


4. <span data-ttu-id="7931a-272">**Crítico**: valide se o aplicativo que gerou o token representa o distribuidor de notificação de alteração do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7931a-272">**Critical**: Validate that the app that generated the token represents the Microsoft Graph change notification publisher.</span></span> 

    - <span data-ttu-id="7931a-273">Verifique se a propriedade **appid** no token corresponde ao valor esperado de `0bf30f3b-4a52-48df-9a82-234910c4a086`.</span><span class="sxs-lookup"><span data-stu-id="7931a-273">Check that the **appid** property in the token matches the expected value of `0bf30f3b-4a52-48df-9a82-234910c4a086`.</span></span>
    - <span data-ttu-id="7931a-274">Isso garante que as notificações de alteração não sejam enviadas por um aplicativo diferente do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7931a-274">This ensures that change notifications are not sent by a different app that is not Microsoft Graph.</span></span>


### <a name="example-jwt-token"></a><span data-ttu-id="7931a-275">Exemplo de Token JWT </span><span class="sxs-lookup"><span data-stu-id="7931a-275">Example JWT token</span></span>

<span data-ttu-id="7931a-276">A seguir, é apresentado um exemplo das propriedades incluídas no token JWT que são necessárias para validação.</span><span class="sxs-lookup"><span data-stu-id="7931a-276">The following is an example of the properties included in the JWT token that are needed for validation.</span></span>

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

### <a name="example-verifying-validation-tokens"></a><span data-ttu-id="7931a-277">Exemplo: verificação de tokens de validação</span><span class="sxs-lookup"><span data-stu-id="7931a-277">Example: Verifying validation tokens</span></span>

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
<span data-ttu-id="7931a-278">Para que o exemplo do Java funcione, também será necessário implementar o `JwkKeyResolver`.</span><span class="sxs-lookup"><span data-stu-id="7931a-278">For the Java sample to work, you will also need to implement the `JwkKeyResolver`.</span></span>  
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

## <a name="decrypting-resource-data-from-change-notifications"></a><span data-ttu-id="7931a-279">Descriptografar os dados de recursos de notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="7931a-279">Decrypting resource data from change notifications</span></span>

<span data-ttu-id="7931a-280">A propriedade **resourceData** de uma notificação de alteração inclui apenas o ID básico e as informações do tipo de uma instância de recurso.</span><span class="sxs-lookup"><span data-stu-id="7931a-280">The **resourceData** property of a change notification includes only the basic ID and type information of a resource instance.</span></span> <span data-ttu-id="7931a-281">A propriedade **encryptedData** contém os dados de recursos completos, criptografados pelo Microsoft Graph usando a chave pública fornecida na assinatura.</span><span class="sxs-lookup"><span data-stu-id="7931a-281">The **encryptedData** property contains the full resource data, encrypted by Microsoft Graph using the public key provided in the subscription.</span></span> <span data-ttu-id="7931a-282">A propriedade também contém valores necessários para verificação e descriptografia.</span><span class="sxs-lookup"><span data-stu-id="7931a-282">The property also contains values required for verification and decryption.</span></span> <span data-ttu-id="7931a-283">Isso é feito para aumentar a segurança dos dados do cliente acessados por meio de notificações de alterações.</span><span class="sxs-lookup"><span data-stu-id="7931a-283">This is done to increase the security of customer data accessed via change notifications.</span></span> <span data-ttu-id="7931a-284">É da sua responsabilidade proteger a chave privada para garantir que os dados do cliente não sejam decriptados por terceiros, mesmo que eles consigam interceptar as notificações de alteração originais.</span><span class="sxs-lookup"><span data-stu-id="7931a-284">It is your responsibility to secure the private key to ensure that customer data cannot be decrypted by a third party, even if they manage to intercept the original change notifications.</span></span>

<span data-ttu-id="7931a-285">Nesta seção:</span><span class="sxs-lookup"><span data-stu-id="7931a-285">In this section:</span></span>

- [<span data-ttu-id="7931a-286">Gerenciar as chaves de criptografia</span><span class="sxs-lookup"><span data-stu-id="7931a-286">Managing encryption keys</span></span>](#managing-encryption-keys)
- [<span data-ttu-id="7931a-287">Descriptografar os dados de recursos</span><span class="sxs-lookup"><span data-stu-id="7931a-287">Decrypting resource data</span></span>](#decrypting-resource-data)
- [<span data-ttu-id="7931a-288">Exemplo: descriptografar uma notificação com dados de recursos criptografados</span><span class="sxs-lookup"><span data-stu-id="7931a-288">Example: decrypting a notification with encrypted resource data</span></span>](#example-decrypting-a-notification-with-encrypted-resource-data)

### <a name="managing-encryption-keys"></a><span data-ttu-id="7931a-289">Gerenciar as chaves de criptografia</span><span class="sxs-lookup"><span data-stu-id="7931a-289">Managing encryption keys</span></span>

1. <span data-ttu-id="7931a-290">Obtenha um certificado com um par de chaves assimétricas.</span><span class="sxs-lookup"><span data-stu-id="7931a-290">Obtain a certificate with a pair of asymmetric keys.</span></span>

    - <span data-ttu-id="7931a-291">Você pode assinatura o certificado sozinho, uma vez que o Microsoft Graph não verifica o emissor do certificado e usa a chave pública somente para criptografia.</span><span class="sxs-lookup"><span data-stu-id="7931a-291">You can self-sign the certificate, since Microsoft Graph does not verify the certificate issuer, and uses the public key for only encryption.</span></span> 
    - <span data-ttu-id="7931a-292">Use o [Cofre da Chave do Azure](https://docs.microsoft.com/azure/key-vault/key-vault-whatis) como a solução para criar, girar e gerenciar certificados com segurança.</span><span class="sxs-lookup"><span data-stu-id="7931a-292">Use [Azure Key Vault](https://docs.microsoft.com/azure/key-vault/key-vault-whatis) as the solution to create, rotate, and securely manage certificates.</span></span> <span data-ttu-id="7931a-293">Cerifique-se de que as chaves atendem aos seguintes critérios:</span><span class="sxs-lookup"><span data-stu-id="7931a-293">Make sure the keys satisfy the following criteria:</span></span>

        - <span data-ttu-id="7931a-294">A chave deve ser do tipo `RSA`</span><span class="sxs-lookup"><span data-stu-id="7931a-294">The key must be of type `RSA`</span></span>
        - <span data-ttu-id="7931a-295">O tamanho da chave deve estar entre 2048 e 4096 bits</span><span class="sxs-lookup"><span data-stu-id="7931a-295">The key size must be between 2048 and 4096 bits</span></span>

2. <span data-ttu-id="7931a-296">Exportar o certificar no formato base64-encoded X.509 e **incluir apenas a chave pública**.</span><span class="sxs-lookup"><span data-stu-id="7931a-296">Export the certificate in base64-encoded X.509 format, and **include only the public key**.</span></span> 

3. <span data-ttu-id="7931a-297">Ao criar uma assinatura:</span><span class="sxs-lookup"><span data-stu-id="7931a-297">When creating a subscription:</span></span>

    - <span data-ttu-id="7931a-298">Forneça o certificado na propriedade **encryptionCertificate** usando o conteúdo base64-encoded no qual o certificado foi exportado.</span><span class="sxs-lookup"><span data-stu-id="7931a-298">Provide the certificate in the **encryptionCertificate** property, using the base64-encoded content that the certificate was exported in.</span></span>
    - <span data-ttu-id="7931a-299">Forneça seu próprio identificador na propriedade **encryptionCertificateId**.</span><span class="sxs-lookup"><span data-stu-id="7931a-299">Provide your own identifier in the **encryptionCertificateId** property.</span></span> 
  
        <span data-ttu-id="7931a-300">Esse identificador permite corresponder seus certificados às notificações de alterações recebidas e recuperar certificados do seu repositório de certificados.</span><span class="sxs-lookup"><span data-stu-id="7931a-300">This identifier allows you to match your certificates to the change notifications you receive, and to retrieve certificates from your certificate store.</span></span> <span data-ttu-id="7931a-301">O identificador pode ter no máximo 128 caracteres.</span><span class="sxs-lookup"><span data-stu-id="7931a-301">The identifier can be up to 128 characters.</span></span>

4. <span data-ttu-id="7931a-302">Gerencie com segurança a chave privada com para que seu código de processamento de notificação de alteração acesse a chave privada para decriptar os dados do recurso.</span><span class="sxs-lookup"><span data-stu-id="7931a-302">Manage the private key securely, so that your change notification processing code can access the private key to decrypt resource data.</span></span>

#### <a name="rotating-keys"></a><span data-ttu-id="7931a-303">Chaves de rotação</span><span class="sxs-lookup"><span data-stu-id="7931a-303">Rotating keys</span></span>

<span data-ttu-id="7931a-304">Para minimizar o risco de uma chave privada ser comprometida, altere periodicamente suas chaves assimétricas.</span><span class="sxs-lookup"><span data-stu-id="7931a-304">To minimize the risk of a private key becoming compromised, periodically change your asymmetric keys.</span></span> <span data-ttu-id="7931a-305">Siga estas etapas para introduzir um novo par de chaves:</span><span class="sxs-lookup"><span data-stu-id="7931a-305">Follow these steps to introduce a new pair of keys:</span></span>

1. <span data-ttu-id="7931a-306">Obtenha um novo certificado com um novo par de chaves assimétricas.</span><span class="sxs-lookup"><span data-stu-id="7931a-306">Obtain a new certificate with a new pair of asymmetric keys.</span></span> <span data-ttu-id="7931a-307">Use-o para todas as novas assinaturas sendo criadas.</span><span class="sxs-lookup"><span data-stu-id="7931a-307">Use it for all new subscriptions being created.</span></span>

2. <span data-ttu-id="7931a-308">Atualize as assinaturas existentes com a nova chave de certificado.</span><span class="sxs-lookup"><span data-stu-id="7931a-308">Update existing subscriptions with the new certificate key.</span></span>

    - <span data-ttu-id="7931a-309">Faça isso como parte da renovação da assinatura regular.</span><span class="sxs-lookup"><span data-stu-id="7931a-309">Do this as part of regular subscription renewal.</span></span> 
    - <span data-ttu-id="7931a-310">Ou enumere todas as assinaturas e forneça a chave.</span><span class="sxs-lookup"><span data-stu-id="7931a-310">Or, enumerate all subscriptions and provide the key.</span></span> <span data-ttu-id="7931a-311">Use a [operação PATCH na assinatura](/graph/api/subscription-update?view=graph-rest-1.0) e atualize as propriedades **encryptionCertificate** e **encryptionCertificateId**.</span><span class="sxs-lookup"><span data-stu-id="7931a-311">Use the [PATCH operation on the subscription](/graph/api/subscription-update?view=graph-rest-1.0) and update the **encryptionCertificate** and **encryptionCertificateId** properties.</span></span>

3. <span data-ttu-id="7931a-312">Lembre-se do seguinte:</span><span class="sxs-lookup"><span data-stu-id="7931a-312">Keep in mind the following:</span></span>
    - <span data-ttu-id="7931a-313">Por um período de tempo, o certificado antigo ainda pode ser usado para criptografia.</span><span class="sxs-lookup"><span data-stu-id="7931a-313">For a period of time, the old certificate may still be used for encryption.</span></span> <span data-ttu-id="7931a-314">Seu aplicativo deve ter acesso a certificados novos e antigos para poder descriptografar o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7931a-314">Your app must have access to both old and new certificates to be able to decrypt content.</span></span>
    - <span data-ttu-id="7931a-315">Use a propriedade **encryptionCertificateId** em cada notificação de alteração para identificar a chave correta a ser utilizada.</span><span class="sxs-lookup"><span data-stu-id="7931a-315">Use the **encryptionCertificateId** property in each change notification to identify the correct key to use.</span></span>
    - <span data-ttu-id="7931a-316">Descarte o certificado antigo somente quando não houver notificações de alterações recentes fazendo referência a ele.</span><span class="sxs-lookup"><span data-stu-id="7931a-316">Discard of the old certificate only when you have seen no recent change notifications referencing it.</span></span>

### <a name="decrypting-resource-data"></a><span data-ttu-id="7931a-317">Descriptografar dados de recursos</span><span class="sxs-lookup"><span data-stu-id="7931a-317">Decrypting resource data</span></span>

<span data-ttu-id="7931a-318">Para otimizar o desempenho, o Microsoft Graph usa um processo de criptografia de duas etapas:</span><span class="sxs-lookup"><span data-stu-id="7931a-318">To optimize performance, Microsoft Graph uses a two-step encryption process:</span></span>
  - <span data-ttu-id="7931a-319">Ele gera uma chave simétrica de uso único e a usa para criptografar os dados do recurso.</span><span class="sxs-lookup"><span data-stu-id="7931a-319">It generates a single use symmetric key, and uses it to encrypt resource data.</span></span>
  - <span data-ttu-id="7931a-320">Ele usa a chave pública assimétrica (que você forneceu ao fazer a assinatura) para criptografar a chave simétrica e a incluir em cada notificação de alteração desta assinatura.</span><span class="sxs-lookup"><span data-stu-id="7931a-320">It uses the public asymmetric key (that you provided when subscribing) to encrypt the symmetric key and includes it in each change notification of that subscription.</span></span>

<span data-ttu-id="7931a-321">Sempre assuma que a chave simétrica é diferente para cada item na notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="7931a-321">Always assume that the symmetric key is different for each item in the change notification.</span></span>

<span data-ttu-id="7931a-322">Para decriptar os dados de recursos, o seu aplicativo deve executar as etapas inversas, usando as propriedades **encryptedContent** em cada notificação de alteração:</span><span class="sxs-lookup"><span data-stu-id="7931a-322">To decrypt resource data, your app should perform the reverse steps, using the properties under **encryptedContent** in each change notification:</span></span>

1. <span data-ttu-id="7931a-323">Use a propriedade **encryptionCertificateId** para identificar o certificado a ser usado.</span><span class="sxs-lookup"><span data-stu-id="7931a-323">Use the **encryptionCertificateId** property to identify the certificate to use.</span></span>

2. <span data-ttu-id="7931a-324">Inicialize um componente criptográfico da RSA (como o .NET [RSACryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) com a chave privada.</span><span class="sxs-lookup"><span data-stu-id="7931a-324">Initialize an RSA cryptographic component (such as the .NET [RSACryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.rsacryptoserviceprovider.decrypt?view=netframework-4.8)) with the private key.</span></span>

3. <span data-ttu-id="7931a-325">Decripte a chave simétrica entregue na propriedade **dataKey** de cada item na notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="7931a-325">Decrypt the symmetric key delivered in the **dataKey** property of each item in the change notification.</span></span>

    <span data-ttu-id="7931a-326">Use o Preenchimento de Criptografia Assimétrica Ideal (OAEP) para o algoritmo de descriptografia.</span><span class="sxs-lookup"><span data-stu-id="7931a-326">Use Optimal Asymmetric Encryption Padding (OAEP) for the decryption algorithm.</span></span>

4. <span data-ttu-id="7931a-327">Use a chave simétrica para calcular a assinatura HMAC-SHA256 do valor em **dados**.</span><span class="sxs-lookup"><span data-stu-id="7931a-327">Use the symmetric key to calculate the HMAC-SHA256 signature of the value in **data**.</span></span>
  
    <span data-ttu-id="7931a-328">Compare-o com o valor em **dataSignature**.</span><span class="sxs-lookup"><span data-stu-id="7931a-328">Compare it to the value in **dataSignature**.</span></span> <span data-ttu-id="7931a-329">Se eles não corresponderem, considere que a carga foi adulterada e não a descriptografe.</span><span class="sxs-lookup"><span data-stu-id="7931a-329">If they do not match, assume the payload has been tampered with and do not decrypt it.</span></span>

5. <span data-ttu-id="7931a-330">Use a chave simétrica com a criptografia AES (como o .NET [AesCryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) para descriptografar o conteúdo em **dados**.</span><span class="sxs-lookup"><span data-stu-id="7931a-330">Use the symmetric key with an Advanced Encryption Standard (AES) (such as the .NET [AesCryptoServiceProvider](https://docs.microsoft.com/dotnet/api/system.security.cryptography.aescryptoserviceprovider?view=netframework-4.8)) to decrypt the content in **data**.</span></span>

    - <span data-ttu-id="7931a-331">Use os seguintes parâmetros de descriptografia para o algoritmo AES:</span><span class="sxs-lookup"><span data-stu-id="7931a-331">Use the following decryption parameters for the AES algorithm:</span></span>

        - <span data-ttu-id="7931a-332">Preenchimento: PKCS7</span><span class="sxs-lookup"><span data-stu-id="7931a-332">Padding: PKCS7</span></span>
        - <span data-ttu-id="7931a-333">Modo de criptografia: CBC</span><span class="sxs-lookup"><span data-stu-id="7931a-333">Cipher mode: CBC</span></span>
    - <span data-ttu-id="7931a-334">Defina o “vetor de inicialização” copiando os primeiros 16 bytes da chave simétrica usada para descriptografia.</span><span class="sxs-lookup"><span data-stu-id="7931a-334">Set the "initialization vector" by copying the first 16 bytes of the symmetric key used for decryption.</span></span>

6. <span data-ttu-id="7931a-335">O valor decriptado é uma sequência JSON que representa a instância do recurso na notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="7931a-335">The decrypted value is a JSON string that represents the resource instance in the change notification.</span></span>


### <a name="example-decrypting-a-notification-with-encrypted-resource-data"></a><span data-ttu-id="7931a-336">Exemplo: decriptando uma notificação com dados de recurso criptografados</span><span class="sxs-lookup"><span data-stu-id="7931a-336">Example: decrypting a notification with encrypted resource data</span></span>

<span data-ttu-id="7931a-337">A seguir, é apresentado um exemplo de notificação de alteração que inclui valores de propriedade criptografados de uma **chatMessage** instância em uma mensagem de canal.</span><span class="sxs-lookup"><span data-stu-id="7931a-337">The following is an example change notification that includes encrypted property values of a **chatMessage** instance in a channel message.</span></span> <span data-ttu-id="7931a-338">A instância é especificada pelo `@odata.id` valor.</span><span class="sxs-lookup"><span data-stu-id="7931a-338">The instance is specified by the `@odata.id` value.</span></span>

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

> <span data-ttu-id="7931a-339">**Nota:** para obter uma descrição completa dos dados enviados quando as notificações de alterações são entregues, consulte [ changeNotificationCollection ](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="7931a-339">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>


<span data-ttu-id="7931a-340">A seção contém alguns trechos de código úteis que usam C# e .NET em cada etapa da descriptografia.</span><span class="sxs-lookup"><span data-stu-id="7931a-340">This section contains some useful code snippets that use C# and .NET for each stage of decryption.</span></span>

#### <a name="decrypt-the-symmetric-key"></a><span data-ttu-id="7931a-341">Descriptografar a chave simétrica</span><span class="sxs-lookup"><span data-stu-id="7931a-341">Decrypt the symmetric key</span></span>

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

#### <a name="compare-data-signature-using-hmac-sha256"></a><span data-ttu-id="7931a-342">Comparar assinatura de dados usando HMAC-SHA256</span><span class="sxs-lookup"><span data-stu-id="7931a-342">Compare data signature using HMAC-SHA256</span></span>

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

#### <a name="decrypt-the-resource-data-content"></a><span data-ttu-id="7931a-343">Descriptografar o conteúdo dos dados de recursos</span><span class="sxs-lookup"><span data-stu-id="7931a-343">Decrypt the resource data content</span></span>

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

## <a name="see-also"></a><span data-ttu-id="7931a-344">Confira também</span><span class="sxs-lookup"><span data-stu-id="7931a-344">See also</span></span>

- [<span data-ttu-id="7931a-345">Configurar notificações para alterações nos dados de usuário</span><span class="sxs-lookup"><span data-stu-id="7931a-345">Set up notifications for changes in user data</span></span>](webhooks.md)
- [<span data-ttu-id="7931a-346">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="7931a-346">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-beta)
- [<span data-ttu-id="7931a-347">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="7931a-347">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="7931a-348">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="7931a-348">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="7931a-349">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="7931a-349">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
