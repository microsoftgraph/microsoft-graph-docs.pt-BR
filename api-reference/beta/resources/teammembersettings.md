---
title: tipo de recurso teamMemberSettings
description: Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots na equipe.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 33f1930096ff63968db39e06ddec26c53ae8bcc9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341719"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="fe56f-103">tipo de recurso teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="fe56f-103">teamMemberSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe56f-104">Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots, na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="fe56f-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fe56f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fe56f-105">Properties</span></span>
| <span data-ttu-id="fe56f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe56f-106">Property</span></span>     | <span data-ttu-id="fe56f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe56f-107">Type</span></span>   |<span data-ttu-id="fe56f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe56f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe56f-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="fe56f-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="fe56f-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe56f-110">Boolean</span></span>|<span data-ttu-id="fe56f-111">Se definido como true, os membros podem adicionar e atualizar canais.</span><span class="sxs-lookup"><span data-stu-id="fe56f-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="fe56f-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="fe56f-112">allowDeleteChannels</span></span>|<span data-ttu-id="fe56f-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe56f-113">Boolean</span></span>|<span data-ttu-id="fe56f-114">Se definido como true, os membros podem excluir canais.</span><span class="sxs-lookup"><span data-stu-id="fe56f-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="fe56f-115">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="fe56f-115">allowAddRemoveApps</span></span>|<span data-ttu-id="fe56f-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe56f-116">Boolean</span></span>|<span data-ttu-id="fe56f-117">Se definido como true, os membros podem adicionar e remover aplicativos.</span><span class="sxs-lookup"><span data-stu-id="fe56f-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="fe56f-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="fe56f-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="fe56f-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe56f-119">Boolean</span></span>|<span data-ttu-id="fe56f-120">Se definido como true, os membros podem adicionar, atualizar e remover guias.</span><span class="sxs-lookup"><span data-stu-id="fe56f-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="fe56f-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="fe56f-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="fe56f-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe56f-122">Boolean</span></span>|<span data-ttu-id="fe56f-123">Se definido como true, os membros podem adicionar, atualizar e remover conectores.</span><span class="sxs-lookup"><span data-stu-id="fe56f-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe56f-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fe56f-124">JSON representation</span></span>

<span data-ttu-id="fe56f-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fe56f-125">The following is a JSON representation of the resource.</span></span>

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
