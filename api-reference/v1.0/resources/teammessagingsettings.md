---
title: tipo de recurso teamMessagingSettings
description: Configurações para definir a mensagens e menções na equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e742dd0e785a94b33a57e55b50a00aab0c207ab4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533516"
---
# <a name="teammessagingsettings-resource-type"></a><span data-ttu-id="1fd12-103">tipo de recurso teamMessagingSettings</span><span class="sxs-lookup"><span data-stu-id="1fd12-103">teamMessagingSettings resource type</span></span>

<span data-ttu-id="1fd12-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fd12-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="1fd12-105">Configurações para configurar mensagens e menção na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="1fd12-105">Settings to configure messaging and mentions in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1fd12-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1fd12-106">Properties</span></span>
| <span data-ttu-id="1fd12-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fd12-107">Property</span></span>     | <span data-ttu-id="1fd12-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fd12-108">Type</span></span>   |<span data-ttu-id="1fd12-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fd12-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fd12-110">allowUserEditMessages</span><span class="sxs-lookup"><span data-stu-id="1fd12-110">allowUserEditMessages</span></span>|<span data-ttu-id="1fd12-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="1fd12-111">Boolean</span></span>|<span data-ttu-id="1fd12-112">Se definido como true, os usuários podem editar suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="1fd12-112">If set to true, users can edit their messages.</span></span>|
|<span data-ttu-id="1fd12-113">allowUserDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="1fd12-113">allowUserDeleteMessages</span></span>|<span data-ttu-id="1fd12-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="1fd12-114">Boolean</span></span>|<span data-ttu-id="1fd12-115">Se definido como true, os usuários podem excluir suas mensagens.</span><span class="sxs-lookup"><span data-stu-id="1fd12-115">If set to true, users can delete their messages.</span></span>|
|<span data-ttu-id="1fd12-116">allowOwnerDeleteMessages</span><span class="sxs-lookup"><span data-stu-id="1fd12-116">allowOwnerDeleteMessages</span></span>|<span data-ttu-id="1fd12-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="1fd12-117">Boolean</span></span>|<span data-ttu-id="1fd12-118">Se definido como true, os proprietários podem excluir qualquer mensagem.</span><span class="sxs-lookup"><span data-stu-id="1fd12-118">If set to true, owners can delete any message.</span></span>|
|<span data-ttu-id="1fd12-119">allowTeamMentions</span><span class="sxs-lookup"><span data-stu-id="1fd12-119">allowTeamMentions</span></span>|<span data-ttu-id="1fd12-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="1fd12-120">Boolean</span></span>|<span data-ttu-id="1fd12-121">Se for definido como true, @team mencionadas serão permitidas.</span><span class="sxs-lookup"><span data-stu-id="1fd12-121">If set to true, @team mentions are allowed.</span></span>|
|<span data-ttu-id="1fd12-122">allowChannelMentions</span><span class="sxs-lookup"><span data-stu-id="1fd12-122">allowChannelMentions</span></span>|<span data-ttu-id="1fd12-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="1fd12-123">Boolean</span></span>|<span data-ttu-id="1fd12-124">Se for definido como true, @channel mencionadas serão permitidas.</span><span class="sxs-lookup"><span data-stu-id="1fd12-124">If set to true, @channel mentions are allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1fd12-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1fd12-125">JSON representation</span></span>

<span data-ttu-id="1fd12-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1fd12-126">The following is a JSON representation of the resource.</span></span>

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
