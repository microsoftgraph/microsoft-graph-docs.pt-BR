---
title: tipo de recurso teamMemberSettings
description: Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots na equipe.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7087457ac68c98b40b1c89dc4b99b13ae85d46b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094005"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="69aea-103">tipo de recurso teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="69aea-103">teamMemberSettings resource type</span></span>

<span data-ttu-id="69aea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69aea-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="69aea-105">Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots, na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="69aea-105">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="69aea-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69aea-106">Properties</span></span>
| <span data-ttu-id="69aea-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69aea-107">Property</span></span>     | <span data-ttu-id="69aea-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="69aea-108">Type</span></span>   |<span data-ttu-id="69aea-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="69aea-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69aea-110">allowCreatePrivateChannels</span><span class="sxs-lookup"><span data-stu-id="69aea-110">allowCreatePrivateChannels</span></span>|<span data-ttu-id="69aea-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="69aea-111">Boolean</span></span>|<span data-ttu-id="69aea-112">Se definido como true, os membros podem adicionar e atualizar canais privados.</span><span class="sxs-lookup"><span data-stu-id="69aea-112">If set to true, members can add and update private channels.</span></span>|
|<span data-ttu-id="69aea-113">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="69aea-113">allowCreateUpdateChannels</span></span>|<span data-ttu-id="69aea-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="69aea-114">Boolean</span></span>|<span data-ttu-id="69aea-115">Se definido como true, os membros podem adicionar e atualizar canais.</span><span class="sxs-lookup"><span data-stu-id="69aea-115">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="69aea-116">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="69aea-116">allowDeleteChannels</span></span>|<span data-ttu-id="69aea-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="69aea-117">Boolean</span></span>|<span data-ttu-id="69aea-118">Se definido como true, os membros podem excluir canais.</span><span class="sxs-lookup"><span data-stu-id="69aea-118">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="69aea-119">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="69aea-119">allowAddRemoveApps</span></span>|<span data-ttu-id="69aea-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="69aea-120">Boolean</span></span>|<span data-ttu-id="69aea-121">Se definido como true, os membros podem adicionar e remover aplicativos.</span><span class="sxs-lookup"><span data-stu-id="69aea-121">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="69aea-122">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="69aea-122">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="69aea-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="69aea-123">Boolean</span></span>|<span data-ttu-id="69aea-124">Se definido como true, os membros podem adicionar, atualizar e remover guias.</span><span class="sxs-lookup"><span data-stu-id="69aea-124">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="69aea-125">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="69aea-125">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="69aea-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="69aea-126">Boolean</span></span>|<span data-ttu-id="69aea-127">Se definido como true, os membros podem adicionar, atualizar e remover conectores.</span><span class="sxs-lookup"><span data-stu-id="69aea-127">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69aea-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69aea-128">JSON representation</span></span>

<span data-ttu-id="69aea-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69aea-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreatePrivateChannels": true,
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

