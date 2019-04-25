---
title: tipo de recurso copyStatusModel
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: bf1a88b74f38f21f89b089b31ea5b6e7b6af9f0b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535222"
---
# <a name="copystatusmodel-resource-type"></a><span data-ttu-id="a8532-103">tipo de recurso copyStatusModel</span><span class="sxs-lookup"><span data-stu-id="a8532-103">copyStatusModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="a8532-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8532-104">JSON representation</span></span>

<span data-ttu-id="a8532-105">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8532-105">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a8532-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8532-106">Properties</span></span>
| <span data-ttu-id="a8532-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8532-107">Property</span></span>     | <span data-ttu-id="a8532-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8532-108">Type</span></span>   |<span data-ttu-id="a8532-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8532-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8532-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8532-110">createdDateTime</span></span>| <span data-ttu-id="a8532-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8532-111">DateTimeOffset</span></span> ||
|<span data-ttu-id="a8532-112">id</span><span class="sxs-lookup"><span data-stu-id="a8532-112">id</span></span>|<span data-ttu-id="a8532-113">string</span><span class="sxs-lookup"><span data-stu-id="a8532-113">string</span></span>||
|<span data-ttu-id="a8532-114">status</span><span class="sxs-lookup"><span data-stu-id="a8532-114">status</span></span>|<span data-ttu-id="a8532-115">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8532-115">string</span></span>||

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
