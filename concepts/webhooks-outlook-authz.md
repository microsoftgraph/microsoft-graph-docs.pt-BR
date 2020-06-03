---
title: Reduzir assinaturas ausentes e alterar as notificações de recursos do Outlook (versão prévia)
description: O Outlook pode suspender a entrega de notificações de alteração devido a eventos de segurança como a redefinição de senha do usuário. Eventos de ciclo de vida especiais – `subscriptionRemoved` e `missed` precisam ser tratados para garantir a entrega ininterrupta de notificações de alteração.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 8b2174ea14dd7e3d6af7f0b4a447c4e5afa6fce1
ms.sourcegitcommit: 4fa554d92a684d7720db1bd96befb9dea8d6ba5f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/30/2020
ms.locfileid: "44429625"
---
# <a name="reduce-missing-subscriptions-and-change-notifications-for-outlook-resources-preview"></a><span data-ttu-id="4b5f2-104">Reduzir assinaturas ausentes e alterar as notificações de recursos do Outlook (versão prévia)</span><span class="sxs-lookup"><span data-stu-id="4b5f2-104">Reduce missing subscriptions and change notifications for Outlook resources (preview)</span></span> 

<span data-ttu-id="4b5f2-105">Os aplicativos que se inscrevem nas notificações de alteração dos recursos do Outlook podem receber suas assinaturas removidas e perder algumas notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-105">Apps subscribing to change notifications for Outlook resources might get their subscriptions removed and miss some change notifications.</span></span> <span data-ttu-id="4b5f2-106">Os aplicativos devem implementar a lógica para detectar e recuperar da perda e retomar o fluxo de notificação de alteração contínua.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-106">Apps should implement logic to detect and recover from the loss, and resume a continuous change notification flow.</span></span>

<span data-ttu-id="4b5f2-107">Determinados eventos no Outlook podem fazer que a assinatura seja removida.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-107">Certain events in Outlook can cause a subscription to be removed.</span></span> <span data-ttu-id="4b5f2-108">Esses eventos incluem:</span><span class="sxs-lookup"><span data-stu-id="4b5f2-108">These events include:</span></span>

- <span data-ttu-id="4b5f2-109">A senha do usuário foi redefinida</span><span class="sxs-lookup"><span data-stu-id="4b5f2-109">User's password has been reset</span></span>
- <span data-ttu-id="4b5f2-110">Dispositivo do usuário está fora de conformidade</span><span class="sxs-lookup"><span data-stu-id="4b5f2-110">User's device is out of compliance</span></span>
-   <span data-ttu-id="4b5f2-111">Conta do usuário foi revogada</span><span class="sxs-lookup"><span data-stu-id="4b5f2-111">User's account has been revoked</span></span>

<span data-ttu-id="4b5f2-112">Quando ocorre um evento, o Outlook envia uma notificação de ciclo de vida especial `subscriptionRemoved`.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-112">When such an event happens, Outlook sends a special lifecycle notification, `subscriptionRemoved`.</span></span>

<span data-ttu-id="4b5f2-113">O Outlook também enviará outra notificação do ciclo de vida, `missed` caso uma notificação de alteração não possa ser entregue a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-113">Outlook also sends another lifecycle notification, `missed`, if a change notification cannot be delivered to an app.</span></span>

<span data-ttu-id="4b5f2-114">Um aplicativo inscrever-se em notificações de alteração para recursos do Outlook, como **mensagem** e **evento**, deve escutar os `subscriptionRemoved` sinais e `missed` fazer o seguinte:</span><span class="sxs-lookup"><span data-stu-id="4b5f2-114">An app subscribing to change notifications for Outlook resources, such as **message** and **event**, should listen to the `subscriptionRemoved` and `missed` signals and do the following:</span></span>

- <span data-ttu-id="4b5f2-115">Após receber uma `subscriptionRemoved` notificação de ciclo de vida, o aplicativo deve recriar a inscrição para manter um fluxo contínuo.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-115">Upon receiving a `subscriptionRemoved` lifecycle notification, the app should recreate the subscription in order to maintain a continuous flow.</span></span>
- <span data-ttu-id="4b5f2-116">Ao receber uma `missed` notificação de ciclo de vida, o aplicativo deve sincronizar novamente os dados de recursos usando o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-116">On receiving a `missed` lifecycle notification, the app should resynchronize resource data using Microsoft Graph.</span></span>

