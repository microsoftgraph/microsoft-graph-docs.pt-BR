---
title: tipo de recurso operationError
description: Descreve erros no teamsAsyncOperation.
localization_priority: Normal
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 014112d78b19ee08836139dc39d8d99b8459027b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003021"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="5ae9f-103">tipo de recurso operationError</span><span class="sxs-lookup"><span data-stu-id="5ae9f-103">operationError resource type</span></span>

<span data-ttu-id="5ae9f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ae9f-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="5ae9f-105">Descreve erros no [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="5ae9f-105">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="5ae9f-106">Propriedades operationError</span><span class="sxs-lookup"><span data-stu-id="5ae9f-106">operationError Properties</span></span>
| <span data-ttu-id="5ae9f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ae9f-107">Property</span></span>     | <span data-ttu-id="5ae9f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ae9f-108">Type</span></span>   |<span data-ttu-id="5ae9f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ae9f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ae9f-110">código</span><span class="sxs-lookup"><span data-stu-id="5ae9f-110">code</span></span>|<span data-ttu-id="5ae9f-111">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="5ae9f-111">string (readonly)</span></span>|<span data-ttu-id="5ae9f-112">Código de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="5ae9f-112">Operation error code.</span></span>|
|<span data-ttu-id="5ae9f-113">message</span><span class="sxs-lookup"><span data-stu-id="5ae9f-113">message</span></span>|<span data-ttu-id="5ae9f-114">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="5ae9f-114">string (readonly)</span></span>|<span data-ttu-id="5ae9f-115">Mensagem de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="5ae9f-115">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5ae9f-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ae9f-116">JSON representation</span></span>

<span data-ttu-id="5ae9f-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ae9f-117">The following is a JSON representation of the resource.</span></span>

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

