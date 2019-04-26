---
title: tipo de recurso de notificação
description: 'Representa uma notificação publicada por um servidor de aplicativos que se destina a um usuário especificado. A notificação é armazenada no Microsoft Graph e é distribuída para diferentes pontos de extremidade do dispositivo de Propriedade do usuário. '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 56a05ced6d722b3c1c347fc43735dec461aa0f69
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344080"
---
# <a name="notification-resource-type"></a><span data-ttu-id="bfba6-104">tipo de recurso de notificação</span><span class="sxs-lookup"><span data-stu-id="bfba6-104">notification resource type</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfba6-105">Representa uma notificação publicada por um servidor de aplicativos que se destina a um usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="bfba6-105">Represents a notification that is published by an app server that targets a specified user.</span></span> <span data-ttu-id="bfba6-106">A notificação é armazenada no Microsoft Graph e é distribuída para diferentes pontos de extremidade do dispositivo de Propriedade do usuário.</span><span class="sxs-lookup"><span data-stu-id="bfba6-106">The notification is stored in Microsoft Graph and is distributed to different device endpoints owned by the user.</span></span> 

<span data-ttu-id="bfba6-107">Uma notificação pode ser uma carga de notificação visual que pode ser interpretada pelo sistema operacional, incluindo plataformas Windows, Android e iOS.</span><span class="sxs-lookup"><span data-stu-id="bfba6-107">A notification can be a visual notification payload that can be interpreted by the operating system, including Windows, Android, and iOS platforms.</span></span> <span data-ttu-id="bfba6-108">Também pode ser uma carga de dados que é entregue e manipulado por clientes de aplicativos, que, em seguida, determinam a experiência do usuário correspondente em cada dispositivo – normalmente, uma interface de usuário de notificação visual que corresponde ao conteúdo da carga de dados original que é gerado localmente.</span><span class="sxs-lookup"><span data-stu-id="bfba6-108">It can also be a data payload that's delivered to and handled by app clients, which then determine the corresponding user experience on each device – usually, a visual notification UI that corresponds to the content in the original data payload that's generated locally.</span></span> 

<span data-ttu-id="bfba6-109">Quando um usuário atua em uma notificação Visual, o cliente do aplicativo pode usar o SDK de projeto do lado do cliente Roma para atualizar o estado do feed de notificação correspondente no Microsoft Graph, por exemplo, marcando uma notificação como descartada.</span><span class="sxs-lookup"><span data-stu-id="bfba6-109">When a user acts on a visual notification, the app client can then use client-side Project Rome SDK to update the state of the corresponding notification feed in Microsoft Graph - for example, by marking a notification as dismissed.</span></span> <span data-ttu-id="bfba6-110">A atualização será distribuída para todos os outros pontos de extremidade do cliente de aplicativos, e os clientes cuidam da alteração de acordo, por exemplo, descartando a notificação para impedir que o usuário veja informações redundantes.</span><span class="sxs-lookup"><span data-stu-id="bfba6-110">The update will then be distributed to all other app client endpoints, and the clients handle the change accordingly, for example by dismissing the notification to prevent the user from seeing redundant information.</span></span> <span data-ttu-id="bfba6-111">Os clientes de aplicativos podem acessar o mesmo recurso de notificação mais tarde antes de expirar (mesmo depois de ser marcado como ignorado), como histórico de notificações, por meio do [SDK do Project Roma](https://github.com/Microsoft/project-rome).</span><span class="sxs-lookup"><span data-stu-id="bfba6-111">App clients can access the same notification resource at a later time before it expires (even after it is marked as dismissed), as notification history, via the [Project Rome SDK](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="methods"></a><span data-ttu-id="bfba6-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="bfba6-112">Methods</span></span>
|<span data-ttu-id="bfba6-113">Método</span><span class="sxs-lookup"><span data-stu-id="bfba6-113">Method</span></span> | <span data-ttu-id="bfba6-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bfba6-114">Return Type</span></span> | <span data-ttu-id="bfba6-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfba6-115">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="bfba6-116">Criar notificação</span><span class="sxs-lookup"><span data-stu-id="bfba6-116">Create notification</span></span>](../api/projectrome-notification-post.md) | [<span data-ttu-id="bfba6-117">Notifica</span><span class="sxs-lookup"><span data-stu-id="bfba6-117">notification</span></span>](projectrome-notification.md) |<span data-ttu-id="bfba6-118">Criar e enviar uma notificação.</span><span class="sxs-lookup"><span data-stu-id="bfba6-118">Create and send a notification.</span></span> |

