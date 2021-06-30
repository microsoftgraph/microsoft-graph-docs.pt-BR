---
title: Tipo de recurso channelMembersNotificationRecipient
description: Representa o destinatário de uma notificação enviada em um feed Microsoft Teams atividade. O destinatário consiste nos membros do canal.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 821d4f2ee41c15cb93cd3d53b9af9cf1e63db97b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211211"
---
# <a name="channelmembersnotificationrecipient-resource-type"></a><span data-ttu-id="4ab38-104">Tipo de recurso channelMembersNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="4ab38-104">channelMembersNotificationRecipient resource type</span></span>

<span data-ttu-id="4ab38-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ab38-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ab38-106">Representa o destinatário de uma notificação enviada em um feed Microsoft Teams atividade.</span><span class="sxs-lookup"><span data-stu-id="4ab38-106">Represents the recipient of a notification sent in a Microsoft Teams activity feed.</span></span> <span data-ttu-id="4ab38-107">O destinatário consiste nos membros do canal.</span><span class="sxs-lookup"><span data-stu-id="4ab38-107">The recipient consists of the channel members.</span></span>

<span data-ttu-id="4ab38-108">Herda de [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="4ab38-108">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4ab38-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ab38-109">Properties</span></span>
| <span data-ttu-id="4ab38-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ab38-110">Property</span></span>  | <span data-ttu-id="4ab38-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ab38-111">Type</span></span>   | <span data-ttu-id="4ab38-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ab38-112">Description</span></span>                                            |
| :-------- | :----- | :----------------------------------------------------- |
| <span data-ttu-id="4ab38-113">teamId</span><span class="sxs-lookup"><span data-stu-id="4ab38-113">teamId</span></span>    | <span data-ttu-id="4ab38-114">String</span><span class="sxs-lookup"><span data-stu-id="4ab38-114">String</span></span> | <span data-ttu-id="4ab38-115">O identificador da equipe no qual o canal reside.</span><span class="sxs-lookup"><span data-stu-id="4ab38-115">The team's identifier under which the channel resides.</span></span> |
| <span data-ttu-id="4ab38-116">channelId</span><span class="sxs-lookup"><span data-stu-id="4ab38-116">channelId</span></span> | <span data-ttu-id="4ab38-117">String</span><span class="sxs-lookup"><span data-stu-id="4ab38-117">String</span></span> | <span data-ttu-id="4ab38-118">O identificador do canal.</span><span class="sxs-lookup"><span data-stu-id="4ab38-118">The channel's identifier.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="4ab38-119">Relações</span><span class="sxs-lookup"><span data-stu-id="4ab38-119">Relationships</span></span>
<span data-ttu-id="4ab38-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ab38-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ab38-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ab38-121">JSON representation</span></span>
<span data-ttu-id="4ab38-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ab38-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelMembersNotificationRecipient"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.channelMembersNotificationRecipient",
  "teamId": "String",
  "channelId": "String"
}
```
