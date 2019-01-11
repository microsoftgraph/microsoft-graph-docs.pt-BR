---
title: tipo de recurso de teamMessagingSettings
description: Configurações para configurar mensagens e menções na equipe de.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: df80fbb828a400e736b2e8c3b73f949fe6bfd1ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878376"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="7ae99-103">tipo de recurso de teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="7ae99-103">teamMessagingSettings resource type</span></span>



<span data-ttu-id="7ae99-104">Configurações para configurar mensagens e menções na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="7ae99-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7ae99-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ae99-105">Properties</span></span>
| <span data-ttu-id="7ae99-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ae99-106">Property</span></span>     | <span data-ttu-id="7ae99-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ae99-107">Type</span></span>   |<span data-ttu-id="7ae99-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ae99-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7ae99-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="7ae99-109">allowUserEditMessages</span></span>|<span data-ttu-id="7ae99-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ae99-110">Boolean</span></span>|<span data-ttu-id="7ae99-111">Se definido como true, os usuários pode editar suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="7ae99-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="7ae99-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="7ae99-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="7ae99-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ae99-113">Boolean</span></span>|<span data-ttu-id="7ae99-114">Se definido como true, os usuários pode excluir suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="7ae99-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="7ae99-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="7ae99-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="7ae99-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ae99-116">Boolean</span></span>|<span data-ttu-id="7ae99-117">Se definido como true, proprietários pode excluir qualquer mensagem.</span><span class="sxs-lookup"><span data-stu-id="7ae99-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="7ae99-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="7ae99-118">allowTeamMentions</span></span>|<span data-ttu-id="7ae99-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ae99-119">Boolean</span></span>|<span data-ttu-id="7ae99-120">Se definido como true, @team menções são permitidas.</span><span class="sxs-lookup"><span data-stu-id="7ae99-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="7ae99-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="7ae99-121">allowChannelMentions</span></span>|<span data-ttu-id="7ae99-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ae99-122">Boolean</span></span>|<span data-ttu-id="7ae99-123">Se definido como true, @channel menções são permitidas.</span><span class="sxs-lookup"><span data-stu-id="7ae99-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7ae99-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ae99-124">JSON representation</span></span>

<span data-ttu-id="7ae99-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ae99-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
