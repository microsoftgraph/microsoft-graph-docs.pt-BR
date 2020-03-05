---
title: tipo de recurso teamMemberSettings
description: Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots na equipe.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f77bc80a5723e3e00675aeaab05f2dd7ea180f76
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519936"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="35699-103">tipo de recurso teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="35699-103">teamMemberSettings resource type</span></span>

<span data-ttu-id="35699-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="35699-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35699-105">Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots, na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="35699-105">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="35699-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35699-106">Properties</span></span>
| <span data-ttu-id="35699-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35699-107">Property</span></span>     | <span data-ttu-id="35699-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="35699-108">Type</span></span>   |<span data-ttu-id="35699-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="35699-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35699-110">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="35699-110">allowCreateUpdateChannels</span></span>|<span data-ttu-id="35699-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="35699-111">Boolean</span></span>|<span data-ttu-id="35699-112">Se definido como true, os membros podem adicionar e atualizar qualquer canal.</span><span class="sxs-lookup"><span data-stu-id="35699-112">If set to true, members can add and update any channels.</span></span>|
|<span data-ttu-id="35699-113">allowCreatePrivateChannels</span><span class="sxs-lookup"><span data-stu-id="35699-113">allowCreatePrivateChannels</span></span>|<span data-ttu-id="35699-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="35699-114">Boolean</span></span>|<span data-ttu-id="35699-115">Se definido como true, os membros podem adicionar e atualizar canais privados.</span><span class="sxs-lookup"><span data-stu-id="35699-115">If set to true, members can add and update private channels.</span></span>|
|<span data-ttu-id="35699-116">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="35699-116">allowDeleteChannels</span></span>|<span data-ttu-id="35699-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="35699-117">Boolean</span></span>|<span data-ttu-id="35699-118">Se definido como true, os membros podem excluir canais.</span><span class="sxs-lookup"><span data-stu-id="35699-118">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="35699-119">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="35699-119">allowAddRemoveApps</span></span>|<span data-ttu-id="35699-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="35699-120">Boolean</span></span>|<span data-ttu-id="35699-121">Se definido como true, os membros podem adicionar e remover aplicativos.</span><span class="sxs-lookup"><span data-stu-id="35699-121">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="35699-122">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="35699-122">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="35699-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="35699-123">Boolean</span></span>|<span data-ttu-id="35699-124">Se definido como true, os membros podem adicionar, atualizar e remover guias.</span><span class="sxs-lookup"><span data-stu-id="35699-124">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="35699-125">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="35699-125">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="35699-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="35699-126">Boolean</span></span>|<span data-ttu-id="35699-127">Se definido como true, os membros podem adicionar, atualizar e remover conectores.</span><span class="sxs-lookup"><span data-stu-id="35699-127">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35699-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35699-128">JSON representation</span></span>

<span data-ttu-id="35699-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35699-129">The following is a JSON representation of the resource.</span></span>

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
