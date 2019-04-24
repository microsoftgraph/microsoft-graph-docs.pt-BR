---
title: tipo de recurso onenoteOperationError
description: Um erro de uma operação do OneNote com falha.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 3291f70e8cc18ee532f636feb1de9e8bb5751e02
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462596"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="c7191-103">tipo de recurso onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="c7191-103">onenoteOperationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7191-104">Um erro de uma operação do OneNote com falha.</span><span class="sxs-lookup"><span data-stu-id="c7191-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7191-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7191-105">JSON representation</span></span>

<span data-ttu-id="c7191-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7191-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="c7191-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7191-107">Properties</span></span>
| <span data-ttu-id="c7191-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7191-108">Property</span></span>     | <span data-ttu-id="c7191-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7191-109">Type</span></span>   |<span data-ttu-id="c7191-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7191-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7191-111">código</span><span class="sxs-lookup"><span data-stu-id="c7191-111">code</span></span>|<span data-ttu-id="c7191-112">string</span><span class="sxs-lookup"><span data-stu-id="c7191-112">string</span></span>|<span data-ttu-id="c7191-113">O código de erro.</span><span class="sxs-lookup"><span data-stu-id="c7191-113">The error code.</span></span>|
|<span data-ttu-id="c7191-114">mensagem</span><span class="sxs-lookup"><span data-stu-id="c7191-114">message</span></span>|<span data-ttu-id="c7191-115">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7191-115">string</span></span>|<span data-ttu-id="c7191-116">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="c7191-116">The error message.</span></span>|

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