<span data-ttu-id="4b5f2-117">Para receber notificações do ciclo de vida, você pode usar o ponto de extremidade do **notificationUrl** existente que já recebe notificações de alteração ou pode registrar um **lifecycleNotificationUrl** separado para receber `subscriptionRemoved` e `missed` notificar as notificações de ciclo de vida em um ponto de extremidade separado.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-117">To receive lifecycle notifications, you can use the existing **notificationUrl** endpoint that already receives change notifications, or you can register a separate **lifecycleNotificationUrl** to receive `subscriptionRemoved` and `missed` lifecycle notifications in a separate endpoint.</span></span>

## <a name="creating-a-subscription"></a><span data-ttu-id="4b5f2-118">Criar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="4b5f2-118">Creating a subscription</span></span>

<span data-ttu-id="4b5f2-119">Ao criar uma assinatura, você pode especificar um ponto de extremidade separado usando a propriedade **lifecycleNotificationUrl** .</span><span class="sxs-lookup"><span data-stu-id="4b5f2-119">When creating a subscription, you can specify a separate endpoint using the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="4b5f2-120">Se você especificar o ponto de extremidade, todos os tipos de atuais e futuros de notificações de ciclo de vida serão entregues lá.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-120">If you specify the endpoint, all current and future types of lifecycle notifications will be delivered there.</span></span> <span data-ttu-id="4b5f2-121">Caso contrário, `subscriptionRemoved` e `missed` as notificações de ciclo de vida serão entregues ao **notificationUrl** existente para todas as assinaturas existentes.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-121">Otherwise, `subscriptionRemoved` and `missed` lifecycle notifications will be delivered to the existing **notificationUrl** for all existing subscriptions.</span></span>

> <span data-ttu-id="4b5f2-122">**Observação:** a propriedade **lifecycleNotificationUrl** só pode ser definida ou lida usando as APIs beta do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-122">**Note:** The **lifecycleNotificationUrl** property can only be set or read using Microsoft Graph beta APIs.</span></span> <span data-ttu-id="4b5f2-123">No entanto, as assinaturas criadas usando as APIs beta são armazenadas no mesmo ambiente de produção que as assinaturas criadas usando v1.0, para que você possa implementar o novo fluxo do Outlook, além de suas assinaturas, usando APIs v1.0.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-123">However, subscriptions created using beta APIs are stored in the same production environment as those created using v1.0, so you can implement the new Outlook flow in addition to your subscriptions creating using v1.0 APIs.</span></span>

> <span data-ttu-id="4b5f2-124">As assinaturas criadas por meio das APIs do v 1.0 receberão notificações do ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-124">Subscriptions created via the v1.0 APIs will receive lifecycle notifications.</span></span> 

### <a name="subscription-request-example"></a><span data-ttu-id="4b5f2-125">Exemplo de solicitação de assinatura</span><span class="sxs-lookup"><span data-stu-id="4b5f2-125">Subscription request example</span></span>

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
 
> <span data-ttu-id="4b5f2-126">**Importante:** Use o mesmo nome de host para ambas as notificações URLs.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-126">**Important:** Use the same hostname for both notifications URLs.</span></span> 

