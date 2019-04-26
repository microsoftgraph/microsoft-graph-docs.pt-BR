---
title: tipo de recurso teamMemberSettings
description: Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots na equipe.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: e6fae4d81ac005c1830d5bed9e05a4675e1a8ad0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558038"
---
# <a name="teammembersettings-resource-type"></a><span data-ttu-id="ccf79-103">tipo de recurso teamMemberSettings</span><span class="sxs-lookup"><span data-stu-id="ccf79-103">teamMemberSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccf79-104">Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots, na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="ccf79-104">Settings to configure whether members can perform certain actions, for example, create channels and add bots, in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ccf79-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ccf79-105">Properties</span></span>
| <span data-ttu-id="ccf79-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccf79-106">Property</span></span>     | <span data-ttu-id="ccf79-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccf79-107">Type</span></span>   |<span data-ttu-id="ccf79-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccf79-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ccf79-109">allowCreateUpdateChannels</span><span class="sxs-lookup"><span data-stu-id="ccf79-109">allowCreateUpdateChannels</span></span>|<span data-ttu-id="ccf79-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="ccf79-110">Boolean</span></span>|<span data-ttu-id="ccf79-111">Se definido como true, os membros podem adicionar e atualizar canais.</span><span class="sxs-lookup"><span data-stu-id="ccf79-111">If set to true, members can add and update channels.</span></span>|
|<span data-ttu-id="ccf79-112">allowDeleteChannels</span><span class="sxs-lookup"><span data-stu-id="ccf79-112">allowDeleteChannels</span></span>|<span data-ttu-id="ccf79-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="ccf79-113">Boolean</span></span>|<span data-ttu-id="ccf79-114">Se definido como true, os membros podem excluir canais.</span><span class="sxs-lookup"><span data-stu-id="ccf79-114">If set to true, members can delete channels.</span></span>|
|<span data-ttu-id="ccf79-115">allowAddRemoveApps</span><span class="sxs-lookup"><span data-stu-id="ccf79-115">allowAddRemoveApps</span></span>|<span data-ttu-id="ccf79-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="ccf79-116">Boolean</span></span>|<span data-ttu-id="ccf79-117">Se definido como true, os membros podem adicionar e remover aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ccf79-117">If set to true, members can add and remove apps.</span></span>|
|<span data-ttu-id="ccf79-118">allowCreateUpdateRemoveTabs</span><span class="sxs-lookup"><span data-stu-id="ccf79-118">allowCreateUpdateRemoveTabs</span></span>|<span data-ttu-id="ccf79-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="ccf79-119">Boolean</span></span>|<span data-ttu-id="ccf79-120">Se definido como true, os membros podem adicionar, atualizar e remover guias.</span><span class="sxs-lookup"><span data-stu-id="ccf79-120">If set to true, members can add, update, and remove tabs.</span></span> |
|<span data-ttu-id="ccf79-121">allowCreateUpdateRemoveConnectors</span><span class="sxs-lookup"><span data-stu-id="ccf79-121">allowCreateUpdateRemoveConnectors</span></span>|<span data-ttu-id="ccf79-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="ccf79-122">Boolean</span></span>|<span data-ttu-id="ccf79-123">Se definido como true, os membros podem adicionar, atualizar e remover conectores.</span><span class="sxs-lookup"><span data-stu-id="ccf79-123">If set to true, members can add, update, and remove connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ccf79-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ccf79-124">JSON representation</span></span>

<span data-ttu-id="ccf79-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ccf79-125">The following is a JSON representation of the resource.</span></span>

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
