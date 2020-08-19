---
title: tipo de recurso operationError
description: Descreve erros no teamsAsyncOperation.
localization_priority: Normal
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6ae6215d00bc573e6c8d004de743b10c0d381e43
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808159"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="7f8bc-103">tipo de recurso operationError</span><span class="sxs-lookup"><span data-stu-id="7f8bc-103">operationError resource type</span></span>

<span data-ttu-id="7f8bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f8bc-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="7f8bc-105">Descreve erros no [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="7f8bc-105">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="7f8bc-106">Propriedades operationError</span><span class="sxs-lookup"><span data-stu-id="7f8bc-106">operationError Properties</span></span>
| <span data-ttu-id="7f8bc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f8bc-107">Property</span></span>     | <span data-ttu-id="7f8bc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f8bc-108">Type</span></span>   |<span data-ttu-id="7f8bc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f8bc-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f8bc-110">código</span><span class="sxs-lookup"><span data-stu-id="7f8bc-110">code</span></span>|<span data-ttu-id="7f8bc-111">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="7f8bc-111">string (readonly)</span></span>|<span data-ttu-id="7f8bc-112">Código de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="7f8bc-112">Operation error code.</span></span>|
|<span data-ttu-id="7f8bc-113">message</span><span class="sxs-lookup"><span data-stu-id="7f8bc-113">message</span></span>|<span data-ttu-id="7f8bc-114">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="7f8bc-114">string (readonly)</span></span>|<span data-ttu-id="7f8bc-115">Mensagem de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="7f8bc-115">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f8bc-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f8bc-116">JSON representation</span></span>

<span data-ttu-id="7f8bc-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f8bc-117">The following is a JSON representation of the resource.</span></span>

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
