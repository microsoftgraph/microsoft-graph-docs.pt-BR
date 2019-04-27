---
title: Reduzir assinaturas ausentes e notificações de recursos do Outlook (visualização)
description: Outlook pode suspender a entrega ou alterar notificações de devido a eventos de segurança como a redefinição de senha do usuário. Eventos com ciclo de vida especial – `subscriptionRemoved` e `missed` -precisam ser tratados para garantir a entrega contínua de notificações.
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 1c430743f860536ef20fa2ad9974e580c78a6f0d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32683973"
---
# <a name="reduce-missing-subscriptions-and-notifications-for-outlook-resources-preview"></a><span data-ttu-id="d5865-104">Reduzir assinaturas ausentes e notificações de recursos do Outlook (visualização)</span><span class="sxs-lookup"><span data-stu-id="d5865-104">Reduce missing subscriptions and notifications for Outlook resources (preview)</span></span> 

<span data-ttu-id="d5865-105">Assinatura de Aplicativos para notificações de recursos do Outlook podem ter suas assinaturas removidas e perder algumas notificações.</span><span class="sxs-lookup"><span data-stu-id="d5865-105">Apps subscribing to notifications for Outlook resources may get their subscriptions removed and miss some notifications.</span></span> <span data-ttu-id="d5865-106">Os aplicativos devem implementar a lógica para detectar e se recuperar da perda e retomar um fluxo de notificação contínuo.</span><span class="sxs-lookup"><span data-stu-id="d5865-106">Apps should implement logic to detect and recover from the loss, and resume a continuous notification flow.</span></span>

<span data-ttu-id="d5865-107">Determinados eventos no Outlook podem fazer que a assinatura seja removida.</span><span class="sxs-lookup"><span data-stu-id="d5865-107">Certain events in Outlook can cause a subscription to be removed.</span></span> <span data-ttu-id="d5865-108">Esses eventos incluem:</span><span class="sxs-lookup"><span data-stu-id="d5865-108">These events include the following:</span></span>

- <span data-ttu-id="d5865-109">A senha do usuário foi redefinida</span><span class="sxs-lookup"><span data-stu-id="d5865-109">User's password has been reset</span></span>
- <span data-ttu-id="d5865-110">Dispositivo do usuário está fora de conformidade</span><span class="sxs-lookup"><span data-stu-id="d5865-110">User's device is out of compliance</span></span>
-   <span data-ttu-id="d5865-111">Conta do usuário foi revogada</span><span class="sxs-lookup"><span data-stu-id="d5865-111">User's account has been revoked</span></span>

<span data-ttu-id="d5865-112">Quando ocorre um evento, o Outlook envia uma notificação de ciclo de vida especial `subscriptionRemoved`.</span><span class="sxs-lookup"><span data-stu-id="d5865-112">When such an event happens, Outlook sends a special lifecycle notification, `subscriptionRemoved`.</span></span>

<span data-ttu-id="d5865-113">O Outlook também envia outra notificação de ciclo de vida `missed`, se não for possível entregar uma notificação em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d5865-113">Outlook also sends another lifecycle notification, `missed`, if a notification cannot be delivered to an app.</span></span>

<span data-ttu-id="d5865-114">Uma assinatura de um aplicativo para notificações de recursos do Outlook, como **mensagem** e **evento**, deve ouvir as `subscriptionRemoved` e `missed` sinais:</span><span class="sxs-lookup"><span data-stu-id="d5865-114">An app subscribing to notifications for Outlook resources, such as **message** and **event**, should listen to the `subscriptionRemoved` and `missed` signals:</span></span>

- <span data-ttu-id="d5865-115">Após receber uma `subscriptionRemoved` notificação, o aplicativo deve recriar a assinatura para manter um fluxo contínuo.</span><span class="sxs-lookup"><span data-stu-id="d5865-115">Upon receiving a `subscriptionRemoved` notification, the app should recreate the subscription in order to maintain a continuous flow.</span></span>
- <span data-ttu-id="d5865-116">Ao receber uma `missed` notificação, o aplicativo deve ressincronizar os dados de recursos usando o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d5865-116">On receiving a `missed` notification, the app should resynchronize resource data using Microsoft Graph.</span></span>

