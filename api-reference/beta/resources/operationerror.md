---
title: tipo de recurso operationError
description: Descreve erros no teamsAsyncOperation.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9026d133e1a58547f5af68c3a5710c5e06399cb6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522148"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="ffbf5-103">tipo de recurso operationError</span><span class="sxs-lookup"><span data-stu-id="ffbf5-103">operationError resource type</span></span>

<span data-ttu-id="ffbf5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ffbf5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffbf5-105">Descreve erros no [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="ffbf5-105">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="ffbf5-106">Propriedades operationError</span><span class="sxs-lookup"><span data-stu-id="ffbf5-106">operationError Properties</span></span>
| <span data-ttu-id="ffbf5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ffbf5-107">Property</span></span>     | <span data-ttu-id="ffbf5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffbf5-108">Type</span></span>   |<span data-ttu-id="ffbf5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffbf5-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ffbf5-110">código</span><span class="sxs-lookup"><span data-stu-id="ffbf5-110">code</span></span>|<span data-ttu-id="ffbf5-111">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="ffbf5-111">string (readonly)</span></span>|<span data-ttu-id="ffbf5-112">Código de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="ffbf5-112">Operation error code.</span></span>|
|<span data-ttu-id="ffbf5-113">message</span><span class="sxs-lookup"><span data-stu-id="ffbf5-113">message</span></span>|<span data-ttu-id="ffbf5-114">cadeia de caracteres (somente leitura)</span><span class="sxs-lookup"><span data-stu-id="ffbf5-114">string (readonly)</span></span>|<span data-ttu-id="ffbf5-115">Mensagem de erro de operação.</span><span class="sxs-lookup"><span data-stu-id="ffbf5-115">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffbf5-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ffbf5-116">JSON representation</span></span>

<span data-ttu-id="ffbf5-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ffbf5-117">The following is a JSON representation of the resource.</span></span>

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
