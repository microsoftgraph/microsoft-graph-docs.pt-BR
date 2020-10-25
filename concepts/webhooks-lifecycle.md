---
title: Reduzir assinaturas ausentes e alterar notificações
description: Os aplicativos que estão se inscrevendo para alterar as notificações de recursos podem ter suas assinaturas removidas e perder algumas notificações de alteração. Os aplicativos devem implementar a lógica para detectar e recuperar da perda e retomar o fluxo de notificação de alteração contínua.
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: e612a3c7aec61b3bf676598f1703d4afb3f4cd6a
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742327"
---
# <a name="reduce-missing-subscriptions-and-change-notifications"></a><span data-ttu-id="f604c-104">Reduzir assinaturas ausentes e alterar notificações</span><span class="sxs-lookup"><span data-stu-id="f604c-104">Reduce missing subscriptions and change notifications</span></span>

<span data-ttu-id="f604c-105">Os aplicativos que estão se inscrevendo para alterar as notificações de recursos podem ter suas assinaturas removidas e perder algumas notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="f604c-105">Apps subscribing to change notifications might get their subscriptions removed and miss some change notifications.</span></span> <span data-ttu-id="f604c-106">Os aplicativos devem implementar a lógica para detectar e recuperar da perda e retomar o fluxo de notificação de alteração contínua.</span><span class="sxs-lookup"><span data-stu-id="f604c-106">Apps should implement logic to detect and recover from the loss, and resume a continuous change notification flow.</span></span>

<span data-ttu-id="f604c-107">Determinados eventos podem fazer que a assinatura seja removida.</span><span class="sxs-lookup"><span data-stu-id="f604c-107">Certain events can cause a subscription to be removed.</span></span> <span data-ttu-id="f604c-108">Esses eventos incluem:</span><span class="sxs-lookup"><span data-stu-id="f604c-108">These events include:</span></span>

- <span data-ttu-id="f604c-109">A senha do usuário foi redefinida</span><span class="sxs-lookup"><span data-stu-id="f604c-109">User's password has been reset</span></span>
- <span data-ttu-id="f604c-110">Dispositivo do usuário está fora de conformidade</span><span class="sxs-lookup"><span data-stu-id="f604c-110">User's device is out of compliance</span></span>
-   <span data-ttu-id="f604c-111">Conta do usuário foi revogada</span><span class="sxs-lookup"><span data-stu-id="f604c-111">User's account has been revoked</span></span>

<span data-ttu-id="f604c-112">Quando ocorre um evento, o Outlook envia uma notificação de ciclo de vida especial `subscriptionRemoved`.</span><span class="sxs-lookup"><span data-stu-id="f604c-112">When such an event happens, Outlook sends a special lifecycle notification, `subscriptionRemoved`.</span></span>

<span data-ttu-id="f604c-113">O Outlook também envia outra notificação do ciclo de vida, `missed`, caso não seja possível entregar uma notificação de alteração a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f604c-113">Outlook also sends another lifecycle notification, `missed`, if a change notification cannot be delivered to an app.</span></span>

<span data-ttu-id="f604c-114">Uma assinatura de um aplicativo para modificar as notificações deve ouvir os sinais `subscriptionRemoved` e `missed` e fazer o seguinte:</span><span class="sxs-lookup"><span data-stu-id="f604c-114">An app subscribing to change notifications should listen to the `subscriptionRemoved` and `missed` signals and do the following:</span></span>

- <span data-ttu-id="f604c-115">Após receber uma notificação de `subscriptionRemoved` ciclo de vida, o aplicativo deve recriar a assinatura para manter um fluxo contínuo.</span><span class="sxs-lookup"><span data-stu-id="f604c-115">Upon receiving a `subscriptionRemoved` lifecycle notification, the app should recreate the subscription in order to maintain a continuous flow.</span></span>
- <span data-ttu-id="f604c-116">Ao receber uma notificação de `missed` ciclo de vida, o aplicativo deve ressincronizar os dados de recurso usando o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f604c-116">On receiving a `missed` lifecycle notification, the app should resynchronize resource data using Microsoft Graph.</span></span>

<span data-ttu-id="f604c-117">Para receber notificações de ciclo de vida, você pode usar o ponto de extremidade existente **notificationUrl** que já recebe notificações de alteração, ou você pode registrar um **lifecycleNotificationUrl** separado para receber `subscriptionRemoved` e `missed` notificações de ciclo de vida em um ponto de extremidade separado.</span><span class="sxs-lookup"><span data-stu-id="f604c-117">To receive lifecycle notifications, you can use the existing **notificationUrl** endpoint that already receives change notifications, or you can register a separate **lifecycleNotificationUrl** to receive `subscriptionRemoved` and `missed` lifecycle notifications in a separate endpoint.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="f604c-118">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="f604c-118">Creating a subscription</span></span>

