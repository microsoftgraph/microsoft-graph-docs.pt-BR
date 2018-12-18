---
title: Tipo de recurso onenoteOperationError
description: Um erro de uma operação do OneNote que falhou.
author: Jewan-microsoft
ms.openlocfilehash: e31d47f9351a050eef134cde2f6a6a8bbdf526d7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320689"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="a35bf-103">Tipo de recurso onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="a35bf-103">onenoteOperationError resource type</span></span>

<span data-ttu-id="a35bf-104">Um erro de uma operação do OneNote que falhou.</span><span class="sxs-lookup"><span data-stu-id="a35bf-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a35bf-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a35bf-105">JSON representation</span></span>

<span data-ttu-id="a35bf-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a35bf-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a35bf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a35bf-107">Properties</span></span>
| <span data-ttu-id="a35bf-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a35bf-108">Property</span></span>     | <span data-ttu-id="a35bf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a35bf-109">Type</span></span>   |<span data-ttu-id="a35bf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a35bf-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a35bf-111">código</span><span class="sxs-lookup"><span data-stu-id="a35bf-111">code</span></span>|<span data-ttu-id="a35bf-112">string</span><span class="sxs-lookup"><span data-stu-id="a35bf-112">string</span></span>|<span data-ttu-id="a35bf-113">O código do erro.</span><span class="sxs-lookup"><span data-stu-id="a35bf-113">The error code.</span></span>|
|<span data-ttu-id="a35bf-114">message</span><span class="sxs-lookup"><span data-stu-id="a35bf-114">message</span></span>|<span data-ttu-id="a35bf-115">string</span><span class="sxs-lookup"><span data-stu-id="a35bf-115">string</span></span>|<span data-ttu-id="a35bf-116">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="a35bf-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
