---
title: tipo de recurso workbookOperation
description: Representa o status de operações de uma pasta de trabalho de execução longa.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 4fa98cdfdfc013386f7d615c54c832d27c5f826e
ms.sourcegitcommit: 233ac43db0eb5edd46fe944a5515d7dd9abb1298
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45408132"
---
# <a name="workbookoperation-resource-type"></a><span data-ttu-id="3c970-103">tipo de recurso workbookOperation</span><span class="sxs-lookup"><span data-stu-id="3c970-103">workbookOperation resource type</span></span>

<span data-ttu-id="3c970-104">Representa o status de uma operação de pasta de trabalho de execução longa.</span><span class="sxs-lookup"><span data-stu-id="3c970-104">Represents the status of a long-running workbook operation.</span></span>


## <a name="methods"></a><span data-ttu-id="3c970-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="3c970-105">Methods</span></span>

| <span data-ttu-id="3c970-106">Método</span><span class="sxs-lookup"><span data-stu-id="3c970-106">Method</span></span>       | <span data-ttu-id="3c970-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3c970-107">Return Type</span></span> | <span data-ttu-id="3c970-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c970-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3c970-109">Obter workbookOperation</span><span class="sxs-lookup"><span data-stu-id="3c970-109">Get workbookOperation</span></span>](../api/workbookoperation-get.md) | [<span data-ttu-id="3c970-110">workbookOperation</span><span class="sxs-lookup"><span data-stu-id="3c970-110">workbookOperation</span></span>](workbookoperation.md) | <span data-ttu-id="3c970-111">Obtenha a operação com `{operation-id}` .</span><span class="sxs-lookup"><span data-stu-id="3c970-111">Get the operation with `{operation-id}`.</span></span> |


## <a name="properties"></a><span data-ttu-id="3c970-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c970-112">Properties</span></span>

| <span data-ttu-id="3c970-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c970-113">Property</span></span>     | <span data-ttu-id="3c970-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c970-114">Type</span></span>        | <span data-ttu-id="3c970-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c970-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3c970-116">status</span><span class="sxs-lookup"><span data-stu-id="3c970-116">status</span></span>|<span data-ttu-id="3c970-117">String</span><span class="sxs-lookup"><span data-stu-id="3c970-117">String</span></span>| <span data-ttu-id="3c970-118">O status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="3c970-118">The current status of the operation.</span></span> <span data-ttu-id="3c970-119">Os valores possíveis são: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="3c970-119">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="3c970-120">id</span><span class="sxs-lookup"><span data-stu-id="3c970-120">id</span></span>|<span data-ttu-id="3c970-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c970-121">String</span></span>| <span data-ttu-id="3c970-122">A ID da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3c970-122">The operation id. Read-only.</span></span>|
|<span data-ttu-id="3c970-123">erro</span><span class="sxs-lookup"><span data-stu-id="3c970-123">error</span></span>|[<span data-ttu-id="3c970-124">workbookOperationError</span><span class="sxs-lookup"><span data-stu-id="3c970-124">workbookOperationError</span></span>](workbookoperationerror.md)| <span data-ttu-id="3c970-125">O erro retornado pela operação.</span><span class="sxs-lookup"><span data-stu-id="3c970-125">The error returned by the operation.</span></span>|
|<span data-ttu-id="3c970-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="3c970-126">resourceLocation</span></span>|<span data-ttu-id="3c970-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c970-127">String</span></span>| <span data-ttu-id="3c970-128">O URI do recurso para o resultado.</span><span class="sxs-lookup"><span data-stu-id="3c970-128">The resource URI for the result.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c970-129">Relações</span><span class="sxs-lookup"><span data-stu-id="3c970-129">Relationships</span></span>

<span data-ttu-id="3c970-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c970-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c970-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c970-131">JSON representation</span></span>

<span data-ttu-id="3c970-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c970-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperation",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "status": {"@odata.type": "microsoft.graph.workbookOperationStatus"},
  "error": {"@odata.type": "microsoft.graph.workbookOperationError"},
  "resourceLocation": "String",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->