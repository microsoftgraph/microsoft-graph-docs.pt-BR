---
title: Reduzir assinaturas ausentes e alterar notificações
description: Os aplicativos que estão se inscrevendo para alterar as notificações de recursos podem ter suas assinaturas removidas e perder algumas notificações de alteração. Os aplicativos devem implementar a lógica para detectar e recuperar da perda e retomar o fluxo de notificação de alteração contínua.
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 2c8cd8d38c0e089e98bc62aa37104b979f33ab9a
ms.sourcegitcommit: 70e09ebbf67f49a0c64ab7a275e751f8a68b8696
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/27/2020
ms.locfileid: "48771759"
---
# <a name="reduce-missing-subscriptions-and-change-notifications"></a><span data-ttu-id="10df9-104">Reduzir assinaturas ausentes e alterar notificações</span><span class="sxs-lookup"><span data-stu-id="10df9-104">Reduce missing subscriptions and change notifications</span></span>

<span data-ttu-id="10df9-105">Os aplicativos que estão se inscrevendo para alterar as notificações de recursos podem ter suas assinaturas removidas e perder algumas notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="10df9-105">Apps subscribing to change notifications might get their subscriptions removed and miss some change notifications.</span></span> <span data-ttu-id="10df9-106">Os aplicativos devem implementar a lógica para detectar e recuperar da perda e retomar o fluxo de notificação de alteração contínua.</span><span class="sxs-lookup"><span data-stu-id="10df9-106">Apps should implement logic to detect and recover from the loss, and resume a continuous change notification flow.</span></span>

<span data-ttu-id="10df9-107">Determinados eventos podem fazer que a assinatura seja removida.</span><span class="sxs-lookup"><span data-stu-id="10df9-107">Certain events can cause a subscription to be removed.</span></span> <span data-ttu-id="10df9-108">Esses eventos incluem:</span><span class="sxs-lookup"><span data-stu-id="10df9-108">These events include:</span></span>

- <span data-ttu-id="10df9-109">A senha do usuário foi redefinida</span><span class="sxs-lookup"><span data-stu-id="10df9-109">User's password has been reset</span></span>
- <span data-ttu-id="10df9-110">Dispositivo do usuário está fora de conformidade</span><span class="sxs-lookup"><span data-stu-id="10df9-110">User's device is out of compliance</span></span>
-   <span data-ttu-id="10df9-111">Conta do usuário foi revogada</span><span class="sxs-lookup"><span data-stu-id="10df9-111">User's account has been revoked</span></span>

<span data-ttu-id="10df9-112">Quando ocorre um evento, o Microsoft Graph envia uma notificação de ciclo de vida especial `subscriptionRemoved`.</span><span class="sxs-lookup"><span data-stu-id="10df9-112">When such an event happens, Microsoft Graph sends a special lifecycle notification, `subscriptionRemoved`.</span></span>

<span data-ttu-id="10df9-113">O Microsoft Graph também envia outra notificação do ciclo de vida, `missed`, caso não seja possível entregar uma notificação de alteração a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="10df9-113">Microsoft Graph also sends another lifecycle notification, `missed`, if a change notification cannot be delivered to an app.</span></span>

<span data-ttu-id="10df9-114">Uma assinatura de um aplicativo para modificar as notificações deve ouvir os sinais `subscriptionRemoved` e `missed` e fazer o seguinte:</span><span class="sxs-lookup"><span data-stu-id="10df9-114">An app subscribing to change notifications should listen to the `subscriptionRemoved` and `missed` signals and do the following:</span></span>

- <span data-ttu-id="10df9-115">Após receber uma notificação de `subscriptionRemoved` ciclo de vida, o aplicativo deve recriar a assinatura para manter um fluxo contínuo.</span><span class="sxs-lookup"><span data-stu-id="10df9-115">Upon receiving a `subscriptionRemoved` lifecycle notification, the app should recreate the subscription in order to maintain a continuous flow.</span></span>
- <span data-ttu-id="10df9-116">Ao receber uma notificação de `missed` ciclo de vida, o aplicativo deve ressincronizar os dados de recurso usando o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="10df9-116">On receiving a `missed` lifecycle notification, the app should resynchronize resource data using Microsoft Graph.</span></span>

<span data-ttu-id="10df9-117">Para receber notificações de ciclo de vida, você pode usar o ponto de extremidade existente **notificationUrl** que já recebe notificações de alteração, ou você pode registrar um **lifecycleNotificationUrl** separado para receber `subscriptionRemoved` e `missed` notificações de ciclo de vida em um ponto de extremidade separado.</span><span class="sxs-lookup"><span data-stu-id="10df9-117">To receive lifecycle notifications, you can use the existing **notificationUrl** endpoint that already receives change notifications, or you can register a separate **lifecycleNotificationUrl** to receive `subscriptionRemoved` and `missed` lifecycle notifications in a separate endpoint.</span></span>

<span data-ttu-id="10df9-118">As notificações de ciclo de vida têm suporte para as assinaturas criadas nesses tipos de recurso:</span><span class="sxs-lookup"><span data-stu-id="10df9-118">Lifecycle notifications are supported for subscriptions created on these resource types:</span></span>

