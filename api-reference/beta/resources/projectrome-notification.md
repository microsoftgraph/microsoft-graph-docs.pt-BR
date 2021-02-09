---
title: tipo de recurso de notificação
description: 'Representa uma notificação publicada por um servidor de aplicativos destinado a um usuário especificado. A notificação é armazenada no Microsoft Graph e distribuída para pontos de extremidade de dispositivo diferentes pertencentes ao usuário. '
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: abd17119e80e4e8a7967197356811ee519d813ba
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159448"
---
# <a name="notification-resource-type"></a><span data-ttu-id="9be5b-104">tipo de recurso de notificação</span><span class="sxs-lookup"><span data-stu-id="9be5b-104">notification resource type</span></span>

<span data-ttu-id="9be5b-105">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="9be5b-105">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="9be5b-106">Representa uma notificação publicada por um servidor de aplicativos destinado a um usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="9be5b-106">Represents a notification that is published by an app server that targets a specified user.</span></span> <span data-ttu-id="9be5b-107">A notificação é armazenada no Microsoft Graph e distribuída para pontos de extremidade de dispositivo diferentes pertencentes ao usuário.</span><span class="sxs-lookup"><span data-stu-id="9be5b-107">The notification is stored in Microsoft Graph and is distributed to different device endpoints owned by the user.</span></span> 

<span data-ttu-id="9be5b-108">Uma notificação pode ser uma carga de notificação visual que pode ser interpretada pelo sistema operacional (plataformas Windows, Android e iOS).</span><span class="sxs-lookup"><span data-stu-id="9be5b-108">A notification can be a visual notification payload that can be interpreted by the operating system (Windows, Android, and iOS platforms).</span></span> <span data-ttu-id="9be5b-109">Também pode ser uma carga de dados (rawContent) entregue e manipulada por clientes de aplicativo (incluindo a Web), que determina a experiência do usuário correspondente em cada dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9be5b-109">It can also be a data payload (rawContent) that's delivered to and handled by app clients (including web), which then determine the corresponding user experience on each device.</span></span>  <span data-ttu-id="9be5b-110">Isso geralmente é uma interface do usuário de notificação visual, gerada localmente, que corresponde ao conteúdo na carga de dados original.</span><span class="sxs-lookup"><span data-stu-id="9be5b-110">This is usually a visual notification UI, generated locally, that corresponds to the content in the original data payload.</span></span> 

