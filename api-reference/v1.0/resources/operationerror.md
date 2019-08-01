---
title: tipo de recurso operationError
description: Descreve erros no teamsAsyncOperation.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8a46943fad974c2e7a12041e9def6a8a6ad6c9a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035711"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="75772-103">tipo de recurso operationError</span><span class="sxs-lookup"><span data-stu-id="75772-103">operationError resource type</span></span>



<span data-ttu-id="75772-104">Descreve erros no [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="75772-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="75772-105">Propriedades operationError</span><span class="sxs-lookup"><span data-stu-id="75772-105">operationError Properties</span></span>
| <span data-ttu-id="75772-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75772-106">Property</span></span>     | <span data-ttu-id="75772-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="75772-107">Type</span></span>   |<span data-ttu-id="75772-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="75772-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75772-109">código</span><span class="sxs-lookup"><span data-stu-id="75772-109">code</span></span>|<span data-ttu-id="75772-110">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="75772-110">string (readonly)</span></span>|<span data-ttu-id="75772-111">Código de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="75772-111">Operation error code.</span></span>|
|<span data-ttu-id="75772-112">message</span><span class="sxs-lookup"><span data-stu-id="75772-112">message</span></span>|<span data-ttu-id="75772-113">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="75772-113">string (readonly)</span></span>|<span data-ttu-id="75772-114">Mensagem de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="75772-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75772-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75772-115">JSON representation</span></span>

<span data-ttu-id="75772-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75772-116">The following is a JSON representation of the resource.</span></span>

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
