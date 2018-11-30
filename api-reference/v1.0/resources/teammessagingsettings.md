---
title: tipo de recurso de teamMessagingSettings
description: Configurações para configurar mensagens e menções na equipe de.
ms.openlocfilehash: 6d1ca12b473f2773d4f56e12405b17e21b0bd0ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004619"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="7680f-103">tipo de recurso de teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="7680f-103">teamMessagingSettings resource type</span></span>



<span data-ttu-id="7680f-104">Configurações para configurar mensagens e menções na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="7680f-104">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7680f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7680f-105">Properties</span></span>
| <span data-ttu-id="7680f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7680f-106">Property</span></span>     | <span data-ttu-id="7680f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7680f-107">Type</span></span>   |<span data-ttu-id="7680f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7680f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7680f-109">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="7680f-109">allowUserEditMessages</span></span>|<span data-ttu-id="7680f-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="7680f-110">Boolean</span></span>|<span data-ttu-id="7680f-111">Se definido como true, os usuários pode editar suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="7680f-111">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="7680f-112">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="7680f-112">allowUserDeleteMessages</span></span>|<span data-ttu-id="7680f-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="7680f-113">Boolean</span></span>|<span data-ttu-id="7680f-114">Se definido como true, os usuários pode excluir suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="7680f-114">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="7680f-115">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="7680f-115">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="7680f-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="7680f-116">Boolean</span></span>|<span data-ttu-id="7680f-117">Se definido como true, proprietários pode excluir qualquer mensagem.</span><span class="sxs-lookup"><span data-stu-id="7680f-117">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="7680f-118">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="7680f-118">allowTeamMentions</span></span>|<span data-ttu-id="7680f-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="7680f-119">Boolean</span></span>|<span data-ttu-id="7680f-120">Se definido como true, @team menções são permitidas.</span><span class="sxs-lookup"><span data-stu-id="7680f-120">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="7680f-121">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="7680f-121">allowChannelMentions</span></span>|<span data-ttu-id="7680f-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="7680f-122">Boolean</span></span>|<span data-ttu-id="7680f-123">Se definido como true, @channel menções são permitidas.</span><span class="sxs-lookup"><span data-stu-id="7680f-123">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7680f-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7680f-124">JSON representation</span></span>

<span data-ttu-id="7680f-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7680f-125">The following is a JSON representation of the resource.</span></span>

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
