---
title: Reduzir assinaturas ausentes e notificações de recursos do Outlook (visualização)
description: O Outlook pode suspender a entrega de notificações de alteração devido a eventos de segurança como a redefinição de senha do usuário. Eventos com ciclo de vida especial – `subscriptionRemoved` e `missed` -precisam ser tratados para garantir a entrega contínua de notificações.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: ad690749db14bdb8994e1bfe85b0b312029657a2
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2020
ms.locfileid: "41651775"
---
# <a name="reduce-missing-subscriptions-and-notifications-for-outlook-resources-preview"></a><span data-ttu-id="7eae3-104">Reduzir assinaturas ausentes e notificações de recursos do Outlook (visualização)</span><span class="sxs-lookup"><span data-stu-id="7eae3-104">Reduce missing subscriptions and notifications for Outlook resources (preview)</span></span> 

<span data-ttu-id="7eae3-105">Assinatura de aplicativos para notificações de recursos do Outlook podem ter suas assinaturas removidas e perder algumas notificações.</span><span class="sxs-lookup"><span data-stu-id="7eae3-105">Apps subscribing to notifications for Outlook resources might get their subscriptions removed and miss some notifications.</span></span> <span data-ttu-id="7eae3-106">Os aplicativos devem implementar a lógica para detectar e se recuperar da perda e retomar um fluxo de notificação contínuo.</span><span class="sxs-lookup"><span data-stu-id="7eae3-106">Apps should implement logic to detect and recover from the loss, and resume a continuous notification flow.</span></span>

<span data-ttu-id="7eae3-107">Determinados eventos no Outlook podem fazer que a assinatura seja removida.</span><span class="sxs-lookup"><span data-stu-id="7eae3-107">Certain events in Outlook can cause a subscription to be removed.</span></span> <span data-ttu-id="7eae3-108">Esses eventos incluem:</span><span class="sxs-lookup"><span data-stu-id="7eae3-108">These events include:</span></span>

- <span data-ttu-id="7eae3-109">A senha do usuário foi redefinida</span><span class="sxs-lookup"><span data-stu-id="7eae3-109">User's password has been reset</span></span>
- <span data-ttu-id="7eae3-110">Dispositivo do usuário está fora de conformidade</span><span class="sxs-lookup"><span data-stu-id="7eae3-110">User's device is out of compliance</span></span>
-   <span data-ttu-id="7eae3-111">Conta do usuário foi revogada</span><span class="sxs-lookup"><span data-stu-id="7eae3-111">User's account has been revoked</span></span>

<span data-ttu-id="7eae3-112">Quando ocorre um evento, o Outlook envia uma notificação especial de ciclo de vida, `subscriptionRemoved`.</span><span class="sxs-lookup"><span data-stu-id="7eae3-112">When such an event happens, Outlook sends a special life cycle notification, `subscriptionRemoved`.</span></span>

<span data-ttu-id="7eae3-113">O Outlook também envia outra notificação de ciclo de vida, `missed`, se não for possível entregar uma notificação em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7eae3-113">Outlook also sends another life cycle notification, `missed`, if a notification cannot be delivered to an app.</span></span>

<span data-ttu-id="7eae3-114">Uma assinatura de um aplicativo para notificações de recursos do Outlook, como **mensagem** e **evento**, deve ouvir os sinais `subscriptionRemoved` e `missed` e fazer o seguinte:</span><span class="sxs-lookup"><span data-stu-id="7eae3-114">An app subscribing to notifications for Outlook resources, such as **message** and **event**, should listen to the `subscriptionRemoved` and `missed` signals and do the following:</span></span>

- <span data-ttu-id="7eae3-115">Após receber uma `subscriptionRemoved` notificação, o aplicativo deve recriar a assinatura para manter um fluxo contínuo.</span><span class="sxs-lookup"><span data-stu-id="7eae3-115">Upon receiving a `subscriptionRemoved` notification, the app should recreate the subscription in order to maintain a continuous flow.</span></span>
- <span data-ttu-id="7eae3-116">Ao receber uma `missed` notificação, o aplicativo deve ressincronizar os dados de recursos usando o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7eae3-116">On receiving a `missed` notification, the app should resynchronize resource data using Microsoft Graph.</span></span>

