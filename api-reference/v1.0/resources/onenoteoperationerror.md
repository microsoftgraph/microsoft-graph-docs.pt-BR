---
title: Tipo de recurso onenoteOperationError
description: Um erro de uma operação do OneNote que falhou.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: df0bfd768d26c751a303f42e1f1123b863388faa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837335"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="805c6-103">Tipo de recurso onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="805c6-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="805c6-104">Um erro de uma operação do OneNote que falhou.</span><span class="sxs-lookup"><span data-stu-id="805c6-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="805c6-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="805c6-105">JSON representation</span></span>

<span data-ttu-id="805c6-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="805c6-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="805c6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="805c6-107">Properties</span></span>
| <span data-ttu-id="805c6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="805c6-108">Property</span></span>     | <span data-ttu-id="805c6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="805c6-109">Type</span></span>   |<span data-ttu-id="805c6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="805c6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="805c6-111">código</span><span class="sxs-lookup"><span data-stu-id="805c6-111">code</span></span>|<span data-ttu-id="805c6-112">string</span><span class="sxs-lookup"><span data-stu-id="805c6-112">string</span></span>|<span data-ttu-id="805c6-113">O código do erro.</span><span class="sxs-lookup"><span data-stu-id="805c6-113">The error code.</span></span>|
|<span data-ttu-id="805c6-114">message</span><span class="sxs-lookup"><span data-stu-id="805c6-114">message</span></span>|<span data-ttu-id="805c6-115">string</span><span class="sxs-lookup"><span data-stu-id="805c6-115">string</span></span>|<span data-ttu-id="805c6-116">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="805c6-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
