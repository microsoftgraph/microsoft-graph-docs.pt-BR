---
title: tipo de recurso onenoteOperationError
description: Um erro de uma operação do OneNote com falha.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: ecd1c42ceb278c483601344dd28c72f7436b9537
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009346"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="50237-103">tipo de recurso onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="50237-103">onenoteOperationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50237-104">Um erro de uma operação do OneNote com falha.</span><span class="sxs-lookup"><span data-stu-id="50237-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="50237-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50237-105">JSON representation</span></span>

<span data-ttu-id="50237-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50237-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="50237-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50237-107">Properties</span></span>
| <span data-ttu-id="50237-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50237-108">Property</span></span>     | <span data-ttu-id="50237-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="50237-109">Type</span></span>   |<span data-ttu-id="50237-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="50237-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50237-111">código</span><span class="sxs-lookup"><span data-stu-id="50237-111">code</span></span>|<span data-ttu-id="50237-112">string</span><span class="sxs-lookup"><span data-stu-id="50237-112">string</span></span>|<span data-ttu-id="50237-113">O código de erro.</span><span class="sxs-lookup"><span data-stu-id="50237-113">The error code.</span></span>|
|<span data-ttu-id="50237-114">mensagem</span><span class="sxs-lookup"><span data-stu-id="50237-114">message</span></span>|<span data-ttu-id="50237-115">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50237-115">string</span></span>|<span data-ttu-id="50237-116">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="50237-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
