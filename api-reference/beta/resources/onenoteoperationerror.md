---
title: Tipo de recurso onenoteOperationError
description: Um erro de uma operação do OneNote que falhou.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 78e0ab763f27d17cf926795459b4e4a25cdf8e71
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522053"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="bd23c-103">Tipo de recurso onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="bd23c-103">onenoteOperationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd23c-104">Um erro de uma operação do OneNote que falhou.</span><span class="sxs-lookup"><span data-stu-id="bd23c-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd23c-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bd23c-105">JSON representation</span></span>

<span data-ttu-id="bd23c-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bd23c-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperationError"
}-->

```json
{
  "code": "string",
  "message": "string"
}

```
## <a name="properties"></a><span data-ttu-id="bd23c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bd23c-107">Properties</span></span>
| <span data-ttu-id="bd23c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd23c-108">Property</span></span>     | <span data-ttu-id="bd23c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd23c-109">Type</span></span>   |<span data-ttu-id="bd23c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd23c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd23c-111">código</span><span class="sxs-lookup"><span data-stu-id="bd23c-111">code</span></span>|<span data-ttu-id="bd23c-112">string</span><span class="sxs-lookup"><span data-stu-id="bd23c-112">string</span></span>|<span data-ttu-id="bd23c-113">O código do erro.</span><span class="sxs-lookup"><span data-stu-id="bd23c-113">The error code.</span></span>|
|<span data-ttu-id="bd23c-114">message</span><span class="sxs-lookup"><span data-stu-id="bd23c-114">message</span></span>|<span data-ttu-id="bd23c-115">string</span><span class="sxs-lookup"><span data-stu-id="bd23c-115">string</span></span>|<span data-ttu-id="bd23c-116">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="bd23c-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteoperationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
