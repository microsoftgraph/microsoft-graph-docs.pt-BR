---
title: tipo de recurso de teamMessagingSettings
description: Configurações para configurar mensagens e menções na equipe de.
author: nkramer
ms.openlocfilehash: 387c2e3ccedc6f11f17d4868b1b0d3eaf67624fa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304547"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="8c1a2-103">tipo de recurso de teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="8c1a2-103">teamMessagingSettings resource type</span></span>



<span data-ttu-id="8c1a2-104">Configurações para configurar mensagens e menções na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="8c1a2-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8c1a2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c1a2-105">Properties</span></span>
| <span data-ttu-id="8c1a2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c1a2-106">Property</span></span>     | <span data-ttu-id="8c1a2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c1a2-107">Type</span></span>   |<span data-ttu-id="8c1a2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c1a2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c1a2-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="8c1a2-109">allowUserEditMessages</span></span>|<span data-ttu-id="8c1a2-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c1a2-110">Boolean</span></span>|<span data-ttu-id="8c1a2-111">Se definido como true, os usuários pode editar suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="8c1a2-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="8c1a2-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="8c1a2-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="8c1a2-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c1a2-113">Boolean</span></span>|<span data-ttu-id="8c1a2-114">Se definido como true, os usuários pode excluir suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="8c1a2-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="8c1a2-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="8c1a2-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="8c1a2-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c1a2-116">Boolean</span></span>|<span data-ttu-id="8c1a2-117">Se definido como true, proprietários pode excluir qualquer mensagem.</span><span class="sxs-lookup"><span data-stu-id="8c1a2-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="8c1a2-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="8c1a2-118">allowTeamMentions</span></span>|<span data-ttu-id="8c1a2-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c1a2-119">Boolean</span></span>|<span data-ttu-id="8c1a2-120">Se definido como true, @team menções são permitidas.</span><span class="sxs-lookup"><span data-stu-id="8c1a2-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="8c1a2-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="8c1a2-121">allowChannelMentions</span></span>|<span data-ttu-id="8c1a2-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c1a2-122">Boolean</span></span>|<span data-ttu-id="8c1a2-123">Se definido como true, @channel menções são permitidas.</span><span class="sxs-lookup"><span data-stu-id="8c1a2-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c1a2-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c1a2-124">JSON representation</span></span>

<span data-ttu-id="8c1a2-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c1a2-125">The following is a JSON representation of the resource.</span></span>

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
