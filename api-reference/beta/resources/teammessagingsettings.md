---
title: tipo de recurso teamMessagingSettings
description: Configurações para definir a mensagens e menções na equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3a89ed35c820338cde7b3f22a7345c860b1a4427
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964526"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="425ae-103">tipo de recurso teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="425ae-103">teamMessagingSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="425ae-104">Configurações para configurar mensagens e menção na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="425ae-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="425ae-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="425ae-105">Properties</span></span>
| <span data-ttu-id="425ae-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="425ae-106">Property</span></span>     | <span data-ttu-id="425ae-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="425ae-107">Type</span></span>   |<span data-ttu-id="425ae-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="425ae-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="425ae-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="425ae-109">allowUserEditMessages</span></span>|<span data-ttu-id="425ae-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="425ae-110">Boolean</span></span>|<span data-ttu-id="425ae-111">Se definido como true, os usuários podem editar suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="425ae-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="425ae-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="425ae-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="425ae-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="425ae-113">Boolean</span></span>|<span data-ttu-id="425ae-114">Se definido como true, os usuários podem excluir suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="425ae-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="425ae-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="425ae-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="425ae-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="425ae-116">Boolean</span></span>|<span data-ttu-id="425ae-117">Se definido como true, os proprietários podem excluir qualquer mensagem.</span><span class="sxs-lookup"><span data-stu-id="425ae-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="425ae-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="425ae-118">allowTeamMentions</span></span>|<span data-ttu-id="425ae-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="425ae-119">Boolean</span></span>|<span data-ttu-id="425ae-120">Se for definido como true, @team mencionadas serão permitidas.</span><span class="sxs-lookup"><span data-stu-id="425ae-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="425ae-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="425ae-121">allowChannelMentions</span></span>|<span data-ttu-id="425ae-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="425ae-122">Boolean</span></span>|<span data-ttu-id="425ae-123">Se for definido como true, @channel mencionadas serão permitidas.</span><span class="sxs-lookup"><span data-stu-id="425ae-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="425ae-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="425ae-124">JSON representation</span></span>

<span data-ttu-id="425ae-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="425ae-125">The following is a JSON representation of the resource.</span></span>

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
