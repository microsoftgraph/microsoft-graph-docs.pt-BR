---
title: tipo de recurso de teamMemberSettings
description: Configurações para configurar se os membros podem realizar determinadas ações, por exemplo, criam canais e adicionar bots, na equipe de.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: e6fae4d81ac005c1830d5bed9e05a4675e1a8ad0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522641"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="c08a7-103">tipo de recurso de teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="c08a7-103">teamMemberSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c08a7-104">Configurações para configurar se os membros podem realizar determinadas ações, por exemplo, criam canais e adicionar bots, em que a [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="c08a7-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c08a7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c08a7-105">Properties</span></span>
| <span data-ttu-id="c08a7-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c08a7-106">Property</span></span>     | <span data-ttu-id="c08a7-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="c08a7-107">Type</span></span>   |<span data-ttu-id="c08a7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c08a7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c08a7-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="c08a7-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="c08a7-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="c08a7-110">Boolean</span></span>|<span data-ttu-id="c08a7-111">Se definido como true, membros pode adicionar e atualizar os canais.</span><span class="sxs-lookup"><span data-stu-id="c08a7-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="c08a7-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="c08a7-112">allowDeleteChannels</span></span>|<span data-ttu-id="c08a7-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="c08a7-113">Boolean</span></span>|<span data-ttu-id="c08a7-114">Se definido como true, membros pode excluir canais.</span><span class="sxs-lookup"><span data-stu-id="c08a7-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="c08a7-115">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="c08a7-115">allowAddRemoveApps</span></span>|<span data-ttu-id="c08a7-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="c08a7-116">Boolean</span></span>|<span data-ttu-id="c08a7-117">Se definido como true, membros pode adicionar e remover aplicativos.</span><span class="sxs-lookup"><span data-stu-id="c08a7-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="c08a7-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="c08a7-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="c08a7-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="c08a7-119">Boolean</span></span>|<span data-ttu-id="c08a7-120">Se definido como true, membros pode adicionar, atualizar e remover guias.</span><span class="sxs-lookup"><span data-stu-id="c08a7-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="c08a7-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="c08a7-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="c08a7-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="c08a7-122">Boolean</span></span>|<span data-ttu-id="c08a7-123">Se definido como true, membros pode adicionar, atualizar e remover conectores.</span><span class="sxs-lookup"><span data-stu-id="c08a7-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c08a7-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c08a7-124">JSON representation</span></span>

<span data-ttu-id="c08a7-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c08a7-125">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/teammembersettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