<span data-ttu-id="d5865-117">Para receber notificações de ciclo de vida, você pode usar o ponto de extremidade **notificationUrl** existentes que já recebe notificações do recurso, ou registrar um **lifecycleNotificationUrl** separado para receber `subscriptionRemoved` e `missed` notificações em um ponto de extremidade separado.</span><span class="sxs-lookup"><span data-stu-id="d5865-117">To receive lifecycle notifications, you can use the existing **notificationUrl** endpoint that already receives resource notifications, or you can register a separate **lifecycleNotificationUrl** to receive `subscriptionRemoved` and `missed` notifications in a separate endpoint.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="d5865-118">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="d5865-118">Creating a subscription</span></span>

<span data-ttu-id="d5865-119">Ao criar uma assinatura, você pode especificar um ponto de extremidade de notificação separado usando a propriedade**lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="d5865-119">When creating a subscription, you can specify a separate notification endpoint using the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="d5865-120">Se você especificar o ponto de extremidade, todos os tipos de atuais e futuros de notificações de ciclo de vida serão entregues lá.</span><span class="sxs-lookup"><span data-stu-id="d5865-120">If you specify the endpoint, all current and future types of lifecycle notifications will be delivered there.</span></span> <span data-ttu-id="d5865-121">Caso contrário, as notificações `subscriptionRemoved` e `missed` serão entregues nas **notificationUrl** existentes para todas as assinaturas existentes.</span><span class="sxs-lookup"><span data-stu-id="d5865-121">Otherwise, `subscriptionRemoved` and `missed` notifications will be delivered to the existing **notificationUrl** for all existing subscriptions.</span></span>

> <span data-ttu-id="d5865-122">**Observação:** No momento, a propriedade **lifecycleNotificationUrl** só pode ser definida ou lida usando a `beta` versão das APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d5865-122">**Note:** At the moment, the **lifecycleNotificationUrl** property can only be set or read using the `beta` version of Microsoft Graph APIs.</span></span> <span data-ttu-id="d5865-123">No entanto, assinaturas criado usando `beta` são armazenadas no ambiente de produção como `v1.0` para que você possa implementar o novo fluxo do Outlook descrito aqui, além de seu uso comum `v1.0` com outras assinaturas.</span><span class="sxs-lookup"><span data-stu-id="d5865-123">However, subscriptions created using `beta` are stored in the same production environment as `v1.0` so you can implement the new Outlook flow described here in addition to your regular usage of `v1.0` with other subscriptions.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="d5865-124">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="d5865-124">Subscription request example</span></span>

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
 
> <span data-ttu-id="d5865-125">**Importante:** Use o mesmo nome de host para ambas as notificações URLs.</span><span class="sxs-lookup"><span data-stu-id="d5865-125">**Important:** Use the same hostname for both notifications URLs.</span></span> 

