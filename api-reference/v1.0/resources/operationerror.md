---
title: tipo de recurso de operationError
description: Descreve os erros em teamsAsyncOperation.
localization_priority: Normal
ms.openlocfilehash: 22590d7d955cf01385292d2796ad960b1c0ced41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824581"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="9ee3c-103">tipo de recurso de operationError</span><span class="sxs-lookup"><span data-stu-id="9ee3c-103">operationError resource type</span></span>



<span data-ttu-id="9ee3c-104">Descreve os erros em [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="9ee3c-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="9ee3c-105">Propriedades de operationError</span><span class="sxs-lookup"><span data-stu-id="9ee3c-105">operationError Properties</span></span>
| <span data-ttu-id="9ee3c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ee3c-106">Property</span></span>     | <span data-ttu-id="9ee3c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ee3c-107">Type</span></span>   |<span data-ttu-id="9ee3c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ee3c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ee3c-109">código</span><span class="sxs-lookup"><span data-stu-id="9ee3c-109">code</span></span>|<span data-ttu-id="9ee3c-110">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="9ee3c-110">string (readonly)</span></span>|<span data-ttu-id="9ee3c-111">Código de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="9ee3c-111">Operation error code.</span></span>|
|<span data-ttu-id="9ee3c-112">message</span><span class="sxs-lookup"><span data-stu-id="9ee3c-112">message</span></span>|<span data-ttu-id="9ee3c-113">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="9ee3c-113">string (readonly)</span></span>|<span data-ttu-id="9ee3c-114">Mensagem de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="9ee3c-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ee3c-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ee3c-115">JSON representation</span></span>

<span data-ttu-id="9ee3c-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ee3c-116">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
