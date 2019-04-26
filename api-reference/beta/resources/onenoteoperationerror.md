---
title: tipo de recurso onenoteOperationError
description: Um erro de uma operação do OneNote com falha.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 8b2912ee02ab22631224b892a09a8c4dd7840dd1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341405"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="6dd07-103">tipo de recurso onenoteOperationError</span><span class="sxs-lookup"><span data-stu-id="6dd07-103">onenoteOperationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dd07-104">Um erro de uma operação do OneNote com falha.</span><span class="sxs-lookup"><span data-stu-id="6dd07-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6dd07-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6dd07-105">JSON representation</span></span>

<span data-ttu-id="6dd07-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6dd07-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="6dd07-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6dd07-107">Properties</span></span>
| <span data-ttu-id="6dd07-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6dd07-108">Property</span></span>     | <span data-ttu-id="6dd07-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6dd07-109">Type</span></span>   |<span data-ttu-id="6dd07-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dd07-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6dd07-111">código</span><span class="sxs-lookup"><span data-stu-id="6dd07-111">code</span></span>|<span data-ttu-id="6dd07-112">string</span><span class="sxs-lookup"><span data-stu-id="6dd07-112">string</span></span>|<span data-ttu-id="6dd07-113">O código de erro.</span><span class="sxs-lookup"><span data-stu-id="6dd07-113">The error code.</span></span>|
|<span data-ttu-id="6dd07-114">mensagem</span><span class="sxs-lookup"><span data-stu-id="6dd07-114">message</span></span>|<span data-ttu-id="6dd07-115">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6dd07-115">string</span></span>|<span data-ttu-id="6dd07-116">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="6dd07-116">The error message.</span></span>|

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
