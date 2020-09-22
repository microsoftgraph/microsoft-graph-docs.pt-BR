---
title: tipo de recurso teamMessagingSettings
description: Configurações para definir a mensagens e menções na equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 352fc5bc8a8794a455a84d729bb3b2cea6ad34f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046626"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="1a64f-103">tipo de recurso teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="1a64f-103">teamMessagingSettings resource type</span></span>

<span data-ttu-id="1a64f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a64f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a64f-105">Configurações para configurar mensagens e menção na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="1a64f-105">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1a64f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a64f-106">Properties</span></span>
| <span data-ttu-id="1a64f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a64f-107">Property</span></span>     | <span data-ttu-id="1a64f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a64f-108">Type</span></span>   |<span data-ttu-id="1a64f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a64f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a64f-110">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="1a64f-110">allowUserEditMessages</span></span>|<span data-ttu-id="1a64f-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a64f-111">Boolean</span></span>|<span data-ttu-id="1a64f-112">Se definido como true, os usuários podem editar suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="1a64f-112">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="1a64f-113">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="1a64f-113">allowUserDeleteMessages</span></span>|<span data-ttu-id="1a64f-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a64f-114">Boolean</span></span>|<span data-ttu-id="1a64f-115">Se definido como true, os usuários podem excluir suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="1a64f-115">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="1a64f-116">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="1a64f-116">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="1a64f-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a64f-117">Boolean</span></span>|<span data-ttu-id="1a64f-118">Se definido como true, os proprietários podem excluir qualquer mensagem.</span><span class="sxs-lookup"><span data-stu-id="1a64f-118">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="1a64f-119">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="1a64f-119">allowTeamMentions</span></span>|<span data-ttu-id="1a64f-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a64f-120">Boolean</span></span>|<span data-ttu-id="1a64f-121">Se for definido como true, @team mencionadas serão permitidas.</span><span class="sxs-lookup"><span data-stu-id="1a64f-121">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="1a64f-122">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="1a64f-122">allowChannelMentions</span></span>|<span data-ttu-id="1a64f-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a64f-123">Boolean</span></span>|<span data-ttu-id="1a64f-124">Se for definido como true, @channel mencionadas serão permitidas.</span><span class="sxs-lookup"><span data-stu-id="1a64f-124">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a64f-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a64f-125">JSON representation</span></span>

<span data-ttu-id="1a64f-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a64f-126">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