- <span data-ttu-id="10df9-119">[Mensagem][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="10df9-119">Outlook [message][]</span></span>
- <span data-ttu-id="10df9-120">[Evento][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="10df9-120">Outlook [event][]</span></span>
- <span data-ttu-id="10df9-121">[Contato][] pessoal do Outlook</span><span class="sxs-lookup"><span data-stu-id="10df9-121">Outlook personal [contact][]</span></span>
- <span data-ttu-id="10df9-122">[chatMessage][] do Teams</span><span class="sxs-lookup"><span data-stu-id="10df9-122">Teams [chatMessage][]</span></span>

<span data-ttu-id="10df9-123">Para outros tipos de recurso, você ainda poderá fornecer um `lifecycleNotificationUrl` ao criar a assinatura e o aplicativo receberá as notificações do ciclo de vida sempre que o recurso implementá-la.</span><span class="sxs-lookup"><span data-stu-id="10df9-123">For other resource types, you may still provide a `lifecycleNotificationUrl` when creating the subscription and your application will receive lifecycle notifications whenver the resource implements it.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="10df9-124">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="10df9-124">Creating a subscription</span></span>

<span data-ttu-id="10df9-125">Ao criar uma assinatura, você deve especificar um ponto de extremidade de notificação separado usando a propriedade **lifecycleNotificationUrl** .</span><span class="sxs-lookup"><span data-stu-id="10df9-125">When creating a subscription, you must specify a separate notification endpoint using the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="10df9-126">Se você especificar o ponto de extremidade, todos os tipos de atuais e futuros de notificações de ciclo de vida serão entregues lá.</span><span class="sxs-lookup"><span data-stu-id="10df9-126">If you specify the endpoint, all current and future types of lifecycle notifications will be delivered there.</span></span> <span data-ttu-id="10df9-127">Caso contrário, as notificações do ciclo de vida `subscriptionRemoved` e `missed` não serão entregues.</span><span class="sxs-lookup"><span data-stu-id="10df9-127">Otherwise, `subscriptionRemoved` and `missed` lifecycle notifications will not be delivered.</span></span> <span data-ttu-id="10df9-128">Esse ponto de extremidade pode ser o mesmo que a **notificationUrl** .</span><span class="sxs-lookup"><span data-stu-id="10df9-128">This endpoint can be the same as the **notificationUrl** .</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="10df9-129">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="10df9-129">Subscription request example</span></span>

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/users/{id}/messages",
  "expirationDateTime": "2020-03-20T11:00:00.0000000Z",
  "clientState": "<secretClientState>"
}
```
 
> [!IMPORTANT]
> <span data-ttu-id="10df9-130">Use o mesmo nome de host (FQDN) para ambas as notificações URLs.</span><span class="sxs-lookup"><span data-stu-id="10df9-130">Use the same hostname (FQDN) for both notifications URLs.</span></span> 

<span data-ttu-id="10df9-131">É necessário validar ambos os pontos de extremidade conforme descrito em [Gerenciar assinaturas](webhooks.md#managing-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="10df9-131">You need to validate both endpoints, as described in [Managing subscriptions](webhooks.md#managing-subscriptions).</span></span> <span data-ttu-id="10df9-132">Se você quiser usar a mesma URL para os dois pontos de extremidade, você receberá e responderá a duas solicitações de validação.</span><span class="sxs-lookup"><span data-stu-id="10df9-132">If you choose to use the same URL for both endpoints, you will receive and respond to two validation requests.</span></span>

> <span data-ttu-id="10df9-133">**Observação:** Não é possível atualizar (`PATCH`) as assinaturas existentes para adicionar a propriedade **lifecycleNotificationUrl** .</span><span class="sxs-lookup"><span data-stu-id="10df9-133">**Note:** You cannot update (`PATCH`) the existing subscriptions to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="10df9-134">Você deve remover essas assinaturas existentes, criar novas assinaturas e especificar a propriedade **lifecycleNotificationUrl** .</span><span class="sxs-lookup"><span data-stu-id="10df9-134">You should remove such existing subscriptions, create new subscriptions, and specify the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="10df9-135">As assinaturas existentes sem uma propriedade **lifecycleNotificationUrl** não receberão as `subscriptionRemoved` e `missed` notificações.</span><span class="sxs-lookup"><span data-stu-id="10df9-135">Existing subscriptions without a **lifecycleNotificationUrl** property will not receive the `subscriptionRemoved` and `missed` notifications.</span></span>

## <a name="responding-to-subscriptionremoved-notifications"></a><span data-ttu-id="10df9-136">Responder a notificações subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="10df9-136">Responding to subscriptionRemoved notifications</span></span>

<span data-ttu-id="10df9-137">A notificação de `subscriptionRemoved` ciclo de vida informa que uma assinatura foi removida e deve ser recriada, se você quiser continuar a receber as notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="10df9-137">The `subscriptionRemoved` lifecycle notification informs you that a subscription has been removed and should be recreated, if you want to continue receiving change notifications.</span></span> 

<span data-ttu-id="10df9-138">Você pode criar uma assinatura de longa duração (três dias) e as notificações de alteração começarão a fluir para o **notificationUrl** .</span><span class="sxs-lookup"><span data-stu-id="10df9-138">You can create a long-lived subscription (3 days), and change notifications will start flowing to the **notificationUrl** .</span></span> <span data-ttu-id="10df9-139">No entanto, as condições de acesso aos dados de recursos podem mudar ao longo do tempo.</span><span class="sxs-lookup"><span data-stu-id="10df9-139">However, the conditions of access to the resource data might change over time.</span></span> <span data-ttu-id="10df9-140">Por exemplo, pode ocorrer um evento no serviço que exija que o aplicativo autentique novamente o usuário.</span><span class="sxs-lookup"><span data-stu-id="10df9-140">For example, an event in the service might occur that requires the app to re-authenticate the user.</span></span> <span data-ttu-id="10df9-141">Nesse caso, o fluxo é:</span><span class="sxs-lookup"><span data-stu-id="10df9-141">In such a case, the flow is as follows:</span></span>

1. <span data-ttu-id="10df9-142">O serviço detecta que uma assinatura precisa ser removida do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="10df9-142">The service detects that a subscription needs to be removed from Microsoft Graph.</span></span>
    
    <span data-ttu-id="10df9-143">Não há cadência definida para esses eventos.</span><span class="sxs-lookup"><span data-stu-id="10df9-143">There is no set cadence for these events.</span></span> <span data-ttu-id="10df9-144">Eles podem ocorrer com frequência para alguns recursos e quase nunca para outros.</span><span class="sxs-lookup"><span data-stu-id="10df9-144">They might occur frequently for some resources, and almost never for others.</span></span>

2. <span data-ttu-id="10df9-145">O Microsoft Graph envia uma notificação `subscriptionRemoved` de ciclo de vida para **lifecycleNotificationUrl** (se especificado).</span><span class="sxs-lookup"><span data-stu-id="10df9-145">Microsoft Graph sends a `subscriptionRemoved` lifecycle notification to the **lifecycleNotificationUrl** (if specified).</span></span>  

3. <span data-ttu-id="10df9-146">Você pode responder a essa notificação do ciclo de vida criando uma nova assinatura para o mesmo recurso.</span><span class="sxs-lookup"><span data-stu-id="10df9-146">You can respond to this lifecycle notification by creating a new subscription for the same resource.</span></span> <span data-ttu-id="10df9-147">Para fazer isso, é necessário apresentar um token de acesso válido; em alguns casos, isso significa que o aplicativo precisa reautenticar o usuário para obter um novo token de acesso válido.</span><span class="sxs-lookup"><span data-stu-id="10df9-147">To do this, you need to present a valid access token; in some cases this means the app needs to re-authenticate the user to obtain a new valid access token.</span></span>

4. <span data-ttu-id="10df9-148">Se você criar uma nova assinatura com êxito, as notificações de alteração de recurso começarão a fluir novamente.</span><span class="sxs-lookup"><span data-stu-id="10df9-148">If you successfully create a new subscription, change notifications will start flowing again.</span></span> <span data-ttu-id="10df9-149">No entanto, se houver falha (por exemplo, o aplicativo não pode obter um token de acesso válido), as notificações de alteração não serão enviadas.</span><span class="sxs-lookup"><span data-stu-id="10df9-149">However, if you fail (for example, the app can't obtain a valid access token), change notifications will not be sent.</span></span>

5. <span data-ttu-id="10df9-150">Depois de criar uma nova assinatura, você pode sincronizar os dados de recursos para identificar alterações ausentes.</span><span class="sxs-lookup"><span data-stu-id="10df9-150">After creating the new subscription, you can sync the resource data to identify any missing changes.</span></span>

### <a name="subscriptionremoved-notification-example"></a><span data-ttu-id="10df9-151">exemplo de notificação subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="10df9-151">subscriptionRemoved notification example</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2019-03-20T11:00:00.0000000Z",
      "tenantId": "<tenant_guid>",
      "clientState":"<secretClientState>",
      "lifecycleEvent": "subscriptionRemoved"
    }
  ]
}
```

<span data-ttu-id="10df9-152">Alguns aspectos a serem observados neste tipo de notificação:</span><span class="sxs-lookup"><span data-stu-id="10df9-152">A few things to note about this type of notification:</span></span>

- <span data-ttu-id="10df9-153">O `"lifecycleEvent": "subscriptionRemoved"` campo designa essa notificação como relacionada à remoção de assinatura.</span><span class="sxs-lookup"><span data-stu-id="10df9-153">The `"lifecycleEvent": "subscriptionRemoved"` field designates this notification as related to subscription removal.</span></span> <span data-ttu-id="10df9-154">Outros tipos de notificações de ciclo de vida também são possíveis, e novos serão disponibilizados no futuro.</span><span class="sxs-lookup"><span data-stu-id="10df9-154">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="10df9-155">A notificação de ciclo de vida não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.</span><span class="sxs-lookup"><span data-stu-id="10df9-155">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="10df9-156">Assim como notificações de alteração, notificações de ciclo de vida devem ser agrupadas (na matriz **valor** ), cada com uma possivelmente valores diferentes **lifecycleEvent** .</span><span class="sxs-lookup"><span data-stu-id="10df9-156">Similar to change notifications, lifecycle notifications can be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="10df9-157">Processe cada notificação de ciclo de vida no lote adequadamente.</span><span class="sxs-lookup"><span data-stu-id="10df9-157">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="10df9-158">**Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração forem entregues, confira [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="10df9-158">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="10df9-159">Ações a serem executadas</span><span class="sxs-lookup"><span data-stu-id="10df9-159">Actions to take</span></span>

1. <span data-ttu-id="10df9-160">[Confirme](webhooks.md#change-notifications) o recebimento da notificação do ciclo de vida respondendo à chamada do POST com `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="10df9-160">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="10df9-161">[Validar](webhooks.md#change-notifications) a autenticidade da notificação do ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="10df9-161">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="10df9-162">Certifique-se de que o aplicativo tenha um token de acesso válido para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="10df9-162">Ensure that the app has a valid access token to take the next step.</span></span> 
  > <span data-ttu-id="10df9-163">**Observação** : se você estiver usando uma das [bibliotecas de autenticação](/azure/active-directory/develop/reference-v2-libraries), elas farão isso para você ao reutilizar um token de cache válido ou obtendo um novo token, inclusive pedindo ao usuário para fazer logon novamente (com uma nova senha).</span><span class="sxs-lookup"><span data-stu-id="10df9-163">**Note:** If you're using one of the [authentication libraries](/azure/active-directory/develop/reference-v2-libraries), they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to sign in again (with a new password).</span></span> <span data-ttu-id="10df9-164">Observe que a obtenção de um novo token pode falhar, pois as condições de acesso podem ser alteradas e o chamador não poderá mais acessar os dados de recursos. </span><span class="sxs-lookup"><span data-stu-id="10df9-164">Note that obtaining a new token might fail, because the conditions of access might have changed, and the caller might no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="10df9-165">Criar uma nova assinatura usando o processo padrão descrito [aqui](webhooks.md#subscription-request-example).</span><span class="sxs-lookup"><span data-stu-id="10df9-165">Create a new subscription using the standard process described [here](webhooks.md#subscription-request-example).</span></span>

  > <span data-ttu-id="10df9-166">**Observação:** essa ação pode falhar, porque as verificações de autorização realizadas pelo sistema podem recusar o aplicativo ou o acesso do usuário ao recurso.</span><span class="sxs-lookup"><span data-stu-id="10df9-166">**Note:** This action might fail, because the authorization checks performed by the system might deny the app or the user access to the resource.</span></span> <span data-ttu-id="10df9-167">Pode ser necessário que o aplicativo obtenha um novo token de acesso do usuário para reautorizar uma assinatura com êxito.</span><span class="sxs-lookup"><span data-stu-id="10df9-167">It might be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> <span data-ttu-id="10df9-168">Você pode tentar essa ações mais tarde, a qualquer momento; por exemplo, quando as condições de acesso mudarem.</span><span class="sxs-lookup"><span data-stu-id="10df9-168">You can retry these actions later, at any time; for example, when the conditions of access have changed.</span></span> <span data-ttu-id="10df9-169">Quaisquer alterações de recursos no período de quando a notificação de ciclo de vida foi enviada até quando o aplicativo recriou a assinatura com êxito, serão perdidas.</span><span class="sxs-lookup"><span data-stu-id="10df9-169">Any resource changes in the time period from when the lifecycle notification was sent, to when the app recreates the subscription successfully, will be lost.</span></span> <span data-ttu-id="10df9-170">O aplicativo precisará buscar essas alterações sozinho.</span><span class="sxs-lookup"><span data-stu-id="10df9-170">The app will need to fetch those changes on its own.</span></span>

5. <span data-ttu-id="10df9-171">Depois de criar a nova assinatura, sincronizar todos os dados de recurso ausentes desde a última vez que você recebeu uma notificação para esse recurso, Por exemplo: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span><span class="sxs-lookup"><span data-stu-id="10df9-171">After creating the new subscription, sync any missing resource data from the last known time you received a change notification for this resource; for example: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span></span>

## <a name="responding-to-missed-notifications"></a><span data-ttu-id="10df9-172">Responder notificações perdidas</span><span class="sxs-lookup"><span data-stu-id="10df9-172">Responding to missed notifications</span></span>

<span data-ttu-id="10df9-173">Esses sinais informam que algumas notificações podem não ter sido entregues.</span><span class="sxs-lookup"><span data-stu-id="10df9-173">These signals inform you that some change notifications might not have been delivered.</span></span> <span data-ttu-id="10df9-174">Você deve ignorar ou lidar com esses sinais são.</span><span class="sxs-lookup"><span data-stu-id="10df9-174">You should decide if you ignore or handle these signals.</span></span>

### <a name="notification-example"></a><span data-ttu-id="10df9-175">Exemplo de notificação</span><span class="sxs-lookup"><span data-stu-id="10df9-175">Notification example</span></span>

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2019-03-20T11:00:00.0000000Z",
      "tenantId": "<tenant_guid>",
      "clientState":"<secretClientState>",
      "lifecycleEvent": "missed"
    }
  ]
}
```

<span data-ttu-id="10df9-176">Alguns aspectos a serem observados neste tipo de notificação:</span><span class="sxs-lookup"><span data-stu-id="10df9-176">A few things to note about this type of notification:</span></span>

- <span data-ttu-id="10df9-177">O `"lifecycleEvent": "missed"` campo designa isso como um sinal de notificações perdidas.</span><span class="sxs-lookup"><span data-stu-id="10df9-177">The `"lifecycleEvent": "missed"` field designates this as a signal about missed change notifications.</span></span> <span data-ttu-id="10df9-178">Outros tipos de notificações de ciclo de vida também são possíveis, e novos serão disponibilizados no futuro.</span><span class="sxs-lookup"><span data-stu-id="10df9-178">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="10df9-179">A notificação de ciclo de vida não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.</span><span class="sxs-lookup"><span data-stu-id="10df9-179">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="10df9-180">Assim como notificações de alteração, notificações de ciclo de vida podem ser agrupadas (na matriz **valor** ), cada com uma possivelmente valores diferentes **lifecycleEvent** .</span><span class="sxs-lookup"><span data-stu-id="10df9-180">Similar to change notifications, lifecycle notifications might be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="10df9-181">Processe cada notificação de ciclo de vida no lote adequadamente.</span><span class="sxs-lookup"><span data-stu-id="10df9-181">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="10df9-182">**Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração forem entregues, confira [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="10df9-182">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="10df9-183">Ações a serem executadas</span><span class="sxs-lookup"><span data-stu-id="10df9-183">Actions to take</span></span>

1. <span data-ttu-id="10df9-184">[Confirme](webhooks.md#change-notifications) o recebimento da notificação do ciclo de vida respondendo à chamada do POST com `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="10df9-184">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
    - <span data-ttu-id="10df9-185">Caso você ignore estes sinais, não faça nada.</span><span class="sxs-lookup"><span data-stu-id="10df9-185">If you ignore these signals, do nothing else.</span></span> <span data-ttu-id="10df9-186">Caso contrário:</span><span class="sxs-lookup"><span data-stu-id="10df9-186">Otherwise:</span></span>
