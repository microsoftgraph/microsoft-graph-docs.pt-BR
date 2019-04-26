---
title: tipo de recurso operationError
description: Descreve erros no teamsAsyncOperation.
localization_priority: Normal
ms.openlocfilehash: 957f1ed2960c33f2e7bc07f79e7f749a3b9f15a5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341756"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="91157-103">tipo de recurso operationError</span><span class="sxs-lookup"><span data-stu-id="91157-103">operationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91157-104">Descreve erros no [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="91157-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="91157-105">Propriedades operationError</span><span class="sxs-lookup"><span data-stu-id="91157-105">operationError Properties</span></span>
| <span data-ttu-id="91157-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91157-106">Property</span></span>     | <span data-ttu-id="91157-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="91157-107">Type</span></span>   |<span data-ttu-id="91157-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="91157-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91157-109">código</span><span class="sxs-lookup"><span data-stu-id="91157-109">code</span></span>|<span data-ttu-id="91157-110">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="91157-110">string (readonly)</span></span>|<span data-ttu-id="91157-111">Código de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="91157-111">Operation error code.</span></span>|
|<span data-ttu-id="91157-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="91157-112">message</span></span>|<span data-ttu-id="91157-113">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="91157-113">string (readonly)</span></span>|<span data-ttu-id="91157-114">Mensagem de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="91157-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91157-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91157-115">JSON representation</span></span>

<span data-ttu-id="91157-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91157-116">The following is a JSON representation of the resource.</span></span>

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
