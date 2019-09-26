---
title: tipo de recurso teamMemberSettings
description: Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots na equipe.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8967eb083ad2bd413277c42b688c2d0c48d8244b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196256"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="be524-103">tipo de recurso teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="be524-103">teamMemberSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be524-104">Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots, na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="be524-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="be524-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="be524-105">Properties</span></span>
| <span data-ttu-id="be524-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be524-106">Property</span></span>     | <span data-ttu-id="be524-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="be524-107">Type</span></span>   |<span data-ttu-id="be524-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="be524-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be524-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="be524-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="be524-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="be524-110">Boolean</span></span>|<span data-ttu-id="be524-111">Se definido como true, os membros podem adicionar e atualizar qualquer canal.</span><span class="sxs-lookup"><span data-stu-id="be524-111">If set to true, members can add and update any channels.</span></span>|
|<span data-ttu-id="be524-112">allowCreatePrivateChannels</span><span class="sxs-lookup"><span data-stu-id="be524-112">allowCreatePrivateChannels</span></span>|<span data-ttu-id="be524-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="be524-113">Boolean</span></span>|<span data-ttu-id="be524-114">Se definido como true, os membros podem adicionar e atualizar canais privados.</span><span class="sxs-lookup"><span data-stu-id="be524-114">If set to true, members can add and update private channels.</span></span>|
|<span data-ttu-id="be524-115">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="be524-115">allowDeleteChannels</span></span>|<span data-ttu-id="be524-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="be524-116">Boolean</span></span>|<span data-ttu-id="be524-117">Se definido como true, os membros podem excluir canais.</span><span class="sxs-lookup"><span data-stu-id="be524-117">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="be524-118">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="be524-118">allowAddRemoveApps</span></span>|<span data-ttu-id="be524-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="be524-119">Boolean</span></span>|<span data-ttu-id="be524-120">Se definido como true, os membros podem adicionar e remover aplicativos.</span><span class="sxs-lookup"><span data-stu-id="be524-120">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="be524-121">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="be524-121">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="be524-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="be524-122">Boolean</span></span>|<span data-ttu-id="be524-123">Se definido como true, os membros podem adicionar, atualizar e remover guias.</span><span class="sxs-lookup"><span data-stu-id="be524-123">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="be524-124">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="be524-124">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="be524-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="be524-125">Boolean</span></span>|<span data-ttu-id="be524-126">Se definido como true, os membros podem adicionar, atualizar e remover conectores.</span><span class="sxs-lookup"><span data-stu-id="be524-126">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be524-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="be524-127">JSON representation</span></span>

<span data-ttu-id="be524-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="be524-128">The following is a JSON representation of the resource.</span></span>

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