<span data-ttu-id="7eae3-117">Para receber notificações de ciclo de vida, você pode usar o ponto de extremidade **notificationUrl** existente que já recebe notificações de recurso, ou registrar um **lifecycleNotificationUrl** separado para receber notificações `subscriptionRemoved` e `missed` em um ponto de extremidade separado.</span><span class="sxs-lookup"><span data-stu-id="7eae3-117">To receive life cycle notifications, you can use the existing **notificationUrl** endpoint that already receives resource notifications, or you can register a separate **lifecycleNotificationUrl** to receive `subscriptionRemoved` and `missed` notifications in a separate endpoint.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="7eae3-118">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="7eae3-118">Creating a subscription</span></span>

<span data-ttu-id="7eae3-119">Ao criar uma assinatura, você pode especificar um ponto de extremidade de notificação separado usando a propriedade**lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7eae3-119">When creating a subscription, you can specify a separate notification endpoint using the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="7eae3-120">Se você especificar o ponto de extremidade, todos os tipos de notificações de ciclo de vida atuais e futuros serão entregues lá.</span><span class="sxs-lookup"><span data-stu-id="7eae3-120">If you specify the endpoint, all current and future types of life cycle notifications will be delivered there.</span></span> <span data-ttu-id="7eae3-121">Caso contrário, as notificações `subscriptionRemoved` e `missed` serão entregues nas **notificationUrl** existentes para todas as assinaturas existentes.</span><span class="sxs-lookup"><span data-stu-id="7eae3-121">Otherwise, `subscriptionRemoved` and `missed` notifications will be delivered to the existing **notificationUrl** for all existing subscriptions.</span></span>

> <span data-ttu-id="7eae3-122">**Observação:** a propriedade **lifecycleNotificationUrl** só pode ser definida ou lida usando as APIs beta do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7eae3-122">**Note:** The **lifecycleNotificationUrl** property can only be set or read using Microsoft Graph beta APIs.</span></span> <span data-ttu-id="7eae3-123">No entanto, as assinaturas criadas usando as APIs beta são armazenadas no mesmo ambiente de produção que as assinaturas criadas usando v1.0, para que você possa implementar o novo fluxo do Outlook, além de suas assinaturas, usando APIs v1.0.</span><span class="sxs-lookup"><span data-stu-id="7eae3-123">However, subscriptions created using beta APIs are stored in the same production environment as those created using v1.0, so you can implement the new Outlook flow in addition to your subscriptions creating using v1.0 APIs.</span></span>

> <span data-ttu-id="7eae3-124">As assinaturas criadas por meio das APIs do v 1.0 receberão notificações do ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="7eae3-124">Subscriptions created via the v1.0 APIs will receive lifecycle notifications.</span></span> 

