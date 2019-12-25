---
title: tipo de recurso teamMemberSettings
description: Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots na equipe.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1c1485bbc43588b8144cbe1cc7cb189f9b8c9fdc
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863775"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="675b6-103">tipo de recurso teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="675b6-103">teamMemberSettings resource type</span></span>



<span data-ttu-id="675b6-104">Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots, na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="675b6-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="675b6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="675b6-105">Properties</span></span>
| <span data-ttu-id="675b6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="675b6-106">Property</span></span>     | <span data-ttu-id="675b6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="675b6-107">Type</span></span>   |<span data-ttu-id="675b6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="675b6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="675b6-109">allowCreatePrivateChannels</span><span class="sxs-lookup"><span data-stu-id="675b6-109">allowCreatePrivateChannels</span></span>|<span data-ttu-id="675b6-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="675b6-110">Boolean</span></span>|<span data-ttu-id="675b6-111">Se definido como true, os membros podem adicionar e atualizar canais privados.</span><span class="sxs-lookup"><span data-stu-id="675b6-111">If set to true, members can add and update private channels.</span></span>|
|<span data-ttu-id="675b6-112">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="675b6-112">allowCreateUpdateChannels</span></span>|<span data-ttu-id="675b6-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="675b6-113">Boolean</span></span>|<span data-ttu-id="675b6-114">Se definido como true, os membros podem adicionar e atualizar canais.</span><span class="sxs-lookup"><span data-stu-id="675b6-114">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="675b6-115">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="675b6-115">allowDeleteChannels</span></span>|<span data-ttu-id="675b6-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="675b6-116">Boolean</span></span>|<span data-ttu-id="675b6-117">Se definido como true, os membros podem excluir canais.</span><span class="sxs-lookup"><span data-stu-id="675b6-117">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="675b6-118">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="675b6-118">allowAddRemoveApps</span></span>|<span data-ttu-id="675b6-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="675b6-119">Boolean</span></span>|<span data-ttu-id="675b6-120">Se definido como true, os membros podem adicionar e remover aplicativos.</span><span class="sxs-lookup"><span data-stu-id="675b6-120">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="675b6-121">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="675b6-121">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="675b6-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="675b6-122">Boolean</span></span>|<span data-ttu-id="675b6-123">Se definido como true, os membros podem adicionar, atualizar e remover guias.</span><span class="sxs-lookup"><span data-stu-id="675b6-123">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="675b6-124">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="675b6-124">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="675b6-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="675b6-125">Boolean</span></span>|<span data-ttu-id="675b6-126">Se definido como true, os membros podem adicionar, atualizar e remover conectores.</span><span class="sxs-lookup"><span data-stu-id="675b6-126">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="675b6-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="675b6-127">JSON representation</span></span>

<span data-ttu-id="675b6-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="675b6-128">The following is a JSON representation of the resource.</span></span>

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