<span data-ttu-id="f604c-119">Ao criar uma assinatura, você deve especificar um ponto de extremidade de notificação separado usando a propriedade **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="f604c-119">When creating a subscription, you must specify a separate notification endpoint using the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="f604c-120">Se você especificar o ponto de extremidade, todos os tipos de atuais e futuros de notificações de ciclo de vida serão entregues lá.</span><span class="sxs-lookup"><span data-stu-id="f604c-120">If you specify the endpoint, all current and future types of lifecycle notifications will be delivered there.</span></span> <span data-ttu-id="f604c-121">Caso contrário, as notificações do ciclo de vida `subscriptionRemoved` e `missed` não serão entregues.</span><span class="sxs-lookup"><span data-stu-id="f604c-121">Otherwise, `subscriptionRemoved` and `missed` lifecycle notifications will not be delivered.</span></span> <span data-ttu-id="f604c-122">Esse ponto de extremidade pode ser o mesmo que a **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="f604c-122">This endpoint can be the same as the **notificationUrl**.</span></span>

### <a name="subscription-request-example"></a><span data-ttu-id="f604c-123">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="f604c-123">Subscription request example</span></span>

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
> <span data-ttu-id="f604c-124">Use o mesmo nome de host (FQDN) para ambas as notificações URLs.</span><span class="sxs-lookup"><span data-stu-id="f604c-124">Use the same hostname (FQDN) for both notifications URLs.</span></span> 