2. <span data-ttu-id="10df9-187">[Validar](webhooks.md#change-notifications) a autenticidade da notificação do ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="10df9-187">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="10df9-188">Executaremos ressincronização de dados completa para identificar as alterações que não foram entregues como notificações.</span><span class="sxs-lookup"><span data-stu-id="10df9-188">Perform a full data resync of the resource to identify the changes that were not delivered as notifications.</span></span> 

## <a name="responding-to-reauthorizationrequired-notifications"></a><span data-ttu-id="10df9-189">Respondendo a notificações reauthorizationRequired</span><span class="sxs-lookup"><span data-stu-id="10df9-189">Responding to reauthorizationRequired notifications</span></span>

<span data-ttu-id="10df9-190">Quando receber uma notificação `reauthorizationRequired` de ciclo de vida, você deve reautorizar a inscrição para manter o fluxo de dados.</span><span class="sxs-lookup"><span data-stu-id="10df9-190">When you receive a `reauthorizationRequired` lifecycle notification, you must reauthorize the subscription to maintain the data flow.</span></span>

<span data-ttu-id="10df9-191">Você pode criar uma inscrição de longa duração (três dias) e as notificações de alteração começarão a fluir para o **notificationUrl** .</span><span class="sxs-lookup"><span data-stu-id="10df9-191">You can create a long-lived subscription (3 days), which enables change notifications to flow to the **notificationUrl** .</span></span> <span data-ttu-id="10df9-192">Caso as condições de acesso tenham sido alteradas desde a criação da assinatura, o Microsoft Graph pode exigir que você recrie a assinatura para provar que ainda tem acesso aos dados do recurso.</span><span class="sxs-lookup"><span data-stu-id="10df9-192">If the conditions of access have changed since the subscription was created, Microsoft Graph may require that you reauthorize the subscription to prove that you still have access to resource data.</span></span> <span data-ttu-id="10df9-193">A seguir estão exemplos de alterações que afetam o acesso aos dados:</span><span class="sxs-lookup"><span data-stu-id="10df9-193">The following are examples of changes that affect your access to data:</span></span>

- <span data-ttu-id="10df9-194">Um administrador de locatários pode revogar as permissões do seu aplicativo para ler um recurso.</span><span class="sxs-lookup"><span data-stu-id="10df9-194">A tenant administrator may revoke your app's permissions to read a resource.</span></span>
- <span data-ttu-id="10df9-195">Em um cenário interativo, o usuário que fornece o token de autenticação ao seu aplicativo pode estar sujeito a políticas dinâmicas com base em vários fatores, como o local, o estado do dispositivo ou a avaliação de risco.</span><span class="sxs-lookup"><span data-stu-id="10df9-195">In an interactive scenario, the user who provides the authentication token to your app may be subject to dynamic policies based on various factors, such as their location, device state, or risk assesment.</span></span> <span data-ttu-id="10df9-196">Por exemplo, se o usuário alterar o seu local físico, pode ser que ele não tenha mais permissão para acessar os dados e seu aplicativo não conseguirá autorizar novamente a assinatura.</span><span class="sxs-lookup"><span data-stu-id="10df9-196">For example, if the user changes their physical location, the user may no longer be allowed to access the data, and your app will not be able to reauthorize the subscription.</span></span> <span data-ttu-id="10df9-197">Para saber mais sobre políticas dinâmicas que controlam o acesso, confira [Políticas de acesso condicional do Azure AD](/azure/active-directory/conditional-access/overview).</span><span class="sxs-lookup"><span data-stu-id="10df9-197">For more information about dynamic policies that control access, see [Azure AD conditional access policies](/azure/active-directory/conditional-access/overview).</span></span> 

<span data-ttu-id="10df9-198">As etapas a seguir representam o fluxo de um desafio de autorização para uma assinatura ativa:</span><span class="sxs-lookup"><span data-stu-id="10df9-198">The following steps represent the flow of an authorization challenge for an active subscription:</span></span>

1. <span data-ttu-id="10df9-199">O Microsoft Graph exige que uma assinatura seja autorizada novamente.</span><span class="sxs-lookup"><span data-stu-id="10df9-199">Microsoft Graph requires a subscription to be reauthorized.</span></span>
    
    <span data-ttu-id="10df9-200">Os motivos para isso podem variar de recurso para recurso e podem mudar com o tempo.</span><span class="sxs-lookup"><span data-stu-id="10df9-200">The reasons for this may vary from resource to resource, and may change over time.</span></span> <span data-ttu-id="10df9-201">Você deve responder a um evento de nova autorização, não importa o que o causou.</span><span class="sxs-lookup"><span data-stu-id="10df9-201">You must respond to a reauthorization event no matter what caused it.</span></span>

2. <span data-ttu-id="10df9-202">O Microsoft Graph envia uma notificação de desafio de autorização para **lifecycleNotificationUrl** .</span><span class="sxs-lookup"><span data-stu-id="10df9-202">Microsoft Graph sends an authorization challenge notification to the **lifecycleNotificationUrl** .</span></span>

    <span data-ttu-id="10df9-203">Observe que o fluxo de notificações de alterações pode continuar por um tempo, dando a você tempo extra para responder.</span><span class="sxs-lookup"><span data-stu-id="10df9-203">Note that the flow of change notifications may continue for a while, giving you extra time to respond.</span></span> <span data-ttu-id="10df9-204">No entanto, eventualmente a alteração na entrega de notificação fará uma pausa até você executar a ação necessária.</span><span class="sxs-lookup"><span data-stu-id="10df9-204">However, eventually change notification delivery pauses, until you take the required action.</span></span>

3. <span data-ttu-id="10df9-205">Responda a esta notificação do ciclo de vida de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="10df9-205">Respond to this lifecycle notification in one of two ways:</span></span>
    - <span data-ttu-id="10df9-206">Autorizar a assinatura novamente.</span><span class="sxs-lookup"><span data-stu-id="10df9-206">Reauthorize the subscription.</span></span> <span data-ttu-id="10df9-207">Isso não estende a data de vencimento da assinatura.</span><span class="sxs-lookup"><span data-stu-id="10df9-207">This does not extend the expiry date of the subscription.</span></span>
    - <span data-ttu-id="10df9-208">Renove a assinatura.</span><span class="sxs-lookup"><span data-stu-id="10df9-208">Renew the subscription.</span></span> <span data-ttu-id="10df9-209">Isso autoriza novamente e estende a data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="10df9-209">This both reauthorizes and extends the expiry date.</span></span>

    <span data-ttu-id="10df9-210">Observação: as duas ações exigem a apresentação de um token de autenticação válido, semelhante a [criar uma nova assinatura](webhooks.md#creating-a-subscription) ou [renova uma assinatura antes da sua expiração](webhooks.md#renewing-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="10df9-210">Note: Both actions require you to present a valid authentication token, similar to [creating a new subscription](webhooks.md#creating-a-subscription) or [renewing a subscription before its expiry](webhooks.md#renewing-a-subscription).</span></span>

4. <span data-ttu-id="10df9-211">Se você autorizar novamente ou renovar com êxito a inscrição, as notificações de alteração continuarão.</span><span class="sxs-lookup"><span data-stu-id="10df9-211">If you successfully reauthorize or renew the subscription, change notifications continue.</span></span> <span data-ttu-id="10df9-212">Caso contrário, as notificações de alteração permanecerão pausadas.</span><span class="sxs-lookup"><span data-stu-id="10df9-212">Otherwise, change notifications remain paused.</span></span>

### <a name="reauthorizationrequired-notification-example"></a><span data-ttu-id="10df9-213">exemplo de notificação reauthorizationRequired</span><span class="sxs-lookup"><span data-stu-id="10df9-213">reauthorizationRequired notification example</span></span>

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

<span data-ttu-id="10df9-214">Alguns aspectos a serem observados neste tipo de notificação:</span><span class="sxs-lookup"><span data-stu-id="10df9-214">A few things to note about this type of notification:</span></span>

- <span data-ttu-id="10df9-215">O campo `"lifecycleEvent": "reauthorizationRequired"` identifica essa notificação como um desafio de autorização.</span><span class="sxs-lookup"><span data-stu-id="10df9-215">The `"lifecycleEvent": "reauthorizationRequired"` field designates this notification as an authorization challenge.</span></span> <span data-ttu-id="10df9-216">Outros tipos de notificações de ciclo de vida também são possíveis, e novos serão disponibilizados no futuro.</span><span class="sxs-lookup"><span data-stu-id="10df9-216">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="10df9-217">A notificação de ciclo de vida não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.</span><span class="sxs-lookup"><span data-stu-id="10df9-217">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="10df9-218">Semelhante às notificações de alteração, você pode agrupar as notificações do ciclo de vida em conjunto (na coleção de **valores** ), cada uma com um valor possivelmente diferente do **lifecycleEvent** .</span><span class="sxs-lookup"><span data-stu-id="10df9-218">Similar to change notifications, you can batch lifecycle notifications together (in the **value** collection), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="10df9-219">Processe cada notificação de ciclo de vida no lote adequadamente.</span><span class="sxs-lookup"><span data-stu-id="10df9-219">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="10df9-220">**Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração forem entregues, confira [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="10df9-220">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="10df9-221">Ações a serem executadas</span><span class="sxs-lookup"><span data-stu-id="10df9-221">Actions to take</span></span>

1. <span data-ttu-id="10df9-222">[Confirme](webhooks.md#change-notifications) o recebimento da notificação do ciclo de vida respondendo à chamada do POST com `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="10df9-222">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="10df9-223">[Validar](webhooks.md#change-notifications) a autenticidade da notificação do ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="10df9-223">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="10df9-224">Certifique-se de que o aplicativo tenha um token de acesso válido para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="10df9-224">Ensure that the app has a valid access token to take the next step.</span></span> 
  > <span data-ttu-id="10df9-225">**Observação** : se você estiver usando uma das [bibliotecas de autenticação](/azure/active-directory/develop/reference-v2-libraries), elas farão isso para você ao reutilizar um token de cache válido ou obtendo um novo token, inclusive pedindo ao usuário para fazer logon novamente (com uma nova senha).</span><span class="sxs-lookup"><span data-stu-id="10df9-225">**Note:** If you're using one of the [authentication libraries](/azure/active-directory/develop/reference-v2-libraries), they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to sign in again (with a new password).</span></span> <span data-ttu-id="10df9-226">Observe que a obtenção de um novo token pode falhar, pois as condições de acesso podem ser alteradas e o chamador não poderá mais acessar os dados de recursos. </span><span class="sxs-lookup"><span data-stu-id="10df9-226">Note that obtaining a new token might fail, because the conditions of access might have changed, and the caller might no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="10df9-227">Chamar uma das duas APIs a seguir.</span><span class="sxs-lookup"><span data-stu-id="10df9-227">Call either of the following two APIs.</span></span> <span data-ttu-id="10df9-228">Se a chamada da API for bem-sucedida, o fluxo de notificação de mudança será retomado.</span><span class="sxs-lookup"><span data-stu-id="10df9-228">If the API call succeeds, the change notification flow resumes.</span></span>

    - <span data-ttu-id="10df9-229">Chame a ação `/reauthorize` para autorizar novamente a assinatura sem estender a data de vencimento:</span><span class="sxs-lookup"><span data-stu-id="10df9-229">Call the `/reauthorize` action to reauthorize the subscription without extending its expiration date:</span></span>
        ```http
        POST  https://graph.microsoft.com/beta/subscriptions/{id}/reauthorize
        Content-type: application/json
        ```
    - <span data-ttu-id="10df9-230">Execute uma ação de renovação regular para autorizar novamente e renovar a assinatura ao mesmo tempo:</span><span class="sxs-lookup"><span data-stu-id="10df9-230">Perform a regular renew action to reauthorize and renew the subscription at the same time:</span></span>
        ```http
        PATCH https://graph.microsoft.com/beta/subscriptions/{id}
        Content-Type: application/json

        {
           "expirationDateTime": "2019-09-21T11:00:00.0000000Z"
        }
        ```

      <span data-ttu-id="10df9-231">A renovação pode falhar, porque as verificações de autorização realizadas pelo sistema podem recusar o aplicativo ou o acesso do usuário ao recurso.</span><span class="sxs-lookup"><span data-stu-id="10df9-231">Renewing may fail, because the authorization checks performed by the system may deny the app or the user access to the resource.</span></span> <span data-ttu-id="10df9-232">Pode ser necessário que o aplicativo obtenha um novo token de acesso do usuário para reautorizar com êxito uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="10df9-232">It may be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> 
      
      <span data-ttu-id="10df9-233">Você pode tentar essa ações mais tarde, a qualquer momento e obter êxito se as condições de acesso mudarem.</span><span class="sxs-lookup"><span data-stu-id="10df9-233">You may retry these actions later, at any time, and succeed if the conditions of access change.</span></span> <span data-ttu-id="10df9-234">As notificações sobre as alterações de recursos que acontecem entre o tempo de envio da notificação do ciclo de vida e o momento em que o aplicativo cria a assinatura novamente, seriam perdidas.</span><span class="sxs-lookup"><span data-stu-id="10df9-234">Any notifications about resource changes that happen between the time the lifecycle notification was sent and the time when the app successfully creates the subscription again, would be lost.</span></span> <span data-ttu-id="10df9-235">Nesses casos, o aplicativo deve buscar essas mudanças separadamente.</span><span class="sxs-lookup"><span data-stu-id="10df9-235">In such cases, the app should separately fetch those changes.</span></span>

### <a name="additional-information"></a><span data-ttu-id="10df9-236">Informações adicionais</span><span class="sxs-lookup"><span data-stu-id="10df9-236">Additional information</span></span>

<span data-ttu-id="10df9-237">As informações a seguir podem ajudá-lo a entender os desafios de autorização:</span><span class="sxs-lookup"><span data-stu-id="10df9-237">The following information can help you understand authorization challenges:</span></span>

- <span data-ttu-id="10df9-238">Os desafios de autorização não substituem a necessidade de renova uma assinatura de alteração de recursos antes de expirar.</span><span class="sxs-lookup"><span data-stu-id="10df9-238">Authorization challenges do not replace the need to renew a resource change subscription before it expires.</span></span> 

    <span data-ttu-id="10df9-239">Embora você possa optar por renovar uma assinatura quando recebe um desafio de autorização, o Microsoft Graph pode não desafiar todas as suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="10df9-239">While you can choose to renew a subscription when you receive an authorization challenge, Microsoft Graph may not challenge all of your subscriptions.</span></span> <span data-ttu-id="10df9-240">Por exemplo, uma assinatura que não possui nenhuma atividade e não possui notificações de alterações com entrega pendente pode não sinalizar nenhum desafio para uma nova autorização do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="10df9-240">For example, a subscription that does not have any activity and has no change notifications pending delivery may not signal any reauthorization challenges to your app.</span></span> <span data-ttu-id="10df9-241">Certifique-se de [renovar assinaturas](webhooks.md#renewing-a-subscription) antes de expirarem.</span><span class="sxs-lookup"><span data-stu-id="10df9-241">Make sure to [renew subscriptions](webhooks.md#renewing-a-subscription) before they expire.</span></span>

- <span data-ttu-id="10df9-242">A frequência dos desafios de autorização está sujeita a mudanças.</span><span class="sxs-lookup"><span data-stu-id="10df9-242">The frequency of authorization challenges is subject to change.</span></span>

    <span data-ttu-id="10df9-243">Não faça suposições sobre a frequência dos desafios de autorização.</span><span class="sxs-lookup"><span data-stu-id="10df9-243">Do not make assumptions about the frequency of authorization challenges.</span></span> <span data-ttu-id="10df9-244">Essas notificações do ciclo de vida informam quando você deve executar as ações, evitando que você precise rastrear quais assinaturas requerem uma nova autorização.</span><span class="sxs-lookup"><span data-stu-id="10df9-244">These lifecycle notifications tell you when to take actions, saving you from having to track which subscriptions require reauthorization.</span></span> <span data-ttu-id="10df9-245">Esteja pronto para lidar com os desafios de autorização de vez em quando, para todas as assinaturas até raramente para apenas algumas das suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="10df9-245">Be ready to handle authorization challenges from once every few minutes for every subscription to rarely for only some of your subscriptions.</span></span>

## <a name="future-proof-the-code-handling-lifecycle-notifications"></a><span data-ttu-id="10df9-246">À prova de futuro o código lidar com as notificações de ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="10df9-246">Future-proof the code handling lifecycle notifications</span></span>

<span data-ttu-id="10df9-247">No futuro, o Microsoft Graph adicionará mais tipos de notificações de ciclo de vida da assinatura.</span><span class="sxs-lookup"><span data-stu-id="10df9-247">In the future, Microsoft Graph will add more types of subscription lifecycle notifications.</span></span> <span data-ttu-id="10df9-248">Elas serão publicadas no mesmo ponto de extremidade: **lifecycleNotificationUrl** , mas terão um valor diferente sob **lifecycleEvent** e podem conter um esquema e propriedades ligeiramente diferentes, específicas para o cenário para o qual serão enviadas.</span><span class="sxs-lookup"><span data-stu-id="10df9-248">They will be posted to the same endpoint: **lifecycleNotificationUrl** , but they will have a different value under **lifecycleEvent** and might contain a slightly different schema and properties, specific to the scenario for which they will be issued.</span></span>

<span data-ttu-id="10df9-249">Você deve implementar o código á prova de futuro para que não pare quando o Microsoft Graph apresentar novos tipos de notificações de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="10df9-249">You should implement your code in a future-proof way so it does not break when Microsoft Graph introduces new types of lifecycle notifications.</span></span> <span data-ttu-id="10df9-250">Recomendamos as seguintes abordagens:</span><span class="sxs-lookup"><span data-stu-id="10df9-250">We recommend the following approach:</span></span>

1. <span data-ttu-id="10df9-251">Identifique explicitamente cada notificação do ciclo de vida como um evento que você oferece suporte, usando a propriedade **lifecycleEvent** .</span><span class="sxs-lookup"><span data-stu-id="10df9-251">Explicitly identify each lifecycle notification as an event that you support, using the **lifecycleEvent** property.</span></span> <span data-ttu-id="10df9-252">Por exemplo, procure a `"lifecycleEvent": "subscriptionRemoved"` propriedade para identificar um evento específico e tratá-lo.</span><span class="sxs-lookup"><span data-stu-id="10df9-252">For example, look for the `"lifecycleEvent": "subscriptionRemoved"` property to identify a specific event, and handle it.</span></span>

2. <span data-ttu-id="10df9-253">Assista aos comunicados de notificações do ciclo de vida para ver novos cenários.</span><span class="sxs-lookup"><span data-stu-id="10df9-253">Watch for announcements of lifecycle notifications for new scenarions.</span></span> <span data-ttu-id="10df9-254">Pode haver mais tipos de notificações de ciclo de vida no futuro.</span><span class="sxs-lookup"><span data-stu-id="10df9-254">There might be more types of lifecycle notifications in the future.</span></span>

3. <span data-ttu-id="10df9-255">Em seu aplicativo ignore todos os eventos de ciclo de vida que o aplicativo não reconhece e registre-os para obter conhecimento.</span><span class="sxs-lookup"><span data-stu-id="10df9-255">In your app, ignore any lifecycle notification that the app does not recognize, and log them to gain awareness.</span></span>

4. <span data-ttu-id="10df9-256">Se desejar, procure a documentação relacionada às novas notificações de ciclo de vida e implemente o suporte para elas conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="10df9-256">At your discretion, look up the related documentation for new lifecycle notifications and implement support for them as appropriate.</span></span>

## <a name="see-also"></a><span data-ttu-id="10df9-257">Confira também</span><span class="sxs-lookup"><span data-stu-id="10df9-257">See also</span></span>

- [<span data-ttu-id="10df9-258">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="10df9-258">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="10df9-259">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="10df9-259">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="10df9-260">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="10df9-260">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="10df9-261">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="10df9-261">Delete subscription</span></span>](/graph/api/subscription-delete?view=graph-rest-1.0)
- [<span data-ttu-id="10df9-262">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="10df9-262">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)


[contato]: /graph/api/resources/contact?view=graph-rest-1.0
[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
[chatMessage]: /graph/api/resources/chatmessage
