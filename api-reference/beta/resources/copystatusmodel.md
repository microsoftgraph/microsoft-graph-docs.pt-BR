---
title: tipo de recurso de copyStatusModel
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: bf1a88b74f38f21f89b089b31ea5b6e7b6af9f0b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521121"
---
# <a name="copystatusmodel-resource-type"></a><span data-ttu-id="e9439-103">tipo de recurso de copyStatusModel</span><span class="sxs-lookup"><span data-stu-id="e9439-103">copyStatusModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="e9439-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e9439-104">JSON representation</span></span>

<span data-ttu-id="e9439-105">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e9439-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.copystatusmodel"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "string",
  "status": "string"
}

```
## <a name="properties"></a><span data-ttu-id="e9439-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e9439-106">Properties</span></span>
| <span data-ttu-id="e9439-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9439-107">Property</span></span>     | <span data-ttu-id="e9439-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9439-108">Type</span></span>   |<span data-ttu-id="e9439-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9439-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9439-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e9439-110">createdDateTime</span></span>| <span data-ttu-id="e9439-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9439-111">DateTimeOffset</span></span> ||
|<span data-ttu-id="e9439-112">id</span><span class="sxs-lookup"><span data-stu-id="e9439-112">id</span></span>|<span data-ttu-id="e9439-113">string</span><span class="sxs-lookup"><span data-stu-id="e9439-113">string</span></span>||
|<span data-ttu-id="e9439-114">status</span><span class="sxs-lookup"><span data-stu-id="e9439-114">status</span></span>|<span data-ttu-id="e9439-115">string</span><span class="sxs-lookup"><span data-stu-id="e9439-115">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "copyStatusModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/copystatusmodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