<span data-ttu-id="f604c-125">É necessário validar ambos os pontos de extremidade conforme descrito em [Gerenciar assinaturas](webhooks.md#managing-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="f604c-125">You need to validate both endpoints, as described in [Managing subscriptions](webhooks.md#managing-subscriptions).</span></span> <span data-ttu-id="f604c-126">Se você quiser usar a mesma URL para os dois pontos de extremidade, você receberá e responderá a duas solicitações de validação.</span><span class="sxs-lookup"><span data-stu-id="f604c-126">If you choose to use the same URL for both endpoints, you will receive and respond to two validation requests.</span></span>

> <span data-ttu-id="f604c-127">**Observação:** Não é possível atualizar (`PATCH`) as assinaturas existentes para adicionar a propriedade **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="f604c-127">**Note:** You cannot update (`PATCH`) the existing subscriptions to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="f604c-128">Você deve remover essas assinaturas existentes, criar novas assinaturas e especificar a propriedade **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="f604c-128">You should remove such existing subscriptions, create new subscriptions, and specify the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="f604c-129">As assinaturas existentes sem uma propriedade **lifecycleNotificationUrl** não receberão as `subscriptionRemoved` e `missed` notificações.</span><span class="sxs-lookup"><span data-stu-id="f604c-129">Existing subscriptions without a **lifecycleNotificationUrl** property will not receive the `subscriptionRemoved` and `missed` notifications.</span></span>

## <a name="responding-to-subscriptionremoved-notifications"></a><span data-ttu-id="f604c-130">Responder a notificações subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="f604c-130">Responding to subscriptionRemoved notifications</span></span>

<span data-ttu-id="f604c-131">A notificação de `subscriptionRemoved` ciclo de vida informa que uma assinatura foi removida e deve ser recriada, se você quiser continuar a receber as notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="f604c-131">The `subscriptionRemoved` lifecycle notification informs you that a subscription has been removed and should be recreated, if you want to continue receiving change notifications.</span></span> 

<span data-ttu-id="f604c-132">Você pode criar uma assinatura de longa duração (três dias) e as notificações de alteração começarão a fluir para o **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="f604c-132">You can create a long-lived subscription (3 days), and change notifications will start flowing to the **notificationUrl**.</span></span> <span data-ttu-id="f604c-133">No entanto, as condições de acesso aos dados de recursos podem mudar ao longo do tempo.</span><span class="sxs-lookup"><span data-stu-id="f604c-133">However, the conditions of access to the resource data might change over time.</span></span> <span data-ttu-id="f604c-134">Por exemplo, pode ocorrer um evento no serviço que exija que o aplicativo autentique novamente o usuário.</span><span class="sxs-lookup"><span data-stu-id="f604c-134">For example, an event in the service might occur that requires the app to re-authenticate the user.</span></span> <span data-ttu-id="f604c-135">Nesse caso, o fluxo é:</span><span class="sxs-lookup"><span data-stu-id="f604c-135">In such a case, the flow is as follows:</span></span>

1. <span data-ttu-id="f604c-136">O serviço detecta que uma assinatura precisa ser removida do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f604c-136">The service detects that a subscription needs to be removed from Microsoft Graph.</span></span>
    
    <span data-ttu-id="f604c-137">Não há cadência definida para esses eventos.</span><span class="sxs-lookup"><span data-stu-id="f604c-137">There is no set cadence for these events.</span></span> <span data-ttu-id="f604c-138">Eles podem ocorrer com frequência para alguns recursos e quase nunca para outros.</span><span class="sxs-lookup"><span data-stu-id="f604c-138">They might occur frequently for some resources, and almost never for others.</span></span>

2. <span data-ttu-id="f604c-139">O Microsoft Graph envia uma notificação `subscriptionRemoved` de ciclo de vida para **lifecycleNotificationUrl** (se especificado).</span><span class="sxs-lookup"><span data-stu-id="f604c-139">Microsoft Graph sends a `subscriptionRemoved` lifecycle notification to the **lifecycleNotificationUrl** (if specified).</span></span>  

3. <span data-ttu-id="f604c-140">Você pode responder a essa notificação do ciclo de vida criando uma nova assinatura para o mesmo recurso.</span><span class="sxs-lookup"><span data-stu-id="f604c-140">You can respond to this lifecycle notification by creating a new subscription for the same resource.</span></span> <span data-ttu-id="f604c-141">Para fazer isso, é necessário apresentar um token de acesso válido; em alguns casos, isso significa que o aplicativo precisa reautenticar o usuário para obter um novo token de acesso válido.</span><span class="sxs-lookup"><span data-stu-id="f604c-141">To do this, you need to present a valid access token; in some cases this means the app needs to re-authenticate the user to obtain a new valid access token.</span></span>

4. <span data-ttu-id="f604c-142">Se você criar uma nova assinatura com êxito, as notificações de alteração de recurso começarão a fluir novamente.</span><span class="sxs-lookup"><span data-stu-id="f604c-142">If you successfully create a new subscription, change notifications will start flowing again.</span></span> <span data-ttu-id="f604c-143">No entanto, se houver falha (por exemplo, o aplicativo não pode obter um token de acesso válido), as notificações de alteração não serão enviadas.</span><span class="sxs-lookup"><span data-stu-id="f604c-143">However, if you fail (for example, the app can't obtain a valid access token), change notifications will not be sent.</span></span>

5. <span data-ttu-id="f604c-144">Depois de criar uma nova assinatura, você pode sincronizar os dados de recursos para identificar alterações ausentes.</span><span class="sxs-lookup"><span data-stu-id="f604c-144">After creating the new subscription, you can sync the resource data to identify any missing changes.</span></span>

### <a name="subscriptionremoved-notification-example"></a><span data-ttu-id="f604c-145">exemplo de notificação subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="f604c-145">subscriptionRemoved notification example</span></span>

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

<span data-ttu-id="f604c-146">Alguns aspectos a serem observados neste tipo de notificação:</span><span class="sxs-lookup"><span data-stu-id="f604c-146">A few things to note about this type of notification:</span></span>

- <span data-ttu-id="f604c-147">O `"lifecycleEvent": "subscriptionRemoved"` campo designa essa notificação como relacionada à remoção de assinatura.</span><span class="sxs-lookup"><span data-stu-id="f604c-147">The `"lifecycleEvent": "subscriptionRemoved"` field designates this notification as related to subscription removal.</span></span> <span data-ttu-id="f604c-148">Outros tipos de notificações de ciclo de vida também são possíveis, e novos serão disponibilizados no futuro.</span><span class="sxs-lookup"><span data-stu-id="f604c-148">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="f604c-149">A notificação de ciclo de vida não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.</span><span class="sxs-lookup"><span data-stu-id="f604c-149">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="f604c-150">Assim como notificações de alteração, notificações de ciclo de vida devem ser agrupadas (na matriz **valor**), cada com uma possivelmente valores diferentes **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="f604c-150">Similar to change notifications, lifecycle notifications can be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="f604c-151">Processe cada notificação de ciclo de vida no lote adequadamente.</span><span class="sxs-lookup"><span data-stu-id="f604c-151">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="f604c-152">**Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração forem entregues, confira [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="f604c-152">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="f604c-153">Ações a serem executadas</span><span class="sxs-lookup"><span data-stu-id="f604c-153">Actions to take</span></span>

1. <span data-ttu-id="f604c-154">[Confirme](webhooks.md#change-notifications) o recebimento da notificação do ciclo de vida respondendo à chamada do POST com `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="f604c-154">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="f604c-155">[Validar](webhooks.md#change-notifications) a autenticidade da notificação do ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="f604c-155">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="f604c-156">Certifique-se de que o aplicativo tenha um token de acesso válido para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="f604c-156">Ensure that the app has a valid access token to take the next step.</span></span> 
  > <span data-ttu-id="f604c-157">**Observação**: se você estiver usando uma das [bibliotecas de autenticação](/azure/active-directory/develop/reference-v2-libraries), elas farão isso para você ao reutilizar um token de cache válido ou obtendo um novo token, inclusive pedindo ao usuário para fazer logon novamente (com uma nova senha).</span><span class="sxs-lookup"><span data-stu-id="f604c-157">**Note:** If you're using one of the [authentication libraries](/azure/active-directory/develop/reference-v2-libraries), they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to sign in again (with a new password).</span></span> <span data-ttu-id="f604c-158">Observe que a obtenção de um novo token pode falhar, pois as condições de acesso podem ser alteradas e o chamador não poderá mais acessar os dados de recursos. </span><span class="sxs-lookup"><span data-stu-id="f604c-158">Note that obtaining a new token might fail, because the conditions of access might have changed, and the caller might no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="f604c-159">Criar uma nova assinatura usando o processo padrão descrito [aqui](webhooks.md#subscription-request-example).</span><span class="sxs-lookup"><span data-stu-id="f604c-159">Create a new subscription using the standard process described [here](webhooks.md#subscription-request-example).</span></span>

  > <span data-ttu-id="f604c-160">**Observação:** essa ação pode falhar, porque as verificações de autorização realizadas pelo sistema podem recusar o aplicativo ou o acesso do usuário ao recurso.</span><span class="sxs-lookup"><span data-stu-id="f604c-160">**Note:** This action might fail, because the authorization checks performed by the system might deny the app or the user access to the resource.</span></span> <span data-ttu-id="f604c-161">Pode ser necessário que o aplicativo obtenha um novo token de acesso do usuário para reautorizar uma assinatura com êxito.</span><span class="sxs-lookup"><span data-stu-id="f604c-161">It might be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> <span data-ttu-id="f604c-162">Você pode tentar essa ações mais tarde, a qualquer momento; por exemplo, quando as condições de acesso mudarem.</span><span class="sxs-lookup"><span data-stu-id="f604c-162">You can retry these actions later, at any time; for example, when the conditions of access have changed.</span></span> <span data-ttu-id="f604c-163">Quaisquer alterações de recursos no período de quando a notificação de ciclo de vida foi enviada até quando o aplicativo recriou a assinatura com êxito, serão perdidas.</span><span class="sxs-lookup"><span data-stu-id="f604c-163">Any resource changes in the time period from when the lifecycle notification was sent, to when the app recreates the subscription successfully, will be lost.</span></span> <span data-ttu-id="f604c-164">O aplicativo precisará buscar essas alterações sozinho.</span><span class="sxs-lookup"><span data-stu-id="f604c-164">The app will need to fetch those changes on its own.</span></span>

5. <span data-ttu-id="f604c-165">Depois de criar a nova assinatura, sincronizar todos os dados de recurso ausentes desde a última vez que você recebeu uma notificação para esse recurso, Por exemplo: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span><span class="sxs-lookup"><span data-stu-id="f604c-165">After creating the new subscription, sync any missing resource data from the last known time you received a change notification for this resource; for example: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span></span>

## <a name="responding-to-missed-notifications"></a><span data-ttu-id="f604c-166">Responder notificações perdidas</span><span class="sxs-lookup"><span data-stu-id="f604c-166">Responding to missed notifications</span></span>

<span data-ttu-id="f604c-167">Esses sinais informam que algumas notificações podem não ter sido entregues.</span><span class="sxs-lookup"><span data-stu-id="f604c-167">These signals inform you that some change notifications might not have been delivered.</span></span> <span data-ttu-id="f604c-168">Você deve ignorar ou lidar com esses sinais são.</span><span class="sxs-lookup"><span data-stu-id="f604c-168">You should decide if you ignore or handle these signals.</span></span>

### <a name="notification-example"></a><span data-ttu-id="f604c-169">Exemplo de notificação</span><span class="sxs-lookup"><span data-stu-id="f604c-169">Notification example</span></span>

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

<span data-ttu-id="f604c-170">Alguns aspectos a serem observados neste tipo de notificação:</span><span class="sxs-lookup"><span data-stu-id="f604c-170">A few things to note about this type of notification:</span></span>

- <span data-ttu-id="f604c-171">O `"lifecycleEvent": "missed"` campo designa isso como um sinal de notificações perdidas.</span><span class="sxs-lookup"><span data-stu-id="f604c-171">The `"lifecycleEvent": "missed"` field designates this as a signal about missed change notifications.</span></span> <span data-ttu-id="f604c-172">Outros tipos de notificações de ciclo de vida também são possíveis, e novos serão disponibilizados no futuro.</span><span class="sxs-lookup"><span data-stu-id="f604c-172">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="f604c-173">A notificação de ciclo de vida não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.</span><span class="sxs-lookup"><span data-stu-id="f604c-173">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="f604c-174">Assim como notificações de alteração, notificações de ciclo de vida podem ser agrupadas (na matriz **valor**), cada com uma possivelmente valores diferentes **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="f604c-174">Similar to change notifications, lifecycle notifications might be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="f604c-175">Processe cada notificação de ciclo de vida no lote adequadamente.</span><span class="sxs-lookup"><span data-stu-id="f604c-175">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="f604c-176">**Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração forem entregues, confira [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="f604c-176">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="f604c-177">Ações a serem executadas</span><span class="sxs-lookup"><span data-stu-id="f604c-177">Actions to take</span></span>

1. <span data-ttu-id="f604c-178">[Confirme](webhooks.md#change-notifications) o recebimento da notificação do ciclo de vida respondendo à chamada do POST com `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="f604c-178">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
    - <span data-ttu-id="f604c-179">Caso você ignore estes sinais, não faça nada.</span><span class="sxs-lookup"><span data-stu-id="f604c-179">If you ignore these signals, do nothing else.</span></span> <span data-ttu-id="f604c-180">Caso contrário:</span><span class="sxs-lookup"><span data-stu-id="f604c-180">Otherwise:</span></span>
2. <span data-ttu-id="f604c-181">[Validar](webhooks.md#change-notifications) a autenticidade da notificação do ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="f604c-181">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="f604c-182">Executaremos ressincronização de dados completa para identificar as alterações que não foram entregues como notificações.</span><span class="sxs-lookup"><span data-stu-id="f604c-182">Perform a full data resync of the resource to identify the changes that were not delivered as notifications.</span></span> 

## <a name="responding-to-reauthorizationrequired-notifications"></a><span data-ttu-id="f604c-183">Respondendo a notificações reauthorizationRequired</span><span class="sxs-lookup"><span data-stu-id="f604c-183">Responding to reauthorizationRequired notifications</span></span>

<span data-ttu-id="f604c-184">Quando receber uma notificação `reauthorizationRequired` de ciclo de vida, você deve reautorizar a inscrição para manter o fluxo de dados.</span><span class="sxs-lookup"><span data-stu-id="f604c-184">When you receive a `reauthorizationRequired` lifecycle notification, you must reauthorize the subscription to maintain the data flow.</span></span>

<span data-ttu-id="f604c-185">Você pode criar uma inscrição de longa duração (três dias) e as notificações de alteração começarão a fluir para o **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="f604c-185">You can create a long-lived subscription (3 days), which enables change notifications to flow to the **notificationUrl**.</span></span> <span data-ttu-id="f604c-186">Caso as condições de acesso tenham sido alteradas desde a criação da assinatura, o Microsoft Graph pode exigir que você recrie a assinatura para provar que ainda tem acesso aos dados do recurso.</span><span class="sxs-lookup"><span data-stu-id="f604c-186">If the conditions of access have changed since the subscription was created, Microsoft Graph may require that you reauthorize the subscription to prove that you still have access to resource data.</span></span> <span data-ttu-id="f604c-187">A seguir estão exemplos de alterações que afetam o acesso aos dados:</span><span class="sxs-lookup"><span data-stu-id="f604c-187">The following are examples of changes that affect your access to data:</span></span>

- <span data-ttu-id="f604c-188">Um administrador de locatários pode revogar as permissões do seu aplicativo para ler um recurso.</span><span class="sxs-lookup"><span data-stu-id="f604c-188">A tenant administrator may revoke your app's permissions to read a resource.</span></span>
- <span data-ttu-id="f604c-189">Em um cenário interativo, o usuário que fornece o token de autenticação ao seu aplicativo pode estar sujeito a políticas dinâmicas com base em vários fatores, como o local, o estado do dispositivo ou a avaliação de risco.</span><span class="sxs-lookup"><span data-stu-id="f604c-189">In an interactive scenario, the user who provides the authentication token to your app may be subject to dynamic policies based on various factors, such as their location, device state, or risk assesment.</span></span> <span data-ttu-id="f604c-190">Por exemplo, se o usuário alterar o seu local físico, pode ser que ele não tenha mais permissão para acessar os dados e seu aplicativo não conseguirá autorizar novamente a assinatura.</span><span class="sxs-lookup"><span data-stu-id="f604c-190">For example, if the user changes their physical location, the user may no longer be allowed to access the data, and your app will not be able to reauthorize the subscription.</span></span> <span data-ttu-id="f604c-191">Para saber mais sobre políticas dinâmicas que controlam o acesso, confira [Políticas de acesso condicional do Azure AD](/azure/active-directory/conditional-access/overview).</span><span class="sxs-lookup"><span data-stu-id="f604c-191">For more information about dynamic policies that control access, see [Azure AD conditional access policies](/azure/active-directory/conditional-access/overview).</span></span> 

<span data-ttu-id="f604c-192">As etapas a seguir representam o fluxo de um desafio de autorização para uma assinatura ativa:</span><span class="sxs-lookup"><span data-stu-id="f604c-192">The following steps represent the flow of an authorization challenge for an active subscription:</span></span>

1. <span data-ttu-id="f604c-193">O Microsoft Graph exige que uma assinatura seja autorizada novamente.</span><span class="sxs-lookup"><span data-stu-id="f604c-193">Microsoft Graph requires a subscription to be reauthorized.</span></span>
    
    <span data-ttu-id="f604c-194">Os motivos para isso podem variar de recurso para recurso e podem mudar com o tempo.</span><span class="sxs-lookup"><span data-stu-id="f604c-194">The reasons for this may vary from resource to resource, and may change over time.</span></span> <span data-ttu-id="f604c-195">Você deve responder a um evento de nova autorização, não importa o que o causou.</span><span class="sxs-lookup"><span data-stu-id="f604c-195">You must respond to a reauthorization event no matter what caused it.</span></span>

2. <span data-ttu-id="f604c-196">O Microsoft Graph envia uma notificação de desafio de autorização para **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="f604c-196">Microsoft Graph sends an authorization challenge notification to the **lifecycleNotificationUrl**.</span></span>

    <span data-ttu-id="f604c-197">Observe que o fluxo de notificações de alterações pode continuar por um tempo, dando a você tempo extra para responder.</span><span class="sxs-lookup"><span data-stu-id="f604c-197">Note that the flow of change notifications may continue for a while, giving you extra time to respond.</span></span> <span data-ttu-id="f604c-198">No entanto, eventualmente a alteração na entrega de notificação fará uma pausa até você executar a ação necessária.</span><span class="sxs-lookup"><span data-stu-id="f604c-198">However, eventually change notification delivery pauses, until you take the required action.</span></span>

3. <span data-ttu-id="f604c-199">Responda a esta notificação do ciclo de vida de duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="f604c-199">Respond to this lifecycle notification in one of two ways:</span></span>
    - <span data-ttu-id="f604c-200">Autorizar a assinatura novamente.</span><span class="sxs-lookup"><span data-stu-id="f604c-200">Reauthorize the subscription.</span></span> <span data-ttu-id="f604c-201">Isso não estende a data de vencimento da assinatura.</span><span class="sxs-lookup"><span data-stu-id="f604c-201">This does not extend the expiry date of the subscription.</span></span>
    - <span data-ttu-id="f604c-202">Renove a assinatura.</span><span class="sxs-lookup"><span data-stu-id="f604c-202">Renew the subscription.</span></span> <span data-ttu-id="f604c-203">Isso autoriza novamente e estende a data de vencimento.</span><span class="sxs-lookup"><span data-stu-id="f604c-203">This both reauthorizes and extends the expiry date.</span></span>

    <span data-ttu-id="f604c-204">Observação: as duas ações exigem a apresentação de um token de autenticação válido, semelhante a [criar uma nova assinatura](webhooks.md#creating-a-subscription) ou [renova uma assinatura antes da sua expiração](webhooks.md#renewing-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="f604c-204">Note: Both actions require you to present a valid authentication token, similar to [creating a new subscription](webhooks.md#creating-a-subscription) or [renewing a subscription before its expiry](webhooks.md#renewing-a-subscription).</span></span>

4. <span data-ttu-id="f604c-205">Se você autorizar novamente ou renovar com êxito a inscrição, as notificações de alteração continuarão.</span><span class="sxs-lookup"><span data-stu-id="f604c-205">If you successfully reauthorize or renew the subscription, change notifications continue.</span></span> <span data-ttu-id="f604c-206">Caso contrário, as notificações de alteração permanecerão pausadas.</span><span class="sxs-lookup"><span data-stu-id="f604c-206">Otherwise, change notifications remain paused.</span></span>

### <a name="reauthorizationrequired-notification-example"></a><span data-ttu-id="f604c-207">exemplo de notificação reauthorizationRequired</span><span class="sxs-lookup"><span data-stu-id="f604c-207">reauthorizationRequired notification example</span></span>

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

<span data-ttu-id="f604c-208">Alguns aspectos a serem observados neste tipo de notificação:</span><span class="sxs-lookup"><span data-stu-id="f604c-208">A few things to note about this type of notification:</span></span>

- <span data-ttu-id="f604c-209">O campo `"lifecycleEvent": "reauthorizationRequired"` identifica essa notificação como um desafio de autorização.</span><span class="sxs-lookup"><span data-stu-id="f604c-209">The `"lifecycleEvent": "reauthorizationRequired"` field designates this notification as an authorization challenge.</span></span> <span data-ttu-id="f604c-210">Outros tipos de notificações de ciclo de vida também são possíveis, e novos serão disponibilizados no futuro.</span><span class="sxs-lookup"><span data-stu-id="f604c-210">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="f604c-211">A notificação de ciclo de vida não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.</span><span class="sxs-lookup"><span data-stu-id="f604c-211">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="f604c-212">Semelhante às notificações de alteração, você pode agrupar as notificações do ciclo de vida em conjunto (na coleção de**valores**), cada uma com um valor possivelmente diferente do **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="f604c-212">Similar to change notifications, you can batch lifecycle notifications together (in the **value** collection), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="f604c-213">Processe cada notificação de ciclo de vida no lote adequadamente.</span><span class="sxs-lookup"><span data-stu-id="f604c-213">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="f604c-214">**Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração forem entregues, confira [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="f604c-214">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="f604c-215">Ações a serem executadas</span><span class="sxs-lookup"><span data-stu-id="f604c-215">Actions to take</span></span>

1. <span data-ttu-id="f604c-216">[Confirme](webhooks.md#change-notifications) o recebimento da notificação do ciclo de vida respondendo à chamada do POST com `202 - Accepted`.</span><span class="sxs-lookup"><span data-stu-id="f604c-216">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="f604c-217">[Validar](webhooks.md#change-notifications) a autenticidade da notificação do ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="f604c-217">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="f604c-218">Certifique-se de que o aplicativo tenha um token de acesso válido para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="f604c-218">Ensure that the app has a valid access token to take the next step.</span></span> 
  > <span data-ttu-id="f604c-219">**Observação**: se você estiver usando uma das [bibliotecas de autenticação](/azure/active-directory/develop/reference-v2-libraries), elas farão isso para você ao reutilizar um token de cache válido ou obtendo um novo token, inclusive pedindo ao usuário para fazer logon novamente (com uma nova senha).</span><span class="sxs-lookup"><span data-stu-id="f604c-219">**Note:** If you're using one of the [authentication libraries](/azure/active-directory/develop/reference-v2-libraries), they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to sign in again (with a new password).</span></span> <span data-ttu-id="f604c-220">Observe que a obtenção de um novo token pode falhar, pois as condições de acesso podem ser alteradas e o chamador não poderá mais acessar os dados de recursos. </span><span class="sxs-lookup"><span data-stu-id="f604c-220">Note that obtaining a new token might fail, because the conditions of access might have changed, and the caller might no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="f604c-221">Chamar uma das duas APIs a seguir.</span><span class="sxs-lookup"><span data-stu-id="f604c-221">Call either of the following two APIs.</span></span> <span data-ttu-id="f604c-222">Se a chamada da API for bem-sucedida, o fluxo de notificação de mudança será retomado.</span><span class="sxs-lookup"><span data-stu-id="f604c-222">If the API call succeeds, the change notification flow resumes.</span></span>

    - <span data-ttu-id="f604c-223">Chame a ação `/reauthorize` para autorizar novamente a assinatura sem estender a data de vencimento:</span><span class="sxs-lookup"><span data-stu-id="f604c-223">Call the `/reauthorize` action to reauthorize the subscription without extending its expiration date:</span></span>
        ```http
        POST  https://graph.microsoft.com/beta/subscriptions/{id}/reauthorize
        Content-type: application/json
        ```
    - <span data-ttu-id="f604c-224">Execute uma ação de renovação regular para autorizar novamente e renovar a assinatura ao mesmo tempo:</span><span class="sxs-lookup"><span data-stu-id="f604c-224">Perform a regular renew action to reauthorize and renew the subscription at the same time:</span></span>
        ```http
        PATCH https://graph.microsoft.com/beta/subscriptions/{id}
        Content-Type: application/json

        {
           "expirationDateTime": "2019-09-21T11:00:00.0000000Z"
        }
        ```

      <span data-ttu-id="f604c-225">A renovação pode falhar, porque as verificações de autorização realizadas pelo sistema podem recusar o aplicativo ou o acesso do usuário ao recurso.</span><span class="sxs-lookup"><span data-stu-id="f604c-225">Renewing may fail, because the authorization checks performed by the system may deny the app or the user access to the resource.</span></span> <span data-ttu-id="f604c-226">Pode ser necessário que o aplicativo obtenha um novo token de acesso do usuário para reautorizar com êxito uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="f604c-226">It may be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> 
      
      <span data-ttu-id="f604c-227">Você pode tentar essa ações mais tarde, a qualquer momento e obter êxito se as condições de acesso mudarem.</span><span class="sxs-lookup"><span data-stu-id="f604c-227">You may retry these actions later, at any time, and succeed if the conditions of access change.</span></span> <span data-ttu-id="f604c-228">As notificações sobre as alterações de recursos que acontecem entre o tempo de envio da notificação do ciclo de vida e o momento em que o aplicativo cria a assinatura novamente, seriam perdidas.</span><span class="sxs-lookup"><span data-stu-id="f604c-228">Any notifications about resource changes that happen between the time the lifecycle notification was sent and the time when the app successfully creates the subscription again, would be lost.</span></span> <span data-ttu-id="f604c-229">Nesses casos, o aplicativo deve buscar essas mudanças separadamente.</span><span class="sxs-lookup"><span data-stu-id="f604c-229">In such cases, the app should separately fetch those changes.</span></span>

### <a name="additional-information"></a><span data-ttu-id="f604c-230">Informações adicionais</span><span class="sxs-lookup"><span data-stu-id="f604c-230">Additional information</span></span>

<span data-ttu-id="f604c-231">As informações a seguir podem ajudá-lo a entender os desafios de autorização:</span><span class="sxs-lookup"><span data-stu-id="f604c-231">The following information can help you understand authorization challenges:</span></span>

- <span data-ttu-id="f604c-232">Os desafios de autorização não substituem a necessidade de renova uma assinatura de alteração de recursos antes de expirar.</span><span class="sxs-lookup"><span data-stu-id="f604c-232">Authorization challenges do not replace the need to renew a resource change subscription before it expires.</span></span> 

    <span data-ttu-id="f604c-233">Embora você possa optar por renovar uma assinatura quando recebe um desafio de autorização, o Microsoft Graph pode não desafiar todas as suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="f604c-233">While you can choose to renew a subscription when you receive an authorization challenge, Microsoft Graph may not challenge all of your subscriptions.</span></span> <span data-ttu-id="f604c-234">Por exemplo, uma assinatura que não possui nenhuma atividade e não possui notificações de alterações com entrega pendente pode não sinalizar nenhum desafio para uma nova autorização do seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f604c-234">For example, a subscription that does not have any activity and has no change notifications pending delivery may not signal any reauthorization challenges to your app.</span></span> <span data-ttu-id="f604c-235">Certifique-se de [renovar assinaturas](webhooks.md#renewing-a-subscription) antes de expirarem.</span><span class="sxs-lookup"><span data-stu-id="f604c-235">Make sure to [renew subscriptions](webhooks.md#renewing-a-subscription) before they expire.</span></span>

- <span data-ttu-id="f604c-236">A frequência dos desafios de autorização está sujeita a mudanças.</span><span class="sxs-lookup"><span data-stu-id="f604c-236">The frequency of authorization challenges is subject to change.</span></span>

    <span data-ttu-id="f604c-237">Não faça suposições sobre a frequência dos desafios de autorização.</span><span class="sxs-lookup"><span data-stu-id="f604c-237">Do not make assumptions about the frequency of authorization challenges.</span></span> <span data-ttu-id="f604c-238">Essas notificações do ciclo de vida informam quando você deve executar as ações, evitando que você precise rastrear quais assinaturas requerem uma nova autorização.</span><span class="sxs-lookup"><span data-stu-id="f604c-238">These lifecycle notifications tell you when to take actions, saving you from having to track which subscriptions require reauthorization.</span></span> <span data-ttu-id="f604c-239">Esteja pronto para lidar com os desafios de autorização de vez em quando, para todas as assinaturas até raramente para apenas algumas das suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="f604c-239">Be ready to handle authorization challenges from once every few minutes for every subscription to rarely for only some of your subscriptions.</span></span>

## <a name="future-proof-the-code-handling-lifecycle-notifications"></a><span data-ttu-id="f604c-240">À prova de futuro o código lidar com as notificações de ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="f604c-240">Future-proof the code handling lifecycle notifications</span></span>

<span data-ttu-id="f604c-241">No futuro, o Microsoft Graph adicionará mais tipos de notificações de ciclo de vida da assinatura.</span><span class="sxs-lookup"><span data-stu-id="f604c-241">In the future, Microsoft Graph will add more types of subscription lifecycle notifications.</span></span> <span data-ttu-id="f604c-242">Elas serão publicadas no mesmo ponto de extremidade: **lifecycleNotificationUrl**, mas terão um valor diferente sob **lifecycleEvent** e podem conter um esquema e propriedades ligeiramente diferentes, específicas para o cenário para o qual serão enviadas.</span><span class="sxs-lookup"><span data-stu-id="f604c-242">They will be posted to the same endpoint: **lifecycleNotificationUrl**, but they will have a different value under **lifecycleEvent** and might contain a slightly different schema and properties, specific to the scenario for which they will be issued.</span></span>

<span data-ttu-id="f604c-243">Você deve implementar o código á prova de futuro para que não pare quando o Microsoft Graph apresentar novos tipos de notificações de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="f604c-243">You should implement your code in a future-proof way so it does not break when Microsoft Graph introduces new types of lifecycle notifications.</span></span> <span data-ttu-id="f604c-244">Recomendamos as seguintes abordagens:</span><span class="sxs-lookup"><span data-stu-id="f604c-244">We recommend the following approach:</span></span>

1. <span data-ttu-id="f604c-245">Identifique explicitamente cada notificação do ciclo de vida como um evento que você oferece suporte, usando a propriedade **lifecycleEvent**.</span><span class="sxs-lookup"><span data-stu-id="f604c-245">Explicitly identify each lifecycle notification as an event that you support, using the **lifecycleEvent** property.</span></span> <span data-ttu-id="f604c-246">Por exemplo, procure a `"lifecycleEvent": "subscriptionRemoved"` propriedade para identificar um evento específico e tratá-lo.</span><span class="sxs-lookup"><span data-stu-id="f604c-246">For example, look for the `"lifecycleEvent": "subscriptionRemoved"` property to identify a specific event, and handle it.</span></span>

2. <span data-ttu-id="f604c-247">Assista aos comunicados de notificações do ciclo de vida para ver novos cenários.</span><span class="sxs-lookup"><span data-stu-id="f604c-247">Watch for announcements of lifecycle notifications for new scenarions.</span></span> <span data-ttu-id="f604c-248">Pode haver mais tipos de notificações de ciclo de vida no futuro.</span><span class="sxs-lookup"><span data-stu-id="f604c-248">There might be more types of lifecycle notifications in the future.</span></span>

3. <span data-ttu-id="f604c-249">Em seu aplicativo ignore todos os eventos de ciclo de vida que o aplicativo não reconhece e registre-os para obter conhecimento.</span><span class="sxs-lookup"><span data-stu-id="f604c-249">In your app, ignore any lifecycle notification that the app does not recognize, and log them to gain awareness.</span></span>

4. <span data-ttu-id="f604c-250">Se desejar, procure a documentação relacionada às novas notificações de ciclo de vida e implemente o suporte para elas conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="f604c-250">At your discretion, look up the related documentation for new lifecycle notifications and implement support for them as appropriate.</span></span>

## <a name="see-also"></a><span data-ttu-id="f604c-251">Confira também</span><span class="sxs-lookup"><span data-stu-id="f604c-251">See also</span></span>

- [<span data-ttu-id="f604c-252">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="f604c-252">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="f604c-253">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="f604c-253">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="f604c-254">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="f604c-254">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="f604c-255">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="f604c-255">Delete subscription</span></span>](/graph/api/subscription-delete?view=graph-rest-1.0)
- [<span data-ttu-id="f604c-256">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="f604c-256">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
