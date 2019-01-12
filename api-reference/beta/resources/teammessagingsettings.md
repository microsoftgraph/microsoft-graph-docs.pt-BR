---
title: tipo de recurso de teamMessagingSettings
description: Configurações para configurar mensagens e menções na equipe de.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 342062ee9661758c8b3179e21246b9366d832f3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930401"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="bb2ec-103">tipo de recurso de teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="bb2ec-103">teamMessagingSettings resource type</span></span>

> <span data-ttu-id="bb2ec-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bb2ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb2ec-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bb2ec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb2ec-106">Configurações para configurar mensagens e menções na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="bb2ec-106">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bb2ec-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb2ec-107">Properties</span></span>
| <span data-ttu-id="bb2ec-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb2ec-108">Property</span></span>     | <span data-ttu-id="bb2ec-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb2ec-109">Type</span></span>   |<span data-ttu-id="bb2ec-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb2ec-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb2ec-111">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="bb2ec-111">allowUserEditMessages</span></span>|<span data-ttu-id="bb2ec-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb2ec-112">Boolean</span></span>|<span data-ttu-id="bb2ec-113">Se definido como true, os usuários pode editar suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="bb2ec-113">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="bb2ec-114">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="bb2ec-114">allowUserDeleteMessages</span></span>|<span data-ttu-id="bb2ec-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb2ec-115">Boolean</span></span>|<span data-ttu-id="bb2ec-116">Se definido como true, os usuários pode excluir suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="bb2ec-116">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="bb2ec-117">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="bb2ec-117">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="bb2ec-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb2ec-118">Boolean</span></span>|<span data-ttu-id="bb2ec-119">Se definido como true, proprietários pode excluir qualquer mensagem.</span><span class="sxs-lookup"><span data-stu-id="bb2ec-119">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="bb2ec-120">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="bb2ec-120">allowTeamMentions</span></span>|<span data-ttu-id="bb2ec-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb2ec-121">Boolean</span></span>|<span data-ttu-id="bb2ec-122">Se definido como true, @team menções são permitidas.</span><span class="sxs-lookup"><span data-stu-id="bb2ec-122">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="bb2ec-123">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="bb2ec-123">allowChannelMentions</span></span>|<span data-ttu-id="bb2ec-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb2ec-124">Boolean</span></span>|<span data-ttu-id="bb2ec-125">Se definido como true, @channel menções são permitidas.</span><span class="sxs-lookup"><span data-stu-id="bb2ec-125">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb2ec-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb2ec-126">JSON representation</span></span>

<span data-ttu-id="bb2ec-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb2ec-127">The following is a JSON representation of the resource.</span></span>

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