### <a name="subscription-request-example"></a><span data-ttu-id="7eae3-125">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="7eae3-125">Subscription request example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/users/{id}/messages",
  "expirationDateTime": "2019-03-20T11:00:00.0000000Z",
  "clientState": "<secretClientState>"
}
```
 
> <span data-ttu-id="7eae3-126">**Importante:** Use o mesmo nome de host para ambas as notificações URLs.</span><span class="sxs-lookup"><span data-stu-id="7eae3-126">**Important:** Use the same hostname for both notifications URLs.</span></span> 

> <span data-ttu-id="7eae3-127">**Observação:** é preciso validar os dois pontos de extremidade da notificação, conforme descrito em [Gerenciar assinaturas](webhooks.md#managing-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="7eae3-127">**Note:** You need to validate both notification endpoints as described in [Managing subscriptions](webhooks.md#managing-subscriptions).</span></span>
<span data-ttu-id="7eae3-128">Se você quiser usar a mesma URL para os dois pontos de extremidade você receberá e responderá a duas solicitações de validação.</span><span class="sxs-lookup"><span data-stu-id="7eae3-128">If you choose to use the same URL for both endpoints you will receive and respond to two validation requests.</span></span>

> <span data-ttu-id="7eae3-129">**Observação:** Não é possível atualizar (`PATCH`) as assinaturas existentes para adicionar a propriedade **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7eae3-129">**Note:** You cannot update (`PATCH`) the existing subscriptions to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="7eae3-130">Você deve remover essas assinaturas existentes, criar novas assinaturas e especificar a propriedade **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7eae3-130">You should remove such existing subscriptions, and create new subscriptions and specify the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="7eae3-131">Assinaturas existentes, sem a propriedade **lifecycleNotificationUrl** receberão a `subscriptionRemoved` e `missed` notificações pelas **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7eae3-131">Existing subscriptions without **lifecycleNotificationUrl** property will receive the `subscriptionRemoved` and `missed` notifications via the **notificationUrl**.</span></span> 

## <a name="responding-to-subscriptionremoved-notifications"></a><span data-ttu-id="7eae3-132">Responder a notificações subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="7eae3-132">Responding to subscriptionRemoved notifications</span></span>

<span data-ttu-id="7eae3-133">A `subscriptionRemoved` notificação informa que uma assinatura foi removida e deve ser recriada, se você quiser continuar a receber notificações.</span><span class="sxs-lookup"><span data-stu-id="7eae3-133">The `subscriptionRemoved` notification informs you that a subscription has been removed and should be recreated, if you want to continue receiving notifications.</span></span> 

<span data-ttu-id="7eae3-134">Você pode criar uma assinatura de longa duração (3 dias) e notificações de dados do recurso começarão a fluir para a **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7eae3-134">You can create a long-lived subscription (3 days), and resource data notifications will start flowing to the **notificationUrl**.</span></span> <span data-ttu-id="7eae3-135">No entanto, as condições de acesso aos dados de recursos podem mudar ao longo do tempo.</span><span class="sxs-lookup"><span data-stu-id="7eae3-135">However, the conditions of access to the resource data might change over time.</span></span> <span data-ttu-id="7eae3-136">Por exemplo, pode ocorrer um evento no serviço do Outlook que requeira que o aplicativo para que o usuário seja autenticado novamente.</span><span class="sxs-lookup"><span data-stu-id="7eae3-136">For example, an event in the Outlook service might occur that requires the app to re-authenticate the user.</span></span> <span data-ttu-id="7eae3-137">Nesse caso, o fluxo é:</span><span class="sxs-lookup"><span data-stu-id="7eae3-137">In such a case, the flow is as follows:</span></span>

1. <span data-ttu-id="7eae3-138">Outlook detecta que uma assinatura precisa ser removido do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7eae3-138">Outlook detects that a subscription needs to be removed from Microsoft Graph.</span></span>
    
    <span data-ttu-id="7eae3-139">Não há cadência definida para esses eventos.</span><span class="sxs-lookup"><span data-stu-id="7eae3-139">There is no set cadence for these events.</span></span> <span data-ttu-id="7eae3-140">Eles podem ocorrer com frequência para alguns recursos e quase nunca para outros.</span><span class="sxs-lookup"><span data-stu-id="7eae3-140">They might occur frequently for some resources, and almost never for others.</span></span>

2. <span data-ttu-id="7eae3-141">O Microsoft Graph envia uma `subscriptionRemoved` notificação para a **lifecycleNotificationUrl** (se especificado), ou uma **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="7eae3-141">Microsoft Graph sends a `subscriptionRemoved` notification to the **lifecycleNotificationUrl** (if specified), or the **notificationUrl**.</span></span>  

3. <span data-ttu-id="7eae3-142">Você pode responder a essa notificação criando uma nova assinatura para o mesmo recurso.</span><span class="sxs-lookup"><span data-stu-id="7eae3-142">You can respond to this notification by creating a new subscription for the same resource.</span></span> <span data-ttu-id="7eae3-143">Para fazer isso, é necessário apresentar um token de acesso válido; em alguns casos, isso significa que o aplicativo precisa reautenticar o usuário para obter um novo token de acesso válido.</span><span class="sxs-lookup"><span data-stu-id="7eae3-143">To do this, you need to present a valid access token; in some cases this means the app needs to re-authenticate the user to obtain a new valid access token.</span></span>

4. <span data-ttu-id="7eae3-144">Se você criar uma nova assinatura com êxito, as notificações de recurso começarão a fluir novamente.</span><span class="sxs-lookup"><span data-stu-id="7eae3-144">If you successfully create a new subscription, resource notifications will start flowing again.</span></span> <span data-ttu-id="7eae3-145">No entanto, se você falhar (por exemplo, o aplicativo não pode obter um token de acesso válido), as notificações do recurso não serão enviadas.</span><span class="sxs-lookup"><span data-stu-id="7eae3-145">However, if you fail (for example, the app can't obtain a valid access token), resource notifications will not be sent.</span></span>

5. <span data-ttu-id="7eae3-146">Depois de criar uma nova assinatura, você pode sincronizar os dados de recursos para identificar alterações ausentes.</span><span class="sxs-lookup"><span data-stu-id="7eae3-146">After creating the new subscription, you can sync the resource data to identify any missing changes.</span></span>

### <a name="subscriptionremoved-notification-example"></a><span data-ttu-id="7eae3-147">exemplo de notificação subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="7eae3-147">subscriptionRemoved notification example</span></span>

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

<span data-ttu-id="7eae3-148">Alguns aspectos a serem observados neste tipo de notificação:</span><span class="sxs-lookup"><span data-stu-id="7eae3-148">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="7eae3-149">O `"lifecycleEvent": "subscriptionRemoved"` campo designa essa notificação como relacionada à remoção de assinatura.</span><span class="sxs-lookup"><span data-stu-id="7eae3-149">The `"lifecycleEvent": "subscriptionRemoved"` field designates this notification as related to subscription removal.</span></span> <span data-ttu-id="7eae3-150">Outros tipos de notificações de ciclo de vida também são possíveis, e novos serão disponibilizados no futuro.</span><span class="sxs-lookup"><span data-stu-id="7eae3-150">Other types of life cycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="7eae3-151">A notificação não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.</span><span class="sxs-lookup"><span data-stu-id="7eae3-151">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="7eae3-152">Assim como as notificações de recursos, as notificações de ciclo de vida podem estar em lote juntas (na matriz **valor**), cada uma com valores **lifecycleEvent** possivelmente diferentes.</span><span class="sxs-lookup"><span data-stu-id="7eae3-152">Similar to resource notifications, life cycle notifications can be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="7eae3-153">Processe cada notificação no lote de acordo.</span><span class="sxs-lookup"><span data-stu-id="7eae3-153">Process each notification in the batch accordingly.</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="7eae3-154">Ações a serem executadas</span><span class="sxs-lookup"><span data-stu-id="7eae3-154">Actions to take</span></span>

1. <span data-ttu-id="7eae3-155">[Aceite](webhooks.md#notifications) o recebimento da notificação respondendo a chamada POSTAGEM com `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="7eae3-155">[Acknowledge](webhooks.md#notifications) the receipt of the notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="7eae3-156">[Validar](webhooks.md#notifications) a autenticidade da notificação.</span><span class="sxs-lookup"><span data-stu-id="7eae3-156">[Validate](webhooks.md#notifications) the authenticity of the notification.</span></span>
3. <span data-ttu-id="7eae3-157">Certifique-se de que o aplicativo tenha um token de acesso válido para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="7eae3-157">Ensure that the app has a valid access token to take the next step.</span></span> 
  > <span data-ttu-id="7eae3-158">**Observação**: se você estiver usando uma das [bibliotecas de autenticação](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), elas farão isso para você ao reutilizar um token de cache válido ou obtendo um novo token, inclusive pedindo ao usuário para fazer logon novamente (com uma nova senha).</span><span class="sxs-lookup"><span data-stu-id="7eae3-158">**Note:** If you're using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to sign in again (with a new password).</span></span> <span data-ttu-id="7eae3-159">Observe que a obtenção de um novo token pode falhar, pois as condições de acesso podem ser alteradas e o chamador não poderá mais acessar os dados de recursos. </span><span class="sxs-lookup"><span data-stu-id="7eae3-159">Note that obtaining a new token might fail, because the conditions of access might have changed, and the caller might no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="7eae3-160">Criar uma nova assinatura usando o processo padrão descrito [aqui](webhooks.md#subscription-request-example).</span><span class="sxs-lookup"><span data-stu-id="7eae3-160">Create a new subscription using the standard process described [here](webhooks.md#subscription-request-example).</span></span>

  > <span data-ttu-id="7eae3-161">**Observação:** essa ação pode falhar, porque as verificações de autorização realizadas pelo sistema podem recusar o aplicativo ou o acesso do usuário ao recurso.</span><span class="sxs-lookup"><span data-stu-id="7eae3-161">**Note:** This action might fail, because the authorization checks performed by the system might deny the app or the user access to the resource.</span></span> <span data-ttu-id="7eae3-162">Pode ser necessário que o aplicativo obtenha um novo token de acesso do usuário para reautorizar uma assinatura com êxito.</span><span class="sxs-lookup"><span data-stu-id="7eae3-162">It might be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> <span data-ttu-id="7eae3-163">Você pode tentar essa ações mais tarde, a qualquer momento; por exemplo, quando as condições de acesso mudarem.</span><span class="sxs-lookup"><span data-stu-id="7eae3-163">You can retry these actions later, at any time; for example, when the conditions of access have changed.</span></span> <span data-ttu-id="7eae3-164">Quaisquer alterações de recursos no período de tempo quando a notificação de ciclo de vida foi enviada até quando o aplicativo recriou a assinatura com êxito, serão perdidas.</span><span class="sxs-lookup"><span data-stu-id="7eae3-164">Any resource changes in the time period from when the life cycle notification was sent, to when the app recreates the subscription successfully, will be lost.</span></span> <span data-ttu-id="7eae3-165">O aplicativo precisará buscar essas alterações sozinho.</span><span class="sxs-lookup"><span data-stu-id="7eae3-165">The app will need to fetch those changes on its own.</span></span>

5. <span data-ttu-id="7eae3-166">Depois de criar a nova assinatura, sincronizar todos os dados de recurso ausentes desde a última hora conhecida que você recebeu uma notificação para esse recurso, Por exemplo: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span><span class="sxs-lookup"><span data-stu-id="7eae3-166">After creating the new subscription, sync any missing resource data from the last known time you received a notification for this resource; for example: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span></span>

## <a name="responding-to-missed-notifications"></a><span data-ttu-id="7eae3-167">Responder notificações perdidas</span><span class="sxs-lookup"><span data-stu-id="7eae3-167">Responding to missed notifications</span></span>

<span data-ttu-id="7eae3-168">Esses sinais informam que algumas notificações podem não ter sido entregues.</span><span class="sxs-lookup"><span data-stu-id="7eae3-168">These signals inform you that some notifications might not have been delivered.</span></span> <span data-ttu-id="7eae3-169">Você deve ignorar ou lidar com esses sinais são.</span><span class="sxs-lookup"><span data-stu-id="7eae3-169">You should decide if you ignore or handle these signals.</span></span>

### <a name="notification-example"></a><span data-ttu-id="7eae3-170">Exemplo de notificação</span><span class="sxs-lookup"><span data-stu-id="7eae3-170">Notification example</span></span>

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

<span data-ttu-id="7eae3-171">Alguns aspectos a serem observados neste tipo de notificação:</span><span class="sxs-lookup"><span data-stu-id="7eae3-171">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="7eae3-172">O `"lifecycleEvent": "missed"` campo designa isso como um sinal de notificações perdidas.</span><span class="sxs-lookup"><span data-stu-id="7eae3-172">The `"lifecycleEvent": "missed"` field designates this as a signal about missed notifications.</span></span> <span data-ttu-id="7eae3-173">Outros tipos de notificações de ciclo de vida também são possíveis, e novos serão disponibilizados no futuro.</span><span class="sxs-lookup"><span data-stu-id="7eae3-173">Other types of life cycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="7eae3-174">A notificação não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.</span><span class="sxs-lookup"><span data-stu-id="7eae3-174">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="7eae3-175">Semelhante às notificações de recursos, as notificações de ciclo de vida podem estar em lote juntas (na matriz **valor**), cada uma com valores **lifecycleEvent** possivelmente diferentes.</span><span class="sxs-lookup"><span data-stu-id="7eae3-175">Similar to resource notifications, life cycle notifications might be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="7eae3-176">Processe cada notificação no lote de acordo.</span><span class="sxs-lookup"><span data-stu-id="7eae3-176">Process each notification in the batch accordingly.</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="7eae3-177">Ações a serem executadas</span><span class="sxs-lookup"><span data-stu-id="7eae3-177">Actions to take</span></span>

1. <span data-ttu-id="7eae3-178">[Aceite](webhooks.md#notifications) o recebimento da notificação respondendo a chamada POSTAGEM com `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="7eae3-178">[Acknowledge](webhooks.md#notifications) the receipt of the notification, by responding to the POST call with `202 - Accepted`.</span></span>
    - <span data-ttu-id="7eae3-179">Caso você ignore estes sinais, não faça nada.</span><span class="sxs-lookup"><span data-stu-id="7eae3-179">If you ignore these signals, do nothing else.</span></span> <span data-ttu-id="7eae3-180">Caso contrário:</span><span class="sxs-lookup"><span data-stu-id="7eae3-180">Otherwise:</span></span>
2. <span data-ttu-id="7eae3-181">[Validar](webhooks.md#notifications) a autenticidade da notificação.</span><span class="sxs-lookup"><span data-stu-id="7eae3-181">[Validate](webhooks.md#notifications) the authenticity of the notification.</span></span>
3. <span data-ttu-id="7eae3-182">Executaremos ressincronização de dados completa para identificar as alterações que não foram entregues como notificações.</span><span class="sxs-lookup"><span data-stu-id="7eae3-182">Perform a full data resync of the resource to identify the changes that were not delivered as notifications.</span></span> 


## <a name="future-proof-the-code-handling-life-cycle-notifications"></a><span data-ttu-id="7eae3-183">Proteja a longo prazo o tratamento de código das notificações do ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="7eae3-183">Future-proof the code handling life cycle notifications</span></span>

<span data-ttu-id="7eae3-184">No futuro, o Microsoft Graph adicionará mais tipos de notificações de ciclo de vida da assinatura.</span><span class="sxs-lookup"><span data-stu-id="7eae3-184">In the future, Microsoft Graph will add more types of subscription life cycle notifications.</span></span> <span data-ttu-id="7eae3-185">Elas serão publicadas no mesmo ponto de extremidade: **lifecycleNotificationUrl**, mas terão um valor diferente sob **lifecycleEvent** e podem conter um esquema e propriedades ligeiramente diferentes, específicas para o cenário para o qual serão enviadas.</span><span class="sxs-lookup"><span data-stu-id="7eae3-185">They will be posted to the same endpoint: **lifecycleNotificationUrl**, but they will have a different value under **lifecycleEvent** and might contain a slightly different schema and properties, specific to the scenario for which they will be issued.</span></span>

<span data-ttu-id="7eae3-186">Você deve fortalecer seu código para que não pare quando o Microsoft Graph apresentar novos tipos de notificações de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="7eae3-186">You should implement your code in a future-proof way so it does not break when Microsoft Graph introduces new types of life cycle notifications.</span></span> <span data-ttu-id="7eae3-187">Recomendamos as seguintes abordagens:</span><span class="sxs-lookup"><span data-stu-id="7eae3-187">We recommend the following approach:</span></span>

1. <span data-ttu-id="7eae3-188">Identificar explicitamente cada notificação como um evento suportado, usando a propriedade **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="7eae3-188">Explicitly identify each notification as an event that you support, using the **lifecycleEvent** property.</span></span> <span data-ttu-id="7eae3-189">Por exemplo, procure a `"lifecycleEvent": "subscriptionRemoved"` propriedade para identificar um evento específico e tratá-lo.</span><span class="sxs-lookup"><span data-stu-id="7eae3-189">For example, look for the `"lifecycleEvent": "subscriptionRemoved"` property to identify a specific event, and handle it.</span></span>

2. <span data-ttu-id="7eae3-190">Assista aos comunicados de notificações para ver novos cenários.</span><span class="sxs-lookup"><span data-stu-id="7eae3-190">Watch for announcements of notifications for new scenarions.</span></span> <span data-ttu-id="7eae3-191">Pode haver mais tipos de notificações de ciclo de vida no futuro.</span><span class="sxs-lookup"><span data-stu-id="7eae3-191">There might be more types of life cycle notifications in the future.</span></span>

3. <span data-ttu-id="7eae3-192">Em seu aplicativo, ignore todos os eventos de ciclo de vida que o aplicativo não reconhece e acesse-os para obter conhecimento.</span><span class="sxs-lookup"><span data-stu-id="7eae3-192">In your app, ignore any life cycle events that the app does not recognize, and log them to gain awareness.</span></span>

4. <span data-ttu-id="7eae3-193">Se desejar, procure a documentação relacionada às novas notificações de ciclo de vida e implemente o suporte para elas conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="7eae3-193">At your discretion, look up the related documentation for new life cycle notifications and implement support for them as appropriate.</span></span>

## <a name="see-also"></a><span data-ttu-id="7eae3-194">Confira também</span><span class="sxs-lookup"><span data-stu-id="7eae3-194">See also</span></span>

- [<span data-ttu-id="7eae3-195">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="7eae3-195">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="7eae3-196">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="7eae3-196">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="7eae3-197">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="7eae3-197">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="7eae3-198">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="7eae3-198">Delete subscription</span></span>](/graph/api/subscription-delete?view=graph-rest-1.0)
- [<span data-ttu-id="7eae3-199">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="7eae3-199">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