<span data-ttu-id="9be5b-111">Quando um usuário atua em uma notificação visual, o cliente do aplicativo pode então usar o SDK de notificações do lado do cliente para atualizar o estado do feed de notificação correspondente no Microsoft Graph, por exemplo, marcando uma notificação como descartada.</span><span class="sxs-lookup"><span data-stu-id="9be5b-111">When a user acts on a visual notification, the app client can then use the client-side notifications SDK to update the state of the corresponding notification feed in Microsoft Graph - for example, by marking a notification as dismissed.</span></span> <span data-ttu-id="9be5b-112">A atualização será então distribuída a todos os outros pontos de extremidade do cliente do aplicativo, e os clientes lidarão com a alteração de acordo, por exemplo, descartando a notificação para impedir que o usuário veja informações redundantes.</span><span class="sxs-lookup"><span data-stu-id="9be5b-112">The update will then be distributed to all other app client endpoints, and the clients handle the change accordingly, for example by dismissing the notification to prevent the user from seeing redundant information.</span></span> <span data-ttu-id="9be5b-113">Os clientes do aplicativo podem acessar o mesmo recurso de notificação posteriormente antes de expirar (mesmo depois de ser marcado como ignorado), como histórico de notificações, por meio do [SDK de notificação.](https://aka.ms/GNSDK)</span><span class="sxs-lookup"><span data-stu-id="9be5b-113">App clients can access the same notification resource at a later time before it expires (even after it is marked as dismissed), as notification history, via the [notification SDK](https://aka.ms/GNSDK).</span></span> 

> [!NOTE]
> <span data-ttu-id="9be5b-114">As atualizações de estado de notificação, como lidas ou descartadas, não serão fan-out para pontos de extremidade da Web.</span><span class="sxs-lookup"><span data-stu-id="9be5b-114">Notification state updates, such as read or dismissed, will not be fanned out to web endpoints.</span></span> <span data-ttu-id="9be5b-115">Isso porque os pushs da Web em vários navegadores exigem que as notificações do sistema visual sejam exibidas para um usuário.</span><span class="sxs-lookup"><span data-stu-id="9be5b-115">This is because web pushes across various browsers require visual toast notifications to be displayed to a user.</span></span> <span data-ttu-id="9be5b-116">Como as alterações de estado não têm conteúdo visual correspondente, elas só terão fan-out para notificações para as plataformas Windows, iOS ou Android.</span><span class="sxs-lookup"><span data-stu-id="9be5b-116">Because state changes have no corresponding visual content, they will only be fanned-out for notifications targeting Windows, iOS, or Android platforms.</span></span>

## <a name="methods"></a><span data-ttu-id="9be5b-117">Métodos</span><span class="sxs-lookup"><span data-stu-id="9be5b-117">Methods</span></span>
|<span data-ttu-id="9be5b-118">Método</span><span class="sxs-lookup"><span data-stu-id="9be5b-118">Method</span></span> | <span data-ttu-id="9be5b-119">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9be5b-119">Return Type</span></span> | <span data-ttu-id="9be5b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9be5b-120">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="9be5b-121">Criar notificação</span><span class="sxs-lookup"><span data-stu-id="9be5b-121">Create notification</span></span>](../api/user-post-notifications.md) | [<span data-ttu-id="9be5b-122">notificação</span><span class="sxs-lookup"><span data-stu-id="9be5b-122">notification</span></span>](projectrome-notification.md) |<span data-ttu-id="9be5b-123">Crie e envie uma notificação.</span><span class="sxs-lookup"><span data-stu-id="9be5b-123">Create and send a notification.</span></span> |

## <a name="properties"></a><span data-ttu-id="9be5b-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9be5b-124">Properties</span></span>
|<span data-ttu-id="9be5b-125">Nome</span><span class="sxs-lookup"><span data-stu-id="9be5b-125">Name</span></span> | <span data-ttu-id="9be5b-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="9be5b-126">Type</span></span> | <span data-ttu-id="9be5b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="9be5b-127">Description</span></span>|
|:----|:-----|:-----------|
| <span data-ttu-id="9be5b-128">targetHostName</span><span class="sxs-lookup"><span data-stu-id="9be5b-128">targetHostName</span></span> | <span data-ttu-id="9be5b-129">String</span><span class="sxs-lookup"><span data-stu-id="9be5b-129">String</span></span> | <span data-ttu-id="9be5b-130">Representa o nome de host do aplicativo para o qual o serviço de chamada deseja postar a notificação para o usuário determinado.</span><span class="sxs-lookup"><span data-stu-id="9be5b-130">Represents the host name of the app to which the calling service wants to post the notification, for the given user.</span></span> <span data-ttu-id="9be5b-131">Se estiver direcionando pontos de extremidade da Web (consulte **targetPolicy.platformTypes**), verifique se **targetHostName** é o mesmo nome usado ao criar uma assinatura no lado do cliente dentro da propriedade JSON do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9be5b-131">If targeting web endpoints (see **targetPolicy.platformTypes**), ensure that **targetHostName** is the same as the name used when creating a subscription on the client side within the application JSON property.</span></span> |
| <span data-ttu-id="9be5b-132">appNotificationId</span><span class="sxs-lookup"><span data-stu-id="9be5b-132">appNotificationId</span></span> | <span data-ttu-id="9be5b-133">String</span><span class="sxs-lookup"><span data-stu-id="9be5b-133">String</span></span> | <span data-ttu-id="9be5b-134">A ID exclusiva definida pelo servidor de aplicativo de uma notificação que é usada para identificar e direcionar uma notificação individual.</span><span class="sxs-lookup"><span data-stu-id="9be5b-134">The unique ID set by the app server of a notification that is used to identify and target an individual notification.</span></span> |
| <span data-ttu-id="9be5b-135">groupName</span><span class="sxs-lookup"><span data-stu-id="9be5b-135">groupName</span></span> | <span data-ttu-id="9be5b-136">String</span><span class="sxs-lookup"><span data-stu-id="9be5b-136">String</span></span> | <span data-ttu-id="9be5b-137">O nome do grupo ao que essa notificação pertence.</span><span class="sxs-lookup"><span data-stu-id="9be5b-137">The name of the group that this notification belongs to.</span></span> <span data-ttu-id="9be5b-138">Ele é definido pelo desenvolvedor para agrupar as notificações.</span><span class="sxs-lookup"><span data-stu-id="9be5b-138">It is set by the developer for the purpose of grouping notifications together.</span></span> |
| <span data-ttu-id="9be5b-139">targetPolicy</span><span class="sxs-lookup"><span data-stu-id="9be5b-139">targetPolicy</span></span> | [<span data-ttu-id="9be5b-140">targetPolicyEndpoints</span><span class="sxs-lookup"><span data-stu-id="9be5b-140">targetPolicyEndpoints</span></span>](targetpolicyendpoints.md) | <span data-ttu-id="9be5b-141">O objeto de política de destino lida com a política de entrega de notificação para tipos de ponto de extremidade que devem ser direcionados (Windows, iOS, Android e WebPush) para o usuário específico.</span><span class="sxs-lookup"><span data-stu-id="9be5b-141">Target policy object handles notification delivery policy for endpoint types that should be targeted (Windows, iOS, Android and WebPush) for the given user.</span></span> |
| <span data-ttu-id="9be5b-142">payload</span><span class="sxs-lookup"><span data-stu-id="9be5b-142">payload</span></span> | [<span data-ttu-id="9be5b-143">payloadTypes</span><span class="sxs-lookup"><span data-stu-id="9be5b-143">payloadTypes</span></span>](payloadtypes.md)| <span data-ttu-id="9be5b-144">Esse é o conteúdo de dados de uma notificação bruta ou visual do usuário que será entregue e consumida pelo cliente de aplicativo que recebe essa notificação.</span><span class="sxs-lookup"><span data-stu-id="9be5b-144">This is the data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> |
| <span data-ttu-id="9be5b-145">displayTimeToLive</span><span class="sxs-lookup"><span data-stu-id="9be5b-145">displayTimeToLive</span></span> | <span data-ttu-id="9be5b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9be5b-146">Int32</span></span> | <span data-ttu-id="9be5b-147">Define por quanto tempo (em segundos) esse conteúdo de notificação ficará no visualizador de notificações de cada plataforma.</span><span class="sxs-lookup"><span data-stu-id="9be5b-147">Sets how long (in seconds) this notification content will stay in each platform’s notification viewer.</span></span> <span data-ttu-id="9be5b-148">Por exemplo, quando a notificação é entregue a um dispositivo Windows, o valor dessa propriedade é passado para ToastNotification.ExpirationTime, que determina por quanto tempo a notificação do sistema ficará na Central de Ações do Windows do usuário.</span><span class="sxs-lookup"><span data-stu-id="9be5b-148">For example, when the notification is delivered to a Windows device, the value of this property is passed on to ToastNotification.ExpirationTime, which determines how long the toast notification will stay in the user’s Windows Action Center.</span></span> |
| <span data-ttu-id="9be5b-149">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9be5b-149">expirationDateTime</span></span> | <span data-ttu-id="9be5b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9be5b-150">DateTimeOffset</span></span> | <span data-ttu-id="9be5b-151">Define uma data e hora de expiração UTC em uma notificação do usuário usando o formato ISO 8601 (por exemplo, meia-noite em UTC no dia 1º de janeiro de 2019 teria esta aparência: `'2019-01-01T00:00:00Z'` ).</span><span class="sxs-lookup"><span data-stu-id="9be5b-151">Sets a UTC expiration date and time on a user notification using ISO 8601 format (for example, midnight UTC on Jan 1, 2019 would look like this: `'2019-01-01T00:00:00Z'`).</span></span> <span data-ttu-id="9be5b-152">Quando o tempo acaba, a notificação é removida do armazenamento de feeds de notificação do Microsoft Graph completamente e não faz mais parte do histórico de notificações.</span><span class="sxs-lookup"><span data-stu-id="9be5b-152">When time is up, the notification is removed from the Microsoft Graph notification feed store completely and is no longer part of notification history.</span></span> <span data-ttu-id="9be5b-153">O valor máximo é de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="9be5b-153">Max value is 30 days.</span></span> |
| <span data-ttu-id="9be5b-154">prioridade</span><span class="sxs-lookup"><span data-stu-id="9be5b-154">priority</span></span> | <span data-ttu-id="9be5b-155">string</span><span class="sxs-lookup"><span data-stu-id="9be5b-155">string</span></span> | <span data-ttu-id="9be5b-156">Indica a prioridade de uma notificação de usuário bruta.</span><span class="sxs-lookup"><span data-stu-id="9be5b-156">Indicates the priority of a raw user notification.</span></span> <span data-ttu-id="9be5b-157">As notificações visuais são enviadas com alta prioridade por padrão.</span><span class="sxs-lookup"><span data-stu-id="9be5b-157">Visual notifications are sent with high priority by default.</span></span> <span data-ttu-id="9be5b-158">Os valores válidos são `None`, `High` e `Low`.</span><span class="sxs-lookup"><span data-stu-id="9be5b-158">Valid values are `None`, `High` and `Low`.</span></span> |
| <span data-ttu-id="9be5b-159">fallbackPolicy</span><span class="sxs-lookup"><span data-stu-id="9be5b-159">fallbackPolicy</span></span> | [<span data-ttu-id="9be5b-160">fallbackpolicy</span><span class="sxs-lookup"><span data-stu-id="9be5b-160">fallbackpolicy</span></span>](fallbackpolicy.md) | <span data-ttu-id="9be5b-161">O objeto de política de fallback opcional lida com a política de fallback de notificação somente para pontos de extremidade do iOS e foi projetado para ser usado para notificações brutas de alta prioridade que podem não ser entregues a dispositivos devido a restrições específicas da plataforma (por exemplo, modo de economia de bateria).</span><span class="sxs-lookup"><span data-stu-id="9be5b-161">Optional fallback policy object handles notification fallback policy for iOS endpoints only and is designed to be used for high-priority raw notifications that might not be delivered to devices due to platform specific restrictions (e.g. battery saver mode).</span></span> |


## <a name="relationships"></a><span data-ttu-id="9be5b-162">Relações</span><span class="sxs-lookup"><span data-stu-id="9be5b-162">Relationships</span></span>
<span data-ttu-id="9be5b-163">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9be5b-163">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9be5b-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9be5b-164">JSON representation</span></span>
<span data-ttu-id="9be5b-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9be5b-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notification",
  "keyProperty": "id"
}-->

```json
{
  "targetHostName": "String",
  "appNotificationid": "String (identifier)",
  "groupName": "String", 
  "targetPolicy": {"@odata.type": "microsoft.graph.targetPolicyEndpoints"},
  "payload": {"@odata.type": "microsoft.graph.payloadTypes"},
  "displayTimeToLive": 1024,
  "expirationDateTime": "String (timestamp)",
  "priority": "string",
  "fallbackPolicy": {"@odata.type": "microsoft.graph.fallbackpolicy"},  
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


