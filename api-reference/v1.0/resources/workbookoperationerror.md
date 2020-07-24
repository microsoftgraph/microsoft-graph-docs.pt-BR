---
title: tipo de recurso workbookOperationError
description: Representa um erro de uma operação de pasta de trabalho com falha.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a04d26a7bdeb14f35859e7c1b02e781b64189201
ms.sourcegitcommit: 233ac43db0eb5edd46fe944a5515d7dd9abb1298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45408131"
---
# <a name="workbookoperationerror-resource-type"></a><span data-ttu-id="d3927-103">tipo de recurso workbookOperationError</span><span class="sxs-lookup"><span data-stu-id="d3927-103">workbookOperationError resource type</span></span>

<span data-ttu-id="d3927-104">Representa um erro de uma operação de pasta de trabalho com falha.</span><span class="sxs-lookup"><span data-stu-id="d3927-104">Represents an error from a failed workbook operation.</span></span>

## <a name="properties"></a><span data-ttu-id="d3927-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3927-105">Properties</span></span>

| <span data-ttu-id="d3927-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3927-106">Property</span></span>     | <span data-ttu-id="d3927-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3927-107">Type</span></span>        | <span data-ttu-id="d3927-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3927-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d3927-109">código</span><span class="sxs-lookup"><span data-stu-id="d3927-109">code</span></span>|<span data-ttu-id="d3927-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3927-110">String</span></span>| <span data-ttu-id="d3927-111">O código de erro.</span><span class="sxs-lookup"><span data-stu-id="d3927-111">The error code.</span></span>|
|<span data-ttu-id="d3927-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="d3927-112">message</span></span>|<span data-ttu-id="d3927-113">String</span><span class="sxs-lookup"><span data-stu-id="d3927-113">String</span></span>| <span data-ttu-id="d3927-114">A mensagem de erro.</span><span class="sxs-lookup"><span data-stu-id="d3927-114">The error message.</span></span>|
|<span data-ttu-id="d3927-115">innererror</span><span class="sxs-lookup"><span data-stu-id="d3927-115">innererror</span></span>|<span data-ttu-id="d3927-116">error object</span><span class="sxs-lookup"><span data-stu-id="d3927-116">error object</span></span>| <span data-ttu-id="d3927-p101">Opcional. Objetos error adicionais que podem ser mais específicos do que o erro de nível superior.</span><span class="sxs-lookup"><span data-stu-id="d3927-p101">Optional. Additional error objects that may be more specific than the top level error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3927-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3927-119">JSON representation</span></span>

<span data-ttu-id="d3927-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3927-120">The following is a JSON representation of the resource.</span></span>

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