> <span data-ttu-id="4b5f2-127">**Observação:** Você precisa validar os dois pontos de extremidade, conforme descrito em [Managing subscriptions](webhooks.md#managing-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="4b5f2-127">**Note:** You need to validate both endpoints as described in [Managing subscriptions](webhooks.md#managing-subscriptions).</span></span>
<span data-ttu-id="4b5f2-128">Se você quiser usar a mesma URL para os dois pontos de extremidade você receberá e responderá a duas solicitações de validação.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-128">If you choose to use the same URL for both endpoints you will receive and respond to two validation requests.</span></span>

> <span data-ttu-id="4b5f2-129">**Observação:** Não é possível atualizar (`PATCH`) as assinaturas existentes para adicionar a propriedade **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-129">**Note:** You cannot update (`PATCH`) the existing subscriptions to add the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="4b5f2-130">Você deve remover essas assinaturas existentes, criar novas assinaturas e especificar a propriedade **lifecycleNotificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-130">You should remove such existing subscriptions, and create new subscriptions and specify the **lifecycleNotificationUrl** property.</span></span> <span data-ttu-id="4b5f2-131">As assinaturas existentes sem a propriedade **lifecycleNotificationUrl** receberão as `subscriptionRemoved` notificações de ciclo de `missed` vida e por meio do **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-131">Existing subscriptions without **lifecycleNotificationUrl** property will receive the `subscriptionRemoved` and `missed` lifecycle notifications via the **notificationUrl**.</span></span> 

## <a name="responding-to-subscriptionremoved-notifications"></a><span data-ttu-id="4b5f2-132">Responder a notificações subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="4b5f2-132">Responding to subscriptionRemoved notifications</span></span>

<span data-ttu-id="4b5f2-133">A `subscriptionRemoved` notificação de ciclo de vida informa que uma assinatura foi removida e deve ser recriada, se você quiser continuar recebendo notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-133">The `subscriptionRemoved` lifecycle notification informs you that a subscription has been removed and should be recreated, if you want to continue receiving change notifications.</span></span> 

<span data-ttu-id="4b5f2-134">Você pode criar uma assinatura de longa vida (3 dias) e as notificações de alteração começarão a fluir para o **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-134">You can create a long-lived subscription (3 days), and change notifications will start flowing to the **notificationUrl**.</span></span> <span data-ttu-id="4b5f2-135">No entanto, as condições de acesso aos dados de recursos podem mudar ao longo do tempo.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-135">However, the conditions of access to the resource data might change over time.</span></span> <span data-ttu-id="4b5f2-136">Por exemplo, pode ocorrer um evento no serviço do Outlook que requeira que o aplicativo para que o usuário seja autenticado novamente.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-136">For example, an event in the Outlook service might occur that requires the app to re-authenticate the user.</span></span> <span data-ttu-id="4b5f2-137">Nesse caso, o fluxo é:</span><span class="sxs-lookup"><span data-stu-id="4b5f2-137">In such a case, the flow is as follows:</span></span>

1. <span data-ttu-id="4b5f2-138">Outlook detecta que uma assinatura precisa ser removido do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-138">Outlook detects that a subscription needs to be removed from Microsoft Graph.</span></span>
    
    <span data-ttu-id="4b5f2-139">Não há cadência definida para esses eventos.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-139">There is no set cadence for these events.</span></span> <span data-ttu-id="4b5f2-140">Eles podem ocorrer com frequência para alguns recursos e quase nunca para outros.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-140">They might occur frequently for some resources, and almost never for others.</span></span>

2. <span data-ttu-id="4b5f2-141">O Microsoft Graph envia uma `subscriptionRemoved` notificação de ciclo de vida para o **lifecycleNotificationUrl** (se especificado) ou para o **notificationUrl**.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-141">Microsoft Graph sends a `subscriptionRemoved` lifecycle notification to the **lifecycleNotificationUrl** (if specified), or the **notificationUrl**.</span></span>  

3. <span data-ttu-id="4b5f2-142">Você pode responder a essa notificação de ciclo de vida criando uma nova assinatura para o mesmo recurso.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-142">You can respond to this lifecycle notification by creating a new subscription for the same resource.</span></span> <span data-ttu-id="4b5f2-143">Para fazer isso, é necessário apresentar um token de acesso válido; em alguns casos, isso significa que o aplicativo precisa reautenticar o usuário para obter um novo token de acesso válido.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-143">To do this, you need to present a valid access token; in some cases this means the app needs to re-authenticate the user to obtain a new valid access token.</span></span>

4. <span data-ttu-id="4b5f2-144">Se você criar uma nova assinatura com êxito, as notificações de alteração começarão a fluir novamente.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-144">If you successfully create a new subscription, change notifications will start flowing again.</span></span> <span data-ttu-id="4b5f2-145">No entanto, se você falhar (por exemplo, o aplicativo não pode obter um token de acesso válido), as notificações de alteração não serão enviadas.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-145">However, if you fail (for example, the app can't obtain a valid access token), change notifications will not be sent.</span></span>

5. <span data-ttu-id="4b5f2-146">Depois de criar uma nova assinatura, você pode sincronizar os dados de recursos para identificar alterações ausentes.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-146">After creating the new subscription, you can sync the resource data to identify any missing changes.</span></span>

### <a name="subscriptionremoved-notification-example"></a><span data-ttu-id="4b5f2-147">exemplo de notificação subscriptionRemoved</span><span class="sxs-lookup"><span data-stu-id="4b5f2-147">subscriptionRemoved notification example</span></span>

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

<span data-ttu-id="4b5f2-148">Alguns aspectos a serem observados neste tipo de notificação:</span><span class="sxs-lookup"><span data-stu-id="4b5f2-148">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="4b5f2-149">O `"lifecycleEvent": "subscriptionRemoved"` campo designa essa notificação como relacionada à remoção de assinatura.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-149">The `"lifecycleEvent": "subscriptionRemoved"` field designates this notification as related to subscription removal.</span></span> <span data-ttu-id="4b5f2-150">Outros tipos de notificações de ciclo de vida também são possíveis, e novos serão disponibilizados no futuro.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-150">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="4b5f2-151">A notificação de ciclo de vida não contém informações sobre um recurso específico, pois ela não está relacionada a uma alteração de recurso, mas à alteração de estado de assinatura.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-151">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="4b5f2-152">Semelhante às notificações de alteração, as notificações de ciclo de vida podem ser encadeados juntas (na matriz de **valor** ), cada uma com um valor possivelmente diferente de **lifecycleEvent** .</span><span class="sxs-lookup"><span data-stu-id="4b5f2-152">Similar to change notifications, lifecycle notifications can be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="4b5f2-153">Processe a cada notificação de ciclo de vida no lote.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-153">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="4b5f2-154">**Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração são entregues, consulte [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="4b5f2-154">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="4b5f2-155">Ações a serem executadas</span><span class="sxs-lookup"><span data-stu-id="4b5f2-155">Actions to take</span></span>

1. <span data-ttu-id="4b5f2-156">[Confirme](webhooks.md#change-notifications) o recebimento da notificação de ciclo de vida, respondendo à chamada post com `202 - Accepted` .</span><span class="sxs-lookup"><span data-stu-id="4b5f2-156">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
2. <span data-ttu-id="4b5f2-157">[Validar](webhooks.md#change-notifications) a autenticidade da notificação de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-157">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="4b5f2-158">Certifique-se de que o aplicativo tenha um token de acesso válido para a próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-158">Ensure that the app has a valid access token to take the next step.</span></span> 
  > <span data-ttu-id="4b5f2-159">**Observação**: se você estiver usando uma das [bibliotecas de autenticação](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), elas farão isso para você ao reutilizar um token de cache válido ou obtendo um novo token, inclusive pedindo ao usuário para fazer logon novamente (com uma nova senha).</span><span class="sxs-lookup"><span data-stu-id="4b5f2-159">**Note:** If you're using one of the [authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), they will handle this for you by either reusing a valid cached token, or obtaining a new token, including asking the user to sign in again (with a new password).</span></span> <span data-ttu-id="4b5f2-160">Observe que a obtenção de um novo token pode falhar, pois as condições de acesso podem ser alteradas e o chamador não poderá mais acessar os dados de recursos. </span><span class="sxs-lookup"><span data-stu-id="4b5f2-160">Note that obtaining a new token might fail, because the conditions of access might have changed, and the caller might no longer be allowed access to the resource data.</span></span>

4. <span data-ttu-id="4b5f2-161">Criar uma nova assinatura usando o processo padrão descrito [aqui](webhooks.md#subscription-request-example).</span><span class="sxs-lookup"><span data-stu-id="4b5f2-161">Create a new subscription using the standard process described [here](webhooks.md#subscription-request-example).</span></span>

  > <span data-ttu-id="4b5f2-162">**Observação:** essa ação pode falhar, porque as verificações de autorização realizadas pelo sistema podem recusar o aplicativo ou o acesso do usuário ao recurso.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-162">**Note:** This action might fail, because the authorization checks performed by the system might deny the app or the user access to the resource.</span></span> <span data-ttu-id="4b5f2-163">Pode ser necessário que o aplicativo obtenha um novo token de acesso do usuário para reautorizar uma assinatura com êxito.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-163">It might be necessary for the app to obtain a new access token from the user to successfully reauthorize a subscription.</span></span> <span data-ttu-id="4b5f2-164">Você pode tentar essa ações mais tarde, a qualquer momento; por exemplo, quando as condições de acesso mudarem.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-164">You can retry these actions later, at any time; for example, when the conditions of access have changed.</span></span> <span data-ttu-id="4b5f2-165">Qualquer alteração de recurso no período de tempo a partir da qual a notificação de ciclo de vida foi enviada, quando o aplicativo recriar a assinatura com êxito, será perdido.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-165">Any resource changes in the time period from when the lifecycle notification was sent, to when the app recreates the subscription successfully, will be lost.</span></span> <span data-ttu-id="4b5f2-166">O aplicativo precisará buscar essas alterações sozinho.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-166">The app will need to fetch those changes on its own.</span></span>

5. <span data-ttu-id="4b5f2-167">Após criar a nova assinatura, sincronize quaisquer dados de recurso ausentes do último tempo conhecido em que você recebeu uma notificação de alteração para este recurso; por exemplo:`GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span><span class="sxs-lookup"><span data-stu-id="4b5f2-167">After creating the new subscription, sync any missing resource data from the last known time you received a change notification for this resource; for example: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`</span></span>

## <a name="responding-to-missed-notifications"></a><span data-ttu-id="4b5f2-168">Responder notificações perdidas</span><span class="sxs-lookup"><span data-stu-id="4b5f2-168">Responding to missed notifications</span></span>

<span data-ttu-id="4b5f2-169">Esses sinais informam que algumas notificações de alteração podem não ter sido entregues.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-169">These signals inform you that some change notifications might not have been delivered.</span></span> <span data-ttu-id="4b5f2-170">Você deve ignorar ou lidar com esses sinais são.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-170">You should decide if you ignore or handle these signals.</span></span>

### <a name="notification-example"></a><span data-ttu-id="4b5f2-171">Exemplo de notificação</span><span class="sxs-lookup"><span data-stu-id="4b5f2-171">Notification example</span></span>

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

<span data-ttu-id="4b5f2-172">Alguns aspectos a serem observados neste tipo de notificação:</span><span class="sxs-lookup"><span data-stu-id="4b5f2-172">A few things to note about this type of notification:</span></span>
- <span data-ttu-id="4b5f2-173">O `"lifecycleEvent": "missed"` campo designa isso como um sinal sobre notificações de alteração perdidas.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-173">The `"lifecycleEvent": "missed"` field designates this as a signal about missed change notifications.</span></span> <span data-ttu-id="4b5f2-174">Outros tipos de notificações de ciclo de vida também são possíveis, e novos serão disponibilizados no futuro.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-174">Other types of lifecycle notifications are also possible, and new ones will be introduced in the future.</span></span>
- <span data-ttu-id="4b5f2-175">A notificação de ciclo de vida não contém informações sobre um recurso específico, pois ela não está relacionada a uma alteração de recurso, mas à alteração de estado de assinatura.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-175">The lifecycle notification does not contain any information about a specific resource, because it is not related to a resource change, but to the subscription state change.</span></span>
- <span data-ttu-id="4b5f2-176">Semelhante às notificações de alteração, as notificações de ciclo de vida podem ser encadeados juntas (na matriz de **valor** ), cada uma com um valor possivelmente diferente de **lifecycleEvent** .</span><span class="sxs-lookup"><span data-stu-id="4b5f2-176">Similar to change notifications, lifecycle notifications might be batched together (in the **value** array), each with a possibly different **lifecycleEvent** value.</span></span> <span data-ttu-id="4b5f2-177">Processe a cada notificação de ciclo de vida no lote.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-177">Process each lifecycle notification in the batch accordingly.</span></span>

> <span data-ttu-id="4b5f2-178">**Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração são entregues, consulte [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span><span class="sxs-lookup"><span data-stu-id="4b5f2-178">**Note:** for a full description of the data sent when change notifications are delivered, see [changeNotificationCollection](/graph/api/resources/changenotificationcollection).</span></span>

### <a name="actions-to-take"></a><span data-ttu-id="4b5f2-179">Ações a serem executadas</span><span class="sxs-lookup"><span data-stu-id="4b5f2-179">Actions to take</span></span>

1. <span data-ttu-id="4b5f2-180">[Confirme](webhooks.md#change-notifications) o recebimento da notificação de ciclo de vida, respondendo à chamada post com `202 - Accepted` .</span><span class="sxs-lookup"><span data-stu-id="4b5f2-180">[Acknowledge](webhooks.md#change-notifications) the receipt of the lifecycle notification, by responding to the POST call with `202 - Accepted`.</span></span>
    - <span data-ttu-id="4b5f2-181">Caso você ignore estes sinais, não faça nada.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-181">If you ignore these signals, do nothing else.</span></span> <span data-ttu-id="4b5f2-182">Caso contrário:</span><span class="sxs-lookup"><span data-stu-id="4b5f2-182">Otherwise:</span></span>
2. <span data-ttu-id="4b5f2-183">[Validar](webhooks.md#change-notifications) a autenticidade da notificação de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-183">[Validate](webhooks.md#change-notifications) the authenticity of the lifecycle notification.</span></span>
3. <span data-ttu-id="4b5f2-184">Executaremos ressincronização de dados completa para identificar as alterações que não foram entregues como notificações.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-184">Perform a full data resync of the resource to identify the changes that were not delivered as notifications.</span></span> 


## <a name="future-proof-the-code-handling-lifecycle-notifications"></a><span data-ttu-id="4b5f2-185">À prova de futuro o código lidar com as notificações de ciclo de vida</span><span class="sxs-lookup"><span data-stu-id="4b5f2-185">Future-proof the code handling lifecycle notifications</span></span>

<span data-ttu-id="4b5f2-186">No futuro, o Microsoft Graph adicionará mais tipos de notificações de ciclo de vida de assinatura.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-186">In the future, Microsoft Graph will add more types of subscription lifecycle notifications.</span></span> <span data-ttu-id="4b5f2-187">Elas serão publicadas no mesmo ponto de extremidade: **lifecycleNotificationUrl**, mas terão um valor diferente sob **lifecycleEvent** e podem conter um esquema e propriedades ligeiramente diferentes, específicas para o cenário para o qual serão enviadas.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-187">They will be posted to the same endpoint: **lifecycleNotificationUrl**, but they will have a different value under **lifecycleEvent** and might contain a slightly different schema and properties, specific to the scenario for which they will be issued.</span></span>

<span data-ttu-id="4b5f2-188">Você deve implementar o código á prova de futuro para que não pare quando o Microsoft Graph apresentar novos tipos de notificações de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-188">You should implement your code in a future-proof way so it does not break when Microsoft Graph introduces new types of lifecycle notifications.</span></span> <span data-ttu-id="4b5f2-189">Recomendamos as seguintes abordagens:</span><span class="sxs-lookup"><span data-stu-id="4b5f2-189">We recommend the following approach:</span></span>

1. <span data-ttu-id="4b5f2-190">Identifique explicitamente cada notificação de ciclo de vida como um evento que você suporta, usando a propriedade **lifecycleEvent** .</span><span class="sxs-lookup"><span data-stu-id="4b5f2-190">Explicitly identify each lifecycle notification as an event that you support, using the **lifecycleEvent** property.</span></span> <span data-ttu-id="4b5f2-191">Por exemplo, procure a `"lifecycleEvent": "subscriptionRemoved"` propriedade para identificar um evento específico e tratá-lo.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-191">For example, look for the `"lifecycleEvent": "subscriptionRemoved"` property to identify a specific event, and handle it.</span></span>

2. <span data-ttu-id="4b5f2-192">Assista aos comunicados de notificações de ciclo de vida para o novo scenarions.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-192">Watch for announcements of lifecycle notifications for new scenarions.</span></span> <span data-ttu-id="4b5f2-193">Talvez haja mais tipos de notificações de ciclo de vida no futuro.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-193">There might be more types of lifecycle notifications in the future.</span></span>

3. <span data-ttu-id="4b5f2-194">Em seu aplicativo, ignore qualquer notificação de ciclo de vida que o aplicativo não reconhece e registre-o para obter conscientização.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-194">In your app, ignore any lifecycle notification that the app does not recognize, and log them to gain awareness.</span></span>

4. <span data-ttu-id="4b5f2-195">Se desejar, procure a documentação relacionada às novas notificações de ciclo de vida e implemente o suporte para elas conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="4b5f2-195">At your discretion, look up the related documentation for new lifecycle notifications and implement support for them as appropriate.</span></span>

## <a name="see-also"></a><span data-ttu-id="4b5f2-196">Confira também</span><span class="sxs-lookup"><span data-stu-id="4b5f2-196">See also</span></span>

- [<span data-ttu-id="4b5f2-197">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="4b5f2-197">Subscription resource type</span></span>](/graph/api/resources/subscription?view=graph-rest-1.0)
- [<span data-ttu-id="4b5f2-198">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="4b5f2-198">Get subscription</span></span>](/graph/api/subscription-get?view=graph-rest-1.0)
- [<span data-ttu-id="4b5f2-199">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="4b5f2-199">Create subscription</span></span>](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [<span data-ttu-id="4b5f2-200">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="4b5f2-200">Delete subscription</span></span>](/graph/api/subscription-delete?view=graph-rest-1.0)
- [<span data-ttu-id="4b5f2-201">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="4b5f2-201">Update subscription</span></span>](/graph/api/subscription-update?view=graph-rest-1.0)
