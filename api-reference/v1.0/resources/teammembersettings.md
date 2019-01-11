---
title: tipo de recurso de teamMemberSettings
description: Configurações para configurar se os membros podem realizar determinadas ações, por exemplo, criam canais e adicionar bots, na equipe de.
localization_priority: Normal
ms.openlocfilehash: 7b63bce5bc298f7d9599d8c6146d7962d319c79f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826065"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="abfc7-103">tipo de recurso de teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="abfc7-103">teamMemberSettings resource type</span></span>



<span data-ttu-id="abfc7-104">Configurações para configurar se os membros podem realizar determinadas ações, por exemplo, criam canais e adicionar bots, em que a [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="abfc7-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="abfc7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="abfc7-105">Properties</span></span>
| <span data-ttu-id="abfc7-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abfc7-106">Property</span></span>     | <span data-ttu-id="abfc7-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="abfc7-107">Type</span></span>   |<span data-ttu-id="abfc7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="abfc7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abfc7-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="abfc7-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="abfc7-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="abfc7-110">Boolean</span></span>|<span data-ttu-id="abfc7-111">Se definido como true, membros pode adicionar e atualizar os canais.</span><span class="sxs-lookup"><span data-stu-id="abfc7-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="abfc7-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="abfc7-112">allowDeleteChannels</span></span>|<span data-ttu-id="abfc7-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="abfc7-113">Boolean</span></span>|<span data-ttu-id="abfc7-114">Se definido como true, membros pode excluir canais.</span><span class="sxs-lookup"><span data-stu-id="abfc7-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="abfc7-115">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="abfc7-115">allowAddRemoveApps</span></span>|<span data-ttu-id="abfc7-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="abfc7-116">Boolean</span></span>|<span data-ttu-id="abfc7-117">Se definido como true, membros pode adicionar e remover aplicativos.</span><span class="sxs-lookup"><span data-stu-id="abfc7-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="abfc7-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="abfc7-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="abfc7-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="abfc7-119">Boolean</span></span>|<span data-ttu-id="abfc7-120">Se definido como true, membros pode adicionar, atualizar e remover guias.</span><span class="sxs-lookup"><span data-stu-id="abfc7-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="abfc7-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="abfc7-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="abfc7-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="abfc7-122">Boolean</span></span>|<span data-ttu-id="abfc7-123">Se definido como true, membros pode adicionar, atualizar e remover conectores.</span><span class="sxs-lookup"><span data-stu-id="abfc7-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="abfc7-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="abfc7-124">JSON representation</span></span>

<span data-ttu-id="abfc7-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="abfc7-125">The following is a JSON representation of the resource.</span></span>

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
