---
title: Tipo de recurso onenoteOperationError
description: Um erro de uma operação do OneNote que falhou.
ms.openlocfilehash: 3e09bd4b4ec0a8fc36113c278ebe7cab25392ecf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003822"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="bd6b1-103">Tipo de recurso onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="bd6b1-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="bd6b1-104">Um erro de uma operação do OneNote que falhou.</span><span class="sxs-lookup"><span data-stu-id="bd6b1-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd6b1-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bd6b1-105">JSON representation</span></span>

<span data-ttu-id="bd6b1-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bd6b1-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="bd6b1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bd6b1-107">Properties</span></span>
| <span data-ttu-id="bd6b1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd6b1-108">Property</span></span>     | <span data-ttu-id="bd6b1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd6b1-109">Type</span></span>   |<span data-ttu-id="bd6b1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd6b1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd6b1-111">código</span><span class="sxs-lookup"><span data-stu-id="bd6b1-111">code</span></span>|<span data-ttu-id="bd6b1-112">string</span><span class="sxs-lookup"><span data-stu-id="bd6b1-112">string</span></span>|<span data-ttu-id="bd6b1-113">O código do erro.</span><span class="sxs-lookup"><span data-stu-id="bd6b1-113">The error code.</span></span>|
|<span data-ttu-id="bd6b1-114">message</span><span class="sxs-lookup"><span data-stu-id="bd6b1-114">message</span></span>|<span data-ttu-id="bd6b1-115">string</span><span class="sxs-lookup"><span data-stu-id="bd6b1-115">string</span></span>|<span data-ttu-id="bd6b1-116">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="bd6b1-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
