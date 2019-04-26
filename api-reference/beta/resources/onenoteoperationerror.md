---
title: tipo de recurso onenoteOperationError
description: Um erro de uma operação do OneNote com falha.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 78e0ab763f27d17cf926795459b4e4a25cdf8e71
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568879"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="5ef8b-103">tipo de recurso onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="5ef8b-103">onenoteOperationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ef8b-104">Um erro de uma operação do OneNote com falha.</span><span class="sxs-lookup"><span data-stu-id="5ef8b-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ef8b-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ef8b-105">JSON representation</span></span>

<span data-ttu-id="5ef8b-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ef8b-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="5ef8b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ef8b-107">Properties</span></span>
| <span data-ttu-id="5ef8b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ef8b-108">Property</span></span>     | <span data-ttu-id="5ef8b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ef8b-109">Type</span></span>   |<span data-ttu-id="5ef8b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ef8b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ef8b-111">código</span><span class="sxs-lookup"><span data-stu-id="5ef8b-111">code</span></span>|<span data-ttu-id="5ef8b-112">string</span><span class="sxs-lookup"><span data-stu-id="5ef8b-112">string</span></span>|<span data-ttu-id="5ef8b-113">O código de erro.</span><span class="sxs-lookup"><span data-stu-id="5ef8b-113">The error code.</span></span>|
|<span data-ttu-id="5ef8b-114">mensagem</span><span class="sxs-lookup"><span data-stu-id="5ef8b-114">message</span></span>|<span data-ttu-id="5ef8b-115">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ef8b-115">string</span></span>|<span data-ttu-id="5ef8b-116">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="5ef8b-116">The error message.</span></span>|

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
