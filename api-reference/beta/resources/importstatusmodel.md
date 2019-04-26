---
title: tipo de recurso importStatusModel
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: c3fe64245d0fbce98db3ba87c3c39694e998c7e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548520"
---
# <a name="importstatusmodel-resource-type"></a><span data-ttu-id="412ab-103">tipo de recurso importStatusModel</span><span class="sxs-lookup"><span data-stu-id="412ab-103">importStatusModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="412ab-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="412ab-104">JSON representation</span></span>

<span data-ttu-id="412ab-105">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="412ab-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.importstatusmodel"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "string",
  "status": "string"
}

```
## <a name="properties"></a><span data-ttu-id="412ab-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="412ab-106">Properties</span></span>
| <span data-ttu-id="412ab-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="412ab-107">Property</span></span>     | <span data-ttu-id="412ab-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="412ab-108">Type</span></span>   |<span data-ttu-id="412ab-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="412ab-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="412ab-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="412ab-110">createdDateTime</span></span>| <span data-ttu-id="412ab-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="412ab-111">DateTimeOffset</span></span> ||
|<span data-ttu-id="412ab-112">id</span><span class="sxs-lookup"><span data-stu-id="412ab-112">id</span></span>|<span data-ttu-id="412ab-113">string</span><span class="sxs-lookup"><span data-stu-id="412ab-113">string</span></span>||
|<span data-ttu-id="412ab-114">status</span><span class="sxs-lookup"><span data-stu-id="412ab-114">status</span></span>|<span data-ttu-id="412ab-115">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="412ab-115">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "importStatusModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/importstatusmodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
