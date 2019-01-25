---
title: tipo de recurso de notificação
description: 'Representa uma notificação que é publicada por um servidor de aplicativo que tem como destino um usuário especificado. A notificação é armazenada no Microsoft Graph e é distribuída aos pontos de extremidade de dispositivo diferente pertencentes ao usuário. '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: af130c9806511b0afbdaedb602790c7c40d3ca2e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509256"
---
# <a name="notification-resource-type"></a><span data-ttu-id="182d6-104">tipo de recurso de notificação</span><span class="sxs-lookup"><span data-stu-id="182d6-104">notification resource type</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="182d6-105">Representa uma notificação que é publicada por um servidor de aplicativo que tem como destino um usuário especificado.</span><span class="sxs-lookup"><span data-stu-id="182d6-105">Represents a notification that is published by an app server that targets a specified user.</span></span> <span data-ttu-id="182d6-106">A notificação é armazenada no Microsoft Graph e é distribuída aos pontos de extremidade de dispositivo diferente pertencentes ao usuário.</span><span class="sxs-lookup"><span data-stu-id="182d6-106">The notification is stored in Microsoft Graph and is distributed to different device endpoints owned by the user.</span></span> 

<span data-ttu-id="182d6-107">Uma notificação pode ser uma carga de notificação visual que possa ser interpretada por um sistema operacional, incluindo as plataformas Windows, Android e iOS.</span><span class="sxs-lookup"><span data-stu-id="182d6-107">A notification can be a visual notification payload that can be interpreted by the operating system, including Windows, Android, and iOS platforms.</span></span> <span data-ttu-id="182d6-108">Ele também pode ser uma carga de dados que tem entregues e manipulados pelos clientes app, que, em seguida, determine o usuário correspondente experiência em cada dispositivo – em geral, uma notificação visual da interface do usuário que corresponde ao conteúdo a carga de dados original que seja gerada localmente.</span><span class="sxs-lookup"><span data-stu-id="182d6-108">It can also be a data payload that's delivered to and handled by app clients, which then determine the corresponding user experience on each device – usually, a visual notification UI that corresponds to the content in the original data payload that's generated locally.</span></span> 

<span data-ttu-id="182d6-109">Quando um usuário atua em uma notificação visual, o cliente app pode usar, em seguida, Roma SDK do lado do cliente Project para atualizar o estado da notificação correspondente feed no Microsoft Graph - por exemplo, marcando uma notificação conforme descartado.</span><span class="sxs-lookup"><span data-stu-id="182d6-109">When a user acts on a visual notification, the app client can then use client-side Project Rome SDK to update the state of the corresponding notification feed in Microsoft Graph - for example, by marking a notification as dismissed.</span></span> <span data-ttu-id="182d6-110">A atualização, em seguida, será distribuída para todos os outros pontos de cliente app e os clientes manipular a alteração apropriadamente, por exemplo, descarte a notificação para impedir que o usuário ver informações redundantes.</span><span class="sxs-lookup"><span data-stu-id="182d6-110">The update will then be distributed to all other app client endpoints, and the clients handle the change accordingly, for example by dismissing the notification to prevent the user from seeing redundant information.</span></span> <span data-ttu-id="182d6-111">Clientes de aplicativo podem acessar o mesmo recurso de notificação em um momento posterior antes que ela expire (mesmo depois que ela é marcada como descartado), como histórico de notificação, por meio do [SDK do Project Roma](https://github.com/Microsoft/project-rome).</span><span class="sxs-lookup"><span data-stu-id="182d6-111">App clients can access the same notification resource at a later time before it expires (even after it is marked as dismissed), as notification history, via the [Project Rome SDK](https://github.com/Microsoft/project-rome).</span></span> 

## <a name="methods"></a><span data-ttu-id="182d6-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="182d6-112">Methods</span></span>
|<span data-ttu-id="182d6-113">Método</span><span class="sxs-lookup"><span data-stu-id="182d6-113">Method</span></span> | <span data-ttu-id="182d6-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="182d6-114">Return Type</span></span> | <span data-ttu-id="182d6-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="182d6-115">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="182d6-116">Criar notificação</span><span class="sxs-lookup"><span data-stu-id="182d6-116">Create notification</span></span>](../api/projectrome-notification-post.md) | <span data-ttu-id="182d6-117">Notification</span><span class="sxs-lookup"><span data-stu-id="182d6-117">[notification](projectrome-notification.md)</span></span> |<span data-ttu-id="182d6-118">Criar e enviar uma notificação.</span><span class="sxs-lookup"><span data-stu-id="182d6-118">Create and send a notification.</span></span> |

