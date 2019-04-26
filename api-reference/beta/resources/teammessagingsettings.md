---
title: tipo de recurso teamMessagingSettings
description: Configurações para definir a mensagens e menções na equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d98dfa3c2306cabb99b6de96aed2010cefa10717
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553943"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="43f01-103">tipo de recurso teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="43f01-103">teamMessagingSettings resource type</span></span>



<span data-ttu-id="43f01-104">Configurações para configurar mensagens e menção na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="43f01-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="43f01-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43f01-105">Properties</span></span>
| <span data-ttu-id="43f01-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43f01-106">Property</span></span>     | <span data-ttu-id="43f01-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="43f01-107">Type</span></span>   |<span data-ttu-id="43f01-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="43f01-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43f01-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="43f01-109">allowUserEditMessages</span></span>|<span data-ttu-id="43f01-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="43f01-110">Boolean</span></span>|<span data-ttu-id="43f01-111">Se definido como true, os usuários podem editar suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="43f01-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="43f01-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="43f01-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="43f01-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="43f01-113">Boolean</span></span>|<span data-ttu-id="43f01-114">Se definido como true, os usuários podem excluir suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="43f01-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="43f01-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="43f01-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="43f01-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="43f01-116">Boolean</span></span>|<span data-ttu-id="43f01-117">Se definido como true, os proprietários podem excluir qualquer mensagem.</span><span class="sxs-lookup"><span data-stu-id="43f01-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="43f01-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="43f01-118">allowTeamMentions</span></span>|<span data-ttu-id="43f01-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="43f01-119">Boolean</span></span>|<span data-ttu-id="43f01-120">Se for definido como true, @team mencionadas serão permitidas.</span><span class="sxs-lookup"><span data-stu-id="43f01-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="43f01-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="43f01-121">allowChannelMentions</span></span>|<span data-ttu-id="43f01-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="43f01-122">Boolean</span></span>|<span data-ttu-id="43f01-123">Se for definido como true, @channel mencionadas serão permitidas.</span><span class="sxs-lookup"><span data-stu-id="43f01-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43f01-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43f01-124">JSON representation</span></span>

<span data-ttu-id="43f01-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43f01-125">The following is a JSON representation of the resource.</span></span>

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
