---
title: tipo de recurso operationError
description: Descreve erros no teamsAsyncOperation.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: billbliss
ms.openlocfilehash: 2419d4230e5618f601a5d8fe0743ec9ef807cf00
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809318"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="ae515-103">tipo de recurso operationError</span><span class="sxs-lookup"><span data-stu-id="ae515-103">operationError resource type</span></span>

<span data-ttu-id="ae515-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae515-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae515-105">Descreve erros no [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ae515-105">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="ae515-106">Propriedades operationError</span><span class="sxs-lookup"><span data-stu-id="ae515-106">operationError Properties</span></span>
| <span data-ttu-id="ae515-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae515-107">Property</span></span>     | <span data-ttu-id="ae515-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae515-108">Type</span></span>   |<span data-ttu-id="ae515-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae515-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae515-110">código</span><span class="sxs-lookup"><span data-stu-id="ae515-110">code</span></span>|<span data-ttu-id="ae515-111">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="ae515-111">string (readonly)</span></span>|<span data-ttu-id="ae515-112">Código de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="ae515-112">Operation error code.</span></span>|
|<span data-ttu-id="ae515-113">message</span><span class="sxs-lookup"><span data-stu-id="ae515-113">message</span></span>|<span data-ttu-id="ae515-114">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="ae515-114">string (readonly)</span></span>|<span data-ttu-id="ae515-115">Mensagem de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="ae515-115">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae515-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae515-116">JSON representation</span></span>

<span data-ttu-id="ae515-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae515-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