## <a name="properties"></a><span data-ttu-id="182d6-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="182d6-119">Properties</span></span>
|<span data-ttu-id="182d6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="182d6-120">Name</span></span> | <span data-ttu-id="182d6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="182d6-121">Type</span></span> | <span data-ttu-id="182d6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="182d6-122">Description</span></span>|
|:----|:-----|:-----------|
| <span data-ttu-id="182d6-123">targetHostName</span><span class="sxs-lookup"><span data-stu-id="182d6-123">targetHostName</span></span> | <span data-ttu-id="182d6-124">String</span><span class="sxs-lookup"><span data-stu-id="182d6-124">String</span></span> | <span data-ttu-id="182d6-125">Representa o nome de host do aplicativo ao qual o serviço de chamada deseja postar a notificação, para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="182d6-125">Represents the host name of the app to which the calling service wants to post the notification, for the given user.</span></span> |
| <span data-ttu-id="182d6-126">appNotificationId</span><span class="sxs-lookup"><span data-stu-id="182d6-126">appNotificationId</span></span> | <span data-ttu-id="182d6-127">String</span><span class="sxs-lookup"><span data-stu-id="182d6-127">String</span></span> | <span data-ttu-id="182d6-128">A id exclusiva definida pelo servidor de aplicativo de uma notificação que é usado para identificar e uma notificação individual de destino.</span><span class="sxs-lookup"><span data-stu-id="182d6-128">The unique id set by the app server of a notification that is used to identify and target an individual notification.</span></span> |
| <span data-ttu-id="182d6-129">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="182d6-129">expirationDateTime</span></span> | <span data-ttu-id="182d6-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="182d6-130">DateTimeOffset</span></span> | <span data-ttu-id="182d6-131">Define um tempo de expiração de UTC em uma notificação de usuário - quando o tempo é para cima, a notificação é removida do repositório de feed de notificação do Microsoft Graph completamente e não está mais parte do histórico de notificação.</span><span class="sxs-lookup"><span data-stu-id="182d6-131">Sets a UTC expiration time on a user notification - when time is up, the notification is removed from the Microsoft Graph notification feed store completely and is no longer part of notification history.</span></span> <span data-ttu-id="182d6-132">Valor máximo é 30 dias.</span><span class="sxs-lookup"><span data-stu-id="182d6-132">Max value is 30 days.</span></span> |
| <span data-ttu-id="182d6-133">payload</span><span class="sxs-lookup"><span data-stu-id="182d6-133">payload</span></span> | <span data-ttu-id="182d6-134">Edm.ComplexType, o objeto JSON</span><span class="sxs-lookup"><span data-stu-id="182d6-134">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="182d6-135">Esse é o conteúdo de dados de uma notificação de usuário brutos ou visual que serão entregues e consumido pelo cliente app receber essa notificação.</span><span class="sxs-lookup"><span data-stu-id="182d6-135">This is the data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> |
| <span data-ttu-id="182d6-136">payload.rawContent</span><span class="sxs-lookup"><span data-stu-id="182d6-136">payload.rawContent</span></span> | <span data-ttu-id="182d6-137">String</span><span class="sxs-lookup"><span data-stu-id="182d6-137">String</span></span> | <span data-ttu-id="182d6-138">O conteúdo de notificação de uma notificação de usuário brutos que serão entregues e consumido pelo cliente app receber essa notificação.</span><span class="sxs-lookup"><span data-stu-id="182d6-138">The notification content of a raw user notification that will be delivered to and consumed by the app client receiving this notification.</span></span> <span data-ttu-id="182d6-139">Pelo menos uma das Payload.RawContent e Payload.VisualContent precisa ser válida para uma solicitação de notificação de POSTAGEM.</span><span class="sxs-lookup"><span data-stu-id="182d6-139">At least one of Payload.RawContent and Payload.VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="182d6-140">payload.Visual</span><span class="sxs-lookup"><span data-stu-id="182d6-140">payload.visual</span></span> | <span data-ttu-id="182d6-141">Edm.ComplexType, o objeto JSON</span><span class="sxs-lookup"><span data-stu-id="182d6-141">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="182d6-142">O conteúdo visual de uma notificação de usuário visual, que será consumida pela plataforma de notificação em cada plataforma móvel e renderizado para os usuários.</span><span class="sxs-lookup"><span data-stu-id="182d6-142">The visual content of a visual user notification, which will be consumed by the notification platform on each mobile platform and rendered for the users.</span></span> <span data-ttu-id="182d6-143">Pelo menos um dos conteúdo e VisualContent precisa ser válida para uma solicitação de notificação de POSTAGEM.</span><span class="sxs-lookup"><span data-stu-id="182d6-143">At least one of Content and VisualContent needs to be valid for a POST Notification request.</span></span> |
| <span data-ttu-id="182d6-144">payload.Visual.Title</span><span class="sxs-lookup"><span data-stu-id="182d6-144">payload.visual.title</span></span> | <span data-ttu-id="182d6-145">String</span><span class="sxs-lookup"><span data-stu-id="182d6-145">String</span></span> | <span data-ttu-id="182d6-146">O título de uma notificação de usuário visual.</span><span class="sxs-lookup"><span data-stu-id="182d6-146">The title of a visual user notification.</span></span> <span data-ttu-id="182d6-147">Deve ter o título ou corpo.</span><span class="sxs-lookup"><span data-stu-id="182d6-147">Must have either title or body.</span></span> |
| <span data-ttu-id="182d6-148">payload.Visual.body</span><span class="sxs-lookup"><span data-stu-id="182d6-148">payload.visual.body</span></span> | <span data-ttu-id="182d6-149">String</span><span class="sxs-lookup"><span data-stu-id="182d6-149">String</span></span> | <span data-ttu-id="182d6-150">O corpo de uma notificação de usuário visual.</span><span class="sxs-lookup"><span data-stu-id="182d6-150">The body of a visual user notification.</span></span> <span data-ttu-id="182d6-151">Deve ter o título ou corpo.</span><span class="sxs-lookup"><span data-stu-id="182d6-151">Must have either title or body.</span></span> |
| <span data-ttu-id="182d6-152">displayTimeToLive</span><span class="sxs-lookup"><span data-stu-id="182d6-152">displayTimeToLive</span></span> | <span data-ttu-id="182d6-153">Int</span><span class="sxs-lookup"><span data-stu-id="182d6-153">Int</span></span> | <span data-ttu-id="182d6-154">Define quanto tempo (em segundos) esse conteúdo notificação permanecerão no Visualizador de notificação da cada plataforma.</span><span class="sxs-lookup"><span data-stu-id="182d6-154">Sets how long (in seconds) this notification content will stay in each platform’s notification viewer.</span></span> <span data-ttu-id="182d6-155">Por exemplo, quando a notificação é entregue a um dispositivo do Windows, o valor dessa propriedade é passado para ToastNotification.ExpirationTime, que determina quanto tempo a notificação de proposta permanecerão na Central de ações do Windows do usuário.</span><span class="sxs-lookup"><span data-stu-id="182d6-155">For example, when the notification is delivered to a Windows device, the value of this property is passed on to ToastNotification.ExpirationTime, which determines how long the toast notification will stay in the user’s Windows Action Center.</span></span> |
| <span data-ttu-id="182d6-156">prioridade</span><span class="sxs-lookup"><span data-stu-id="182d6-156">priority</span></span> | <span data-ttu-id="182d6-157">EnumType</span><span class="sxs-lookup"><span data-stu-id="182d6-157">EnumType</span></span> | <span data-ttu-id="182d6-158">Indica a prioridade de uma notificação de usuário brutos.</span><span class="sxs-lookup"><span data-stu-id="182d6-158">Indicates the priority of a raw user notification.</span></span> <span data-ttu-id="182d6-159">Por padrão, notificações visuais são enviadas com alta prioridade.</span><span class="sxs-lookup"><span data-stu-id="182d6-159">Visual notifications are sent with high priority by default.</span></span> <span data-ttu-id="182d6-160">Valores válidos são de alta e baixa.</span><span class="sxs-lookup"><span data-stu-id="182d6-160">Valid values are High and Low.</span></span> |
| <span data-ttu-id="182d6-161">GroupName</span><span class="sxs-lookup"><span data-stu-id="182d6-161">groupName</span></span> | <span data-ttu-id="182d6-162">String</span><span class="sxs-lookup"><span data-stu-id="182d6-162">String</span></span> | <span data-ttu-id="182d6-163">O nome do grupo ao qual essa notificação pertence.</span><span class="sxs-lookup"><span data-stu-id="182d6-163">The name of the group that this notification belongs to.</span></span> <span data-ttu-id="182d6-164">Ela é definida pelo desenvolvedor para fins de agrupamento de notificações.</span><span class="sxs-lookup"><span data-stu-id="182d6-164">It is set by the developer for the purpose of grouping notifications together.</span></span> |
| <span data-ttu-id="182d6-165">targetPolicy</span><span class="sxs-lookup"><span data-stu-id="182d6-165">targetPolicy</span></span> | <span data-ttu-id="182d6-166">Edm.ComplexType, o objeto JSON</span><span class="sxs-lookup"><span data-stu-id="182d6-166">Edm.ComplexType, JSON object</span></span> | <span data-ttu-id="182d6-167">Política de entrega da notificação em dois níveis diferentes - tipos de ponto de extremidade (Windows, iOS e Android) que devem ser direcionados e pontos de extremidade específicos (identificados por ids de inscrição) que devem ser direcionados lida com o objeto de diretiva de destino.</span><span class="sxs-lookup"><span data-stu-id="182d6-167">Target policy object handles notification delivery policy at two different levels - endpoint types (Windows, iOS and Android) that should be targeted, and specific endpoints (identified by subscription ids) that should be targeted.</span></span> |
| <span data-ttu-id="182d6-168">targetPolicy.platformTypes</span><span class="sxs-lookup"><span data-stu-id="182d6-168">targetPolicy.platformTypes</span></span> | <span data-ttu-id="182d6-169">Edm.ComplexType, a coleção (EnumType)</span><span class="sxs-lookup"><span data-stu-id="182d6-169">Edm.ComplexType, Collection (EnumType)</span></span> | <span data-ttu-id="182d6-170">Use para filtrar a distribuição de notificação para uma plataforma específica ou plataformas.</span><span class="sxs-lookup"><span data-stu-id="182d6-170">Use to filter the notification distribution to a specific platform or platforms.</span></span> <span data-ttu-id="182d6-171">Por padrão, todos os tipos de ponto de extremidade de push (iOS, Windows e Android) estão habilitados.</span><span class="sxs-lookup"><span data-stu-id="182d6-171">By default, all push endpoint types (iOS, Windows, and Android) are enabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="182d6-172">Relações</span><span class="sxs-lookup"><span data-stu-id="182d6-172">Relationships</span></span>
<span data-ttu-id="182d6-173">Nenhum</span><span class="sxs-lookup"><span data-stu-id="182d6-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="182d6-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="182d6-174">JSON representation</span></span>
<span data-ttu-id="182d6-175">A seguir está uma representação JSON do recurso quando você publica uma notificação visual direta que será enviada para o sistema operacional de destino.</span><span class="sxs-lookup"><span data-stu-id="182d6-175">The following is a JSON representation of the resource when you publish a direct visual notification that is delivered to the destination operating system.</span></span>

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

<span data-ttu-id="182d6-176">A seguir está uma representação JSON do recurso quando você publica uma notificação de dados brutos é entregue aos clientes app.</span><span class="sxs-lookup"><span data-stu-id="182d6-176">The following is a JSON representation of the resource when you publish a raw data notification that is delivered to app clients.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-notification.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
