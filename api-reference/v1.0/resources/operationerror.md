---
title: tipo de recurso de operationError
description: Descreve os erros em teamsAsyncOperation.
ms.openlocfilehash: bcd8c989c4c69336165ef1ca29e1d114d524aa9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006413"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="201b0-103">tipo de recurso de operationError</span><span class="sxs-lookup"><span data-stu-id="201b0-103">operationError resource type</span></span>



<span data-ttu-id="201b0-104">Descreve os erros em [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="201b0-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="201b0-105">Propriedades de operationError</span><span class="sxs-lookup"><span data-stu-id="201b0-105">operationError Properties</span></span>
| <span data-ttu-id="201b0-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="201b0-106">Property</span></span>     | <span data-ttu-id="201b0-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="201b0-107">Type</span></span>   |<span data-ttu-id="201b0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="201b0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="201b0-109">código</span><span class="sxs-lookup"><span data-stu-id="201b0-109">code</span></span>|<span data-ttu-id="201b0-110">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="201b0-110">string (readonly)</span></span>|<span data-ttu-id="201b0-111">Código de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="201b0-111">Operation error code.</span></span>|
|<span data-ttu-id="201b0-112">message</span><span class="sxs-lookup"><span data-stu-id="201b0-112">message</span></span>|<span data-ttu-id="201b0-113">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="201b0-113">string (readonly)</span></span>|<span data-ttu-id="201b0-114">Mensagem de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="201b0-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="201b0-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="201b0-115">JSON representation</span></span>

<span data-ttu-id="201b0-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="201b0-116">The following is a JSON representation of the resource.</span></span>

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
