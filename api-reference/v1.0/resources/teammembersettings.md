---
title: tipo de recurso teamMemberSettings
description: Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots na equipe.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d657b8f022395c24d27df56442c164731215a04e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033849"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="3615a-103">tipo de recurso teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="3615a-103">teamMemberSettings resource type</span></span>



<span data-ttu-id="3615a-104">Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots, na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="3615a-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3615a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3615a-105">Properties</span></span>
| <span data-ttu-id="3615a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3615a-106">Property</span></span>     | <span data-ttu-id="3615a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3615a-107">Type</span></span>   |<span data-ttu-id="3615a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3615a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3615a-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="3615a-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="3615a-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="3615a-110">Boolean</span></span>|<span data-ttu-id="3615a-111">Se definido como true, os membros podem adicionar e atualizar canais.</span><span class="sxs-lookup"><span data-stu-id="3615a-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="3615a-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="3615a-112">allowDeleteChannels</span></span>|<span data-ttu-id="3615a-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="3615a-113">Boolean</span></span>|<span data-ttu-id="3615a-114">Se definido como true, os membros podem excluir canais.</span><span class="sxs-lookup"><span data-stu-id="3615a-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="3615a-115">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="3615a-115">allowAddRemoveApps</span></span>|<span data-ttu-id="3615a-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="3615a-116">Boolean</span></span>|<span data-ttu-id="3615a-117">Se definido como true, os membros podem adicionar e remover aplicativos.</span><span class="sxs-lookup"><span data-stu-id="3615a-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="3615a-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="3615a-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="3615a-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="3615a-119">Boolean</span></span>|<span data-ttu-id="3615a-120">Se definido como true, os membros podem adicionar, atualizar e remover guias.</span><span class="sxs-lookup"><span data-stu-id="3615a-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="3615a-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="3615a-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="3615a-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="3615a-122">Boolean</span></span>|<span data-ttu-id="3615a-123">Se definido como true, os membros podem adicionar, atualizar e remover conectores.</span><span class="sxs-lookup"><span data-stu-id="3615a-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3615a-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3615a-124">JSON representation</span></span>

<span data-ttu-id="3615a-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3615a-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
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
