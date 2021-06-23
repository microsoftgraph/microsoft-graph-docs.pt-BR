---
title: Tipo de recurso teamMemberSettings
description: Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots na equipe.
localization_priority: Normal
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dfa463ce47b9724d18f6f13b53ef46a1cb493f4a
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060454"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="bbcf3-103">Tipo de recurso teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="bbcf3-103">teamMemberSettings resource type</span></span>

<span data-ttu-id="bbcf3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbcf3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbcf3-105">Configurações configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots, na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="bbcf3-105">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bbcf3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bbcf3-106">Properties</span></span>
| <span data-ttu-id="bbcf3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbcf3-107">Property</span></span>     | <span data-ttu-id="bbcf3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbcf3-108">Type</span></span>   |<span data-ttu-id="bbcf3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbcf3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbcf3-110">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="bbcf3-110">allowCreateUpdateChannels</span></span>|<span data-ttu-id="bbcf3-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="bbcf3-111">Boolean</span></span>|<span data-ttu-id="bbcf3-112">Se definido como true, os membros podem adicionar e atualizar quaisquer canais.</span><span class="sxs-lookup"><span data-stu-id="bbcf3-112">If set to true, members can add and update any channels.</span></span>|
|<span data-ttu-id="bbcf3-113">allowCreatePrivateChannels</span><span class="sxs-lookup"><span data-stu-id="bbcf3-113">allowCreatePrivateChannels</span></span>|<span data-ttu-id="bbcf3-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="bbcf3-114">Boolean</span></span>|<span data-ttu-id="bbcf3-115">Se definido como true, os membros podem adicionar e atualizar canais privados.</span><span class="sxs-lookup"><span data-stu-id="bbcf3-115">If set to true, members can add and update private channels.</span></span>|
|<span data-ttu-id="bbcf3-116">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="bbcf3-116">allowDeleteChannels</span></span>|<span data-ttu-id="bbcf3-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="bbcf3-117">Boolean</span></span>|<span data-ttu-id="bbcf3-118">Se definido como true, os membros poderão excluir canais.</span><span class="sxs-lookup"><span data-stu-id="bbcf3-118">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="bbcf3-119">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="bbcf3-119">allowAddRemoveApps</span></span>|<span data-ttu-id="bbcf3-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="bbcf3-120">Boolean</span></span>|<span data-ttu-id="bbcf3-121">Se definido como true, os membros podem adicionar e remover aplicativos.</span><span class="sxs-lookup"><span data-stu-id="bbcf3-121">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="bbcf3-122">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="bbcf3-122">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="bbcf3-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="bbcf3-123">Boolean</span></span>|<span data-ttu-id="bbcf3-124">Se definido como true, os membros podem adicionar, atualizar e remover guias.</span><span class="sxs-lookup"><span data-stu-id="bbcf3-124">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="bbcf3-125">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="bbcf3-125">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="bbcf3-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="bbcf3-126">Boolean</span></span>|<span data-ttu-id="bbcf3-127">Se definido como true, os membros podem adicionar, atualizar e remover conectores.</span><span class="sxs-lookup"><span data-stu-id="bbcf3-127">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bbcf3-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bbcf3-128">JSON representation</span></span>

<span data-ttu-id="bbcf3-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bbcf3-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowCreatePrivateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


