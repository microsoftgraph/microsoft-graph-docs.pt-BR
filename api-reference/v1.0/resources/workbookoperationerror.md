---
title: tipo de recurso workbookOperationError
description: Representa um erro de uma operação de pasta de trabalho com falha.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ce65847d6ddbb0a8db0c1277e38753ecab7080e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015138"
---
# <a name="workbookoperationerror-resource-type"></a><span data-ttu-id="2e70e-103">tipo de recurso workbookOperationError</span><span class="sxs-lookup"><span data-stu-id="2e70e-103">workbookOperationError resource type</span></span>

<span data-ttu-id="2e70e-104">Representa um erro de uma operação de pasta de trabalho com falha.</span><span class="sxs-lookup"><span data-stu-id="2e70e-104">Represents an error from a failed workbook operation.</span></span>

## <a name="properties"></a><span data-ttu-id="2e70e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2e70e-105">Properties</span></span>

| <span data-ttu-id="2e70e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e70e-106">Property</span></span>     | <span data-ttu-id="2e70e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e70e-107">Type</span></span>        | <span data-ttu-id="2e70e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e70e-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2e70e-109">código</span><span class="sxs-lookup"><span data-stu-id="2e70e-109">code</span></span>|<span data-ttu-id="2e70e-110">String</span><span class="sxs-lookup"><span data-stu-id="2e70e-110">String</span></span>| <span data-ttu-id="2e70e-111">O código de erro.</span><span class="sxs-lookup"><span data-stu-id="2e70e-111">The error code.</span></span>|
|<span data-ttu-id="2e70e-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="2e70e-112">message</span></span>|<span data-ttu-id="2e70e-113">String</span><span class="sxs-lookup"><span data-stu-id="2e70e-113">String</span></span>| <span data-ttu-id="2e70e-114">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="2e70e-114">The error message.</span></span>|
|<span data-ttu-id="2e70e-115">innererror</span><span class="sxs-lookup"><span data-stu-id="2e70e-115">innererror</span></span>|<span data-ttu-id="2e70e-116">error object</span><span class="sxs-lookup"><span data-stu-id="2e70e-116">error object</span></span>| <span data-ttu-id="2e70e-p101">Opcional. Objetos error adicionais que podem ser mais específicos do que o erro de nível superior.</span><span class="sxs-lookup"><span data-stu-id="2e70e-p101">Optional. Additional error objects that may be more specific than the top level error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e70e-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2e70e-119">JSON representation</span></span>

<span data-ttu-id="2e70e-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2e70e-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperationError",
  "baseType": null
}-->

```json
{
  "code": "String",
  "message": "String",
  "innererror": { "@odata.type": "odata.error" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