> <span data-ttu-id="d5865-126">**Observação:** É preciso validar os dois pontos de extremidade da notificação, conforme descrito no [artigo notificação genérica](webhooks.md#managing-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="d5865-126">**Note:** You need to validate both notification endpoints as described in [the generic notification article](webhooks.md#managing-subscriptions).</span></span>
<span data-ttu-id="d5865-127">Se você quiser usar a mesma URL para os dois pontos de extremidade você receberá e responderá a duas solicitações de validação.</span><span class="sxs-lookup"><span data-stu-id="d5865-127">If you choose to use the same URL for both endpoints you will receive and respond to two validation requests.</span></span>

> <span data-ttu-id="d5865-128">**Observação:** Não é possível atualizar (`PATCH`) as assinaturas existentes para adicionar a propriedade **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="d5865-128">**Note:** You cannot update (`PATCH`) the existing subscriptions to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="d5865-129">Você deve remover essas assinaturas existentes, criar novas assinaturas e especificar a propriedade **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="d5865-129">You should remove such existing subscriptions, and create new subscriptions and specify the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="d5865-130">Assinaturas existentes, sem a propriedade **lifecycleNotificationUrl** receberão a `subscriptionRemoved` e `missed` notificações pelas **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="d5865-130">Existing subscriptions without **lifecycleNotificationUrl** property will receive the `subscriptionRemoved` and `missed` notifications via the **notificationUrl**.</span></span> 

## <a name="responding-to-subscriptionremoved-notifications"></a><span data-ttu-id="d5865-131">Responder a notificações subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="d5865-131">Responding to subscriptionRemoved notifications</span></span>

<span data-ttu-id="d5865-132">A `subscriptionRemoved` notificação informa que uma assinatura foi removida e deve ser recriada, se você quiser continuar a receber notificações.</span><span class="sxs-lookup"><span data-stu-id="d5865-132">The `subscriptionRemoved` notification informs you that a subscription has been removed and should be recreated, if you want to continue receiving notifications.</span></span> 

<span data-ttu-id="d5865-133">Você pode criar uma assinatura de longa duração (por exemplo, três dias) e notificações de dados do recurso começarão a fluir para a **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="d5865-133">You can create a long-lived subscription (e.g. 3 days), and resource data notifications will start flowing to the **notificationUrl**.</span></span> <span data-ttu-id="d5865-134">No entanto, as condições de acesso aos dados de recursos podem mudar ao longo do tempo.</span><span class="sxs-lookup"><span data-stu-id="d5865-134">However, the conditions of access to the resource data may change over time.</span></span> <span data-ttu-id="d5865-135">Por exemplo, pode ocorrer um evento no serviço do Outlook que requeira que o aplicativo para que o usuário seja autenticado novamente.</span><span class="sxs-lookup"><span data-stu-id="d5865-135">For example, an event in the Outlook service may occur that requires the app to re-authenticate the user.</span></span> <span data-ttu-id="d5865-136">Nesse caso, o fluxo é:</span><span class="sxs-lookup"><span data-stu-id="d5865-136">In such a case, the flow looks as follows:</span></span>

1. <span data-ttu-id="d5865-137">Outlook detecta que uma assinatura precisa ser removido do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d5865-137">Outlook detects that a subscription needs to be removed from Microsoft Graph.</span></span>
    1. <span data-ttu-id="d5865-138">Não há cadência definida para esses eventos.</span><span class="sxs-lookup"><span data-stu-id="d5865-138">There is no set cadence for these events.</span></span> <span data-ttu-id="d5865-139">Eles podem ocorrer com frequência para alguns recursos e quase nunca para outros.</span><span class="sxs-lookup"><span data-stu-id="d5865-139">They may occur frequently for some resources, and almost never for others.</span></span>

2. <span data-ttu-id="d5865-140">O Microsoft Graph envia uma `subscriptionRemoved` notificação para a **lifecycleNotificationUrl** (se especificado), ou uma **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="d5865-140">Microsoft Graph sends a `subscriptionRemoved` notification to the **lifecycleNotificationUrl** (if specified), or the **notificationUrl**.</span></span>  

3. <span data-ttu-id="d5865-141">Você pode responder a essa notificação criando uma nova assinatura para o mesmo recurso.</span><span class="sxs-lookup"><span data-stu-id="d5865-141">You can respond to this notification by creating a new subscription for the same resource.</span></span> <span data-ttu-id="d5865-142">Para fazer isso, é necessário apresentar um token de acesso válido; em alguns casos, isso significa que o aplicativo precisa reautenticar o usuário para obter um novo token de acesso válido.</span><span class="sxs-lookup"><span data-stu-id="d5865-142">To do this, you need to present a valid access token; in some cases this means the app needs to re-authenticate the user to obtain a new valid access token.</span></span>

4. <span data-ttu-id="d5865-143">Se você criar uma nova assinatura com êxito, as notificações de recurso começarão a fluir novamente.</span><span class="sxs-lookup"><span data-stu-id="d5865-143">If you successfully create a new subscription, resource notifications will start flowing again.</span></span> <span data-ttu-id="d5865-144">No entanto, se você falhar (por exemplo, o aplicativo não pode obter um token de acesso válido), as notificações do recurso não serão enviadas.</span><span class="sxs-lookup"><span data-stu-id="d5865-144">However, if you fail (for example, the app could not obtain a valid access token), resource notifications will not be sent.</span></span>

5. <span data-ttu-id="d5865-145">Depois de criar uma nova assinatura, você pode sincronizar os dados de recursos para identificar alterações ausentes.</span><span class="sxs-lookup"><span data-stu-id="d5865-145">After creating the new subscription, you can sync the resource data to identify any missing changes.</span></span>

### <a name="subscriptionremoved-notification-example"></a><span data-ttu-id="d5865-146">exemplo de notificação subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="d5865-146">subscriptionRemoved notification example</span></span>

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

<span data-ttu-id="d5865-147">Alguns aspectos a serem observados neste tipo de notificação:</span><span class="sxs-lookup"><span data-stu-id="d5865-147">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="d5865-148">O `"lifecycleEvent": "subscriptionRemoved"` campo designa essa notificação como relacionada à remoção de assinatura.</span><span class="sxs-lookup"><span data-stu-id="d5865-148">The `"lifecycleEvent": "subscriptionRemoved"` field designates this notification as related to subscription removal.</span></span> <span data-ttu-id="d5865-149">Outros tipos de notificações de ciclo de vida também são possíveis, e novos serão disponibilizados no futuro.</span><span class="sxs-lookup"><span data-stu-id="d5865-149">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="d5865-150">A notificação não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.</span><span class="sxs-lookup"><span data-stu-id="d5865-150">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="d5865-151">Assim como as notificações de recursos, as notificações de ciclo de vida podem estar em lote juntas (na matriz **valor**), cada uma com valores possivelmente diferentes **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="d5865-151">Similar to resource notifications, lifecycle notifications may be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="d5865-152">Processe cada notificação no lote de acordo.</span><span class="sxs-lookup"><span data-stu-id="d5865-152">Process each notification in the batch accordingly.</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="d5865-153">Ações a serem executadas</span><span class="sxs-lookup"><span data-stu-id="d5865-153">Actions to take</span></span>

1. <span data-ttu-id="d5865-154">[Aceite](webhooks.md#notifications) o recebimento da notificação respondendo a chamada POSTAGEM com `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="d5865-154">[Acknowledge](webhooks.md#notifications) the receipt of the notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="d5865-155">[Validar](webhooks.md#notifications) a autenticidade da notificação.</span><span class="sxs-lookup"><span data-stu-id="d5865-155">[Validate](webhooks.md#notifications) the authenticity of the notification.</span></span>
3. <span data-ttu-id="d5865-156">Certifique-se de que o aplicativo tenha um token de acesso válido para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="d5865-156">Ensure the app has a valid access token to take the next step.</span></span> 
> <span data-ttu-id="d5865-157">**Observação:** Se você estiver usando uma das [bibliotecas de autenticação](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) elas farão isso para você ao reutilizar um token de cache válido ou obtendo um novo token, inclusive pedindo ao usuário para fazer logon novamente (por exemplo, com uma nova senha).</span><span class="sxs-lookup"><span data-stu-id="d5865-157">**Note:** If you are using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to login again (e.g. with a new password).</span></span> <span data-ttu-id="d5865-158">Observe que a obtenção de um novo token pode falhar, pois as condições de acesso podem ser alteradas e o chamador não poderá mais acessar os dados de recursos.</span><span class="sxs-lookup"><span data-stu-id="d5865-158">Note that obtaining a new token may fail, since the conditions of access may have changed, and the caller may no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="d5865-159">Criar uma nova assinatura usando o processo padrão descrito [aqui](webhooks.md#subscription-request-example).</span><span class="sxs-lookup"><span data-stu-id="d5865-159">Create a new subscription using the standard process described [here](webhooks.md#subscription-request-example).</span></span>

> <span data-ttu-id="d5865-160">**Observação:** essa ação pode falhar, porque as verificações de autorização realizadas pelo sistema podem recusar o aplicativo ou o acesso do usuário ao recurso.</span><span class="sxs-lookup"><span data-stu-id="d5865-160">**Note:** This action may fail, because the authorization checks performed by the system may deny the app or the user access to the resource.</span></span> <span data-ttu-id="d5865-161">Pode ser necessário que o aplicativo obtenha um novo token de acesso do usuário para reautorizar com êxito uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="d5865-161">It may be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> <span data-ttu-id="d5865-162">Você pode tentar essas ações mais tarde, a qualquer momento, por exemplo, quando as condições de acesso mudarem.</span><span class="sxs-lookup"><span data-stu-id="d5865-162">You may retry these actions later, at any time, for example when the conditions of access have change.</span></span> <span data-ttu-id="d5865-163">Quaisquer alterações de recursos no período de tempo de quando a notificação de ciclo de vida foi enviada até quando o aplicativo recriou a assinatura com êxito, serão perdidas.</span><span class="sxs-lookup"><span data-stu-id="d5865-163">Any resource changes in the time period from when the lifecycle notification was sent, to when the app re-creates the subscription successfully, will be lost.</span></span> <span data-ttu-id="d5865-164">O aplicativo precisará buscar essas alterações sozinho.</span><span class="sxs-lookup"><span data-stu-id="d5865-164">The app will need to fetch those changes on its own.</span></span>

5. <span data-ttu-id="d5865-165">Depois de criar a nova assinatura, sincronizar todos os dados de recurso ausentes desde a última hora conhecida que você recebeu uma notificação para esse recurso, Por exemplo: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span><span class="sxs-lookup"><span data-stu-id="d5865-165">After creating the new subscription, sync any missing resource data from the last known time you received a notification for this resource; for example: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span></span>

## <a name="responding-to-missed-notifications"></a><span data-ttu-id="d5865-166">Responder notificações perdidas</span><span class="sxs-lookup"><span data-stu-id="d5865-166">Responding to missed notifications</span></span>

<span data-ttu-id="d5865-167">Esses sinais informam que algumas notificações podem não terem sido entregues.</span><span class="sxs-lookup"><span data-stu-id="d5865-167">These signals inform you that some notifications may have not been delivered.</span></span> <span data-ttu-id="d5865-168">Você deve ignorar ou lidar com esses sinais são.</span><span class="sxs-lookup"><span data-stu-id="d5865-168">You should decide if you ignore or handle these signals.</span></span>

### <a name="notification-example"></a><span data-ttu-id="d5865-169">Exemplo de notificação</span><span class="sxs-lookup"><span data-stu-id="d5865-169">Notification example</span></span>

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

<span data-ttu-id="d5865-170">Alguns aspectos a serem observados neste tipo de notificação:</span><span class="sxs-lookup"><span data-stu-id="d5865-170">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="d5865-171">O `"lifecycleEvent": "missed"` campo designa isso como um sinal de notificações perdidas.</span><span class="sxs-lookup"><span data-stu-id="d5865-171">The `"lifecycleEvent": "missed"` field designates this as a signal about missed notifications.</span></span> <span data-ttu-id="d5865-172">Outros tipos de notificações de ciclo de vida também são possíveis, e novos serão disponibilizados no futuro.</span><span class="sxs-lookup"><span data-stu-id="d5865-172">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="d5865-173">A notificação não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura</span><span class="sxs-lookup"><span data-stu-id="d5865-173">The notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change</span></span>
- <span data-ttu-id="d5865-174">Assim como as notificações de recursos, as notificações de ciclo de vida podem estar em lote juntas (na matriz **valor**), cada uma com valores possivelmente diferentes **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="d5865-174">Similar to resource notifications, lifecycle notifications may be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="d5865-175">Processe cada notificação no lote de acordo.</span><span class="sxs-lookup"><span data-stu-id="d5865-175">Process each notification in the batch accordingly.</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="d5865-176">Ações a serem executadas</span><span class="sxs-lookup"><span data-stu-id="d5865-176">Actions to take</span></span>

1. <span data-ttu-id="d5865-177">[Aceite](webhooks.md#notifications) o recebimento da notificação respondendo a chamada POSTAGEM com `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="d5865-177">[Acknowledge](webhooks.md#notifications) the receipt of the notification, by responding to the POST call with `202 - Accepted`.</span></span>
  - <span data-ttu-id="d5865-178">Caso você ignore estes, sinais, não faça nada.</span><span class="sxs-lookup"><span data-stu-id="d5865-178">If you ignore these, signals, do nothing else.</span></span> <span data-ttu-id="d5865-179">Caso contrário:</span><span class="sxs-lookup"><span data-stu-id="d5865-179">Otherwise, YES.</span></span>
2. <span data-ttu-id="d5865-180">[Validar](webhooks.md#notifications) a autenticidade da notificação.</span><span class="sxs-lookup"><span data-stu-id="d5865-180">[Validate](webhooks.md#notifications) the authenticity of the notification.</span></span>
3. <span data-ttu-id="d5865-181">Executaremos ressincronização de dados completa para identificar as alterações que não foram entregues como notificações.</span><span class="sxs-lookup"><span data-stu-id="d5865-181">Perform a full data resync of the resource to identify the changes that were not delivered as notifications.</span></span> 


## <a name="future-proof-the-code-handling-lifecycle-notifications"></a><span data-ttu-id="d5865-182">À prova de futuro o código lidar com as notificações de ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="d5865-182">Future-proof the code handling lifecycle notifications</span></span>

<span data-ttu-id="d5865-183">No futuro o Microsoft Graph adicionará mais tipos de notificações de ciclo de vida da assinatura.</span><span class="sxs-lookup"><span data-stu-id="d5865-183">In the future Microsoft Graph will add more types of subscription lifecycle notifications.</span></span> <span data-ttu-id="d5865-184">Serão publicadas no mesmo ponto de extremidade: **lifecycleNotificationUrl**, mas terão um valor diferente sob o **lifecycleEvent** e poderão conter um esquema e propriedades ligeiramente diferentes, específicas para o cenário para o qual serão enviadas.</span><span class="sxs-lookup"><span data-stu-id="d5865-184">They will be posted to the same endpoint: **lifecycleNotificationUrl**, but they will have a different value under **lifecycleEvent** and may contain a slightly different schema and properties, specific to the scenario for which they will be issued.</span></span>

<span data-ttu-id="d5865-185">Você deve implementar o código á prova de futuro para que não pare quando o Microsoft Graph apresentar novos tipos de notificações de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="d5865-185">You should implement your code in a future-proof way so it does not break when Microsoft Graph introduces new types of lifecycle notifications.</span></span> <span data-ttu-id="d5865-186">Recomendamos as seguintes abordagens:</span><span class="sxs-lookup"><span data-stu-id="d5865-186">We recommend the following:</span></span>

1. <span data-ttu-id="d5865-187">Identificar explicitamente cada notificação como um evento suportado, usando a propriedade **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="d5865-187">Explicitly identify each notification as an event that you support, using the **lifecycleEvent** property.</span></span> <span data-ttu-id="d5865-188">Por exemplo, procure a `"lifecycleEvent": "subscriptionRemoved"` propriedade para identificar um evento específico e tratá-lo.</span><span class="sxs-lookup"><span data-stu-id="d5865-188">For example, look for the `"lifecycleEvent": "subscriptionRemoved"` property to identify a specific event, and handle it.</span></span>

2. <span data-ttu-id="d5865-189">Fique atento aos anúncios de notificações para novos cenários, pois podem haver mais tipos de notificações de ciclo de vida no futuro.</span><span class="sxs-lookup"><span data-stu-id="d5865-189">Watch for announcements of notifications for new scenarions, as there may be more types of lifecycle notifications in the future.</span></span>

3. <span data-ttu-id="d5865-190">Em seu aplicativo ignore todos os eventos de ciclo de vida que o aplicativo não reconhece e acesse-os para obter conhecimento.</span><span class="sxs-lookup"><span data-stu-id="d5865-190">In your app, ignore any lifecycle events that the app does not recognize, and log them to gain awareness.</span></span>

4. <span data-ttu-id="d5865-191">Se desejar, procure a documentação relacionada às novas notificações de ciclo de vida e implemente o suporte para elas conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="d5865-191">At your discretion, look up the related documentation for new lifecycle notifications and implement support for them as appropriate.</span></span>

## <a name="see-also"></a><span data-ttu-id="d5865-192">Confira também</span><span class="sxs-lookup"><span data-stu-id="d5865-192">See also</span></span>

- [<span data-ttu-id="d5865-193">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="d5865-193">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="d5865-194">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="d5865-194">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="d5865-195">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="d5865-195">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="d5865-196">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="d5865-196">Delete subscription</span></span>](/graph/api/subscription-delete?view=graph-rest-1.0)
- [<span data-ttu-id="d5865-197">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="d5865-197">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
