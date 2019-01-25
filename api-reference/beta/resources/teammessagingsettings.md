---
title: tipo de recurso de teamMessagingSettings
description: Configurações para configurar mensagens e menções na equipe de.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d98dfa3c2306cabb99b6de96aed2010cefa10717
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510096"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="c55bf-103">tipo de recurso de teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="c55bf-103">teamMessagingSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c55bf-104">Configurações para configurar mensagens e menções na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="c55bf-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c55bf-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c55bf-105">Properties</span></span>
| <span data-ttu-id="c55bf-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c55bf-106">Property</span></span>     | <span data-ttu-id="c55bf-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c55bf-107">Type</span></span>   |<span data-ttu-id="c55bf-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c55bf-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c55bf-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="c55bf-109">allowUserEditMessages</span></span>|<span data-ttu-id="c55bf-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="c55bf-110">Boolean</span></span>|<span data-ttu-id="c55bf-111">Se definido como true, os usuários pode editar suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="c55bf-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="c55bf-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="c55bf-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="c55bf-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="c55bf-113">Boolean</span></span>|<span data-ttu-id="c55bf-114">Se definido como true, os usuários pode excluir suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="c55bf-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="c55bf-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="c55bf-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="c55bf-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="c55bf-116">Boolean</span></span>|<span data-ttu-id="c55bf-117">Se definido como true, proprietários pode excluir qualquer mensagem.</span><span class="sxs-lookup"><span data-stu-id="c55bf-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="c55bf-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="c55bf-118">allowTeamMentions</span></span>|<span data-ttu-id="c55bf-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="c55bf-119">Boolean</span></span>|<span data-ttu-id="c55bf-120">Se definido como true, @team menções são permitidas.</span><span class="sxs-lookup"><span data-stu-id="c55bf-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="c55bf-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="c55bf-121">allowChannelMentions</span></span>|<span data-ttu-id="c55bf-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="c55bf-122">Boolean</span></span>|<span data-ttu-id="c55bf-123">Se definido como true, @channel menções são permitidas.</span><span class="sxs-lookup"><span data-stu-id="c55bf-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c55bf-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c55bf-124">JSON representation</span></span>

<span data-ttu-id="c55bf-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c55bf-125">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teammessagingsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
