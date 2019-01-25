---
title: tipo de recurso de operationError
description: Descreve os erros em teamsAsyncOperation.
localization_priority: Normal
ms.openlocfilehash: 1f07fe064d7bbd255f2693071c86842a34fdffa0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526127"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="ec9ff-103">tipo de recurso de operationError</span><span class="sxs-lookup"><span data-stu-id="ec9ff-103">operationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec9ff-104">Descreve os erros em [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ec9ff-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="ec9ff-105">Propriedades de operationError</span><span class="sxs-lookup"><span data-stu-id="ec9ff-105">operationError Properties</span></span>
| <span data-ttu-id="ec9ff-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec9ff-106">Property</span></span>     | <span data-ttu-id="ec9ff-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec9ff-107">Type</span></span>   |<span data-ttu-id="ec9ff-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec9ff-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec9ff-109">código</span><span class="sxs-lookup"><span data-stu-id="ec9ff-109">code</span></span>|<span data-ttu-id="ec9ff-110">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="ec9ff-110">string (readonly)</span></span>|<span data-ttu-id="ec9ff-111">Código de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="ec9ff-111">Operation error code.</span></span>|
|<span data-ttu-id="ec9ff-112">message</span><span class="sxs-lookup"><span data-stu-id="ec9ff-112">message</span></span>|<span data-ttu-id="ec9ff-113">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="ec9ff-113">string (readonly)</span></span>|<span data-ttu-id="ec9ff-114">Mensagem de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="ec9ff-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec9ff-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec9ff-115">JSON representation</span></span>

<span data-ttu-id="ec9ff-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec9ff-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/operationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
