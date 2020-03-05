---
title: tipo de recurso teamMessagingSettings
description: Configurações para definir a mensagens e menções na equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 213a8d388b80a4b35d26afc0071445a8ac6095b9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519929"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="0c033-103">tipo de recurso teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="0c033-103">teamMessagingSettings resource type</span></span>

<span data-ttu-id="0c033-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0c033-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c033-105">Configurações para configurar mensagens e menção na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="0c033-105">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0c033-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c033-106">Properties</span></span>
| <span data-ttu-id="0c033-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c033-107">Property</span></span>     | <span data-ttu-id="0c033-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c033-108">Type</span></span>   |<span data-ttu-id="0c033-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c033-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c033-110">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="0c033-110">allowUserEditMessages</span></span>|<span data-ttu-id="0c033-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c033-111">Boolean</span></span>|<span data-ttu-id="0c033-112">Se definido como true, os usuários podem editar suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="0c033-112">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="0c033-113">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="0c033-113">allowUserDeleteMessages</span></span>|<span data-ttu-id="0c033-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c033-114">Boolean</span></span>|<span data-ttu-id="0c033-115">Se definido como true, os usuários podem excluir suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="0c033-115">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="0c033-116">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="0c033-116">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="0c033-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c033-117">Boolean</span></span>|<span data-ttu-id="0c033-118">Se definido como true, os proprietários podem excluir qualquer mensagem.</span><span class="sxs-lookup"><span data-stu-id="0c033-118">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="0c033-119">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="0c033-119">allowTeamMentions</span></span>|<span data-ttu-id="0c033-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c033-120">Boolean</span></span>|<span data-ttu-id="0c033-121">Se for definido como true, @team mencionadas serão permitidas.</span><span class="sxs-lookup"><span data-stu-id="0c033-121">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="0c033-122">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="0c033-122">allowChannelMentions</span></span>|<span data-ttu-id="0c033-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c033-123">Boolean</span></span>|<span data-ttu-id="0c033-124">Se for definido como true, @channel mencionadas serão permitidas.</span><span class="sxs-lookup"><span data-stu-id="0c033-124">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c033-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c033-125">JSON representation</span></span>

<span data-ttu-id="0c033-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c033-126">The following is a JSON representation of the resource.</span></span>

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