## <a name="properties"></a><span data-ttu-id="bfba6-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bfba6-119">Properties</span></span>
|<span data-ttu-id="bfba6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bfba6-120">Name</span></span> | <span data-ttu-id="bfba6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfba6-121">Type</span></span> | <span data-ttu-id="bfba6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfba6-122">Description</span></span>|
|:----|:-----|:-----------|
| <span data-ttu-id="bfba6-123">targetHostName</span><span class="sxs-lookup"><span data-stu-id="bfba6-123">targetHostName</span></span> | <span data-ttu-id="bfba6-124">String</span><span class="sxs-lookup"><span data-stu-id="bfba6-124">String</span></span> | <span data-ttu-id="bfba6-125">Representa o nome do host do aplicativo para o qual o serviço de chamada deseja postar a notificação para o usuário específico.</span><span class="sxs-lookup"><span data-stu-id="bfba6-125">Represents the host name of the app to which the calling service wants to post the notification, for the given user.</span></span> |
| <span data-ttu-id="bfba6-126">appNotificationId</span><span class="sxs-lookup"><span data-stu-id="bfba6-126">appNotificationId</span></span> | <span data-ttu-id="bfba6-127">String</span><span class="sxs-lookup"><span data-stu-id="bfba6-127">String</span></span> | <span data-ttu-id="bfba6-128">A ID exclusiva definida pelo servidor de aplicativos de uma notificação que é usada para identificar e direcionar uma notificação individual.</span><span class="sxs-lookup"><span data-stu-id="bfba6-128">The unique id set by the app server of a notification that is used to identify and target an individual notification.</span></span> |
| <span data-ttu-id="bfba6-129">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bfba6-129">expirationDateTime</span></span> | <span data-ttu-id="bfba6-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfba6-130">DateTimeOffset</span></span> | <span data-ttu-id="bfba6-131">Define um horário de expiração UTC em uma notificação de usuário-quando o tempo for ativado, a notificação será removida do repositório de feed de notificação do Microsoft Graph completamente e não faz mais parte do histórico de notificações.</span><span class="sxs-lookup"><span data-stu-id="bfba6-131">Sets a UTC expiration time on a user notification - when time is up, the notification is removed from the Microsoft Graph notification feed store completely and is no longer part of notification history.</span></span> <span data-ttu-id="bfba6-132">O valor máximo é 30 dias.</span><span class="sxs-lookup"><span data-stu-id="bfba6-132">Max value is 30 days.</span></span> |
| <span data-ttu-id="bfba6-133">payload</span><span class="sxs-lookup"><span data-stu-id="bfba6-133">payload</span></span> | <span data-ttu-id="bfba6-134">EDM. complexType, objeto JSON</span><span class="sxs-lookup"><span data-stu-id="bfba6-134">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="bfba6-135">Este é o conteúdo de dados de uma notificação de usuário bruto ou Visual que será entregue e consumido pelo cliente do aplicativo que está recebendo esta notificação.</span><span class="sxs-lookup"><span data-stu-id="bfba6-135">This is the data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> |
| <span data-ttu-id="bfba6-136">Payload. rawContent</span><span class="sxs-lookup"><span data-stu-id="bfba6-136">payload.rawContent</span></span> | <span data-ttu-id="bfba6-137">String</span><span class="sxs-lookup"><span data-stu-id="bfba6-137">String</span></span> | <span data-ttu-id="bfba6-138">O conteúdo de notificação de uma notificação de usuário bruto que será entregue e consumido pelo cliente do aplicativo que está recebendo esta notificação.</span><span class="sxs-lookup"><span data-stu-id="bfba6-138">The notification content of a raw user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> <span data-ttu-id="bfba6-139">Pelo menos um dos payloads. RawContent e Payload. VisualContent precisam ser válidos para uma solicitação de notificação POST.</span><span class="sxs-lookup"><span data-stu-id="bfba6-139">At least one of Payload.RawContent and Payload.VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="bfba6-140">Payload. Visual</span><span class="sxs-lookup"><span data-stu-id="bfba6-140">payload.visual</span></span> | <span data-ttu-id="bfba6-141">EDM. complexType, objeto JSON</span><span class="sxs-lookup"><span data-stu-id="bfba6-141">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="bfba6-142">O conteúdo visual de uma notificação de usuário visual, que será consumida pela plataforma de notificação em cada plataforma móvel e renderizada para os usuários.</span><span class="sxs-lookup"><span data-stu-id="bfba6-142">The visual content of a visual user notification, which will be consumed by the notification platform on each mobile platform and rendered for the users.</span></span> <span data-ttu-id="bfba6-143">Pelo menos um dos conteúdos e VisualContent precisa ser válido para uma solicitação de notificação POST.</span><span class="sxs-lookup"><span data-stu-id="bfba6-143">At least one of Content and VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="bfba6-144">Payload. Visual. title</span><span class="sxs-lookup"><span data-stu-id="bfba6-144">payload.visual.title</span></span> | <span data-ttu-id="bfba6-145">String</span><span class="sxs-lookup"><span data-stu-id="bfba6-145">String</span></span> | <span data-ttu-id="bfba6-146">O título de uma notificação de usuário visual.</span><span class="sxs-lookup"><span data-stu-id="bfba6-146">The title of a visual user notification.</span></span> <span data-ttu-id="bfba6-147">Deve ter título ou corpo.</span><span class="sxs-lookup"><span data-stu-id="bfba6-147">Must have either title or body.</span></span> |
| <span data-ttu-id="bfba6-148">Payload. Visual. Body</span><span class="sxs-lookup"><span data-stu-id="bfba6-148">payload.visual.body</span></span> | <span data-ttu-id="bfba6-149">String</span><span class="sxs-lookup"><span data-stu-id="bfba6-149">String</span></span> | <span data-ttu-id="bfba6-150">O corpo de uma notificação de usuário visual.</span><span class="sxs-lookup"><span data-stu-id="bfba6-150">The body of a visual user notification.</span></span> <span data-ttu-id="bfba6-151">Deve ter título ou corpo.</span><span class="sxs-lookup"><span data-stu-id="bfba6-151">Must have either title or body.</span></span> |
| <span data-ttu-id="bfba6-152">displayTimeToLive</span><span class="sxs-lookup"><span data-stu-id="bfba6-152">displayTimeToLive</span></span> | <span data-ttu-id="bfba6-153">Int</span><span class="sxs-lookup"><span data-stu-id="bfba6-153">Int</span></span> | <span data-ttu-id="bfba6-154">Define por quanto tempo (em segundos) esse conteúdo de notificação permanecerá no Visualizador de notificação de cada plataforma.</span><span class="sxs-lookup"><span data-stu-id="bfba6-154">Sets how long (in seconds) this notification content will stay in each platform’s notification viewer.</span></span> <span data-ttu-id="bfba6-155">Por exemplo, quando a notificação é entregue a um dispositivo do Windows, o valor dessa propriedade é passado para ToastNotification. ExpirationTime, que determina por quanto tempo a notificação de notificação de falha permanecerá na central de ações do Windows do usuário.</span><span class="sxs-lookup"><span data-stu-id="bfba6-155">For example, when the notification is delivered to a Windows device, the value of this property is passed on to ToastNotification.ExpirationTime, which determines how long the toast notification will stay in the user’s Windows Action Center.</span></span> |
| <span data-ttu-id="bfba6-156">prioridade</span><span class="sxs-lookup"><span data-stu-id="bfba6-156">priority</span></span> | <span data-ttu-id="bfba6-157">EnumType</span><span class="sxs-lookup"><span data-stu-id="bfba6-157">EnumType</span></span> | <span data-ttu-id="bfba6-158">Indica a prioridade de uma notificação de usuário bruto.</span><span class="sxs-lookup"><span data-stu-id="bfba6-158">Indicates the priority of a raw user notification.</span></span> <span data-ttu-id="bfba6-159">As notificações visuais são enviadas com alta prioridade por padrão.</span><span class="sxs-lookup"><span data-stu-id="bfba6-159">Visual notifications are sent with high priority by default.</span></span> <span data-ttu-id="bfba6-160">Os valores válidos são alto e baixo.</span><span class="sxs-lookup"><span data-stu-id="bfba6-160">Valid values are High and Low.</span></span> |
| <span data-ttu-id="bfba6-161">Nome_do_grupo</span><span class="sxs-lookup"><span data-stu-id="bfba6-161">groupName</span></span> | <span data-ttu-id="bfba6-162">String</span><span class="sxs-lookup"><span data-stu-id="bfba6-162">String</span></span> | <span data-ttu-id="bfba6-163">O nome do grupo ao qual essa notificação pertence.</span><span class="sxs-lookup"><span data-stu-id="bfba6-163">The name of the group that this notification belongs to.</span></span> <span data-ttu-id="bfba6-164">Ele é definido pelo desenvolvedor com o objetivo de agrupar notificações.</span><span class="sxs-lookup"><span data-stu-id="bfba6-164">It is set by the developer for the purpose of grouping notifications together.</span></span> |
| <span data-ttu-id="bfba6-165">targetPolicy</span><span class="sxs-lookup"><span data-stu-id="bfba6-165">targetPolicy</span></span> | <span data-ttu-id="bfba6-166">EDM. complexType, objeto JSON</span><span class="sxs-lookup"><span data-stu-id="bfba6-166">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="bfba6-167">O objeto de política de destino trata a política de entrega de notificação em dois níveis diferentes-tipos de ponto de extremidade (Windows, iOS e Android) que devem ser direcionados e pontos de extremidade específicos (identificados por IDs de assinatura) que devem ser direcionados.</span><span class="sxs-lookup"><span data-stu-id="bfba6-167">Target policy object handles notification delivery policy at two different levels - endpoint types (Windows, iOS and Android) that should be targeted, and specific endpoints (identified by subscription ids) that should be targeted.</span></span> |
| <span data-ttu-id="bfba6-168">targetPolicy. platformTypes</span><span class="sxs-lookup"><span data-stu-id="bfba6-168">targetPolicy.platformTypes</span></span> | <span data-ttu-id="bfba6-169">EDM. complexType, coleção (EnumType)</span><span class="sxs-lookup"><span data-stu-id="bfba6-169">Edm.ComplexType, Collection (EnumType)</span></span> | <span data-ttu-id="bfba6-170">Use para filtrar a distribuição de notificação para uma plataforma ou plataformas específicas.</span><span class="sxs-lookup"><span data-stu-id="bfba6-170">Use to filter the notification distribution to a specific platform or platforms.</span></span> <span data-ttu-id="bfba6-171">Por padrão, todos os tipos de ponto de extremidade de envio (iOS, Windows e Android) estão habilitados.</span><span class="sxs-lookup"><span data-stu-id="bfba6-171">By default, all push endpoint types (iOS, Windows, and Android) are enabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bfba6-172">Relações</span><span class="sxs-lookup"><span data-stu-id="bfba6-172">Relationships</span></span>
<span data-ttu-id="bfba6-173">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bfba6-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bfba6-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bfba6-174">JSON representation</span></span>
<span data-ttu-id="bfba6-175">Veja a seguir uma representação JSON do recurso quando você publica uma notificação Visual direta que é entregue ao sistema operacional de destino.</span><span class="sxs-lookup"><span data-stu-id="bfba6-175">The following is a JSON representation of the resource when you publish a direct visual notification that is delivered to the destination operating system.</span></span>

```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "visualContent": 
    {
      "title": "String",
      "body": "String"
    },
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```

<span data-ttu-id="bfba6-176">Veja a seguir uma representação JSON do recurso quando você publica uma notificação de dados brutos entregue a clientes de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="bfba6-176">The following is a JSON representation of the resource when you publish a raw data notification that is delivered to app clients.</span></span>
```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "rawContent": "String"
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```
