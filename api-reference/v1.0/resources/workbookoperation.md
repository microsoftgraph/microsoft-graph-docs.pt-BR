---
title: tipo de recurso workbookOperation
description: Representa o status de operações de uma longa execução de uma livro de trabalho.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c674186befbb6a24c41cd8741f554876a17a4394
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158944"
---
# <a name="workbookoperation-resource-type"></a><span data-ttu-id="93cf9-103">tipo de recurso workbookOperation</span><span class="sxs-lookup"><span data-stu-id="93cf9-103">workbookOperation resource type</span></span>

<span data-ttu-id="93cf9-104">Representa o status de uma operação de livro de trabalho de execução longa.</span><span class="sxs-lookup"><span data-stu-id="93cf9-104">Represents the status of a long-running workbook operation.</span></span>


## <a name="methods"></a><span data-ttu-id="93cf9-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="93cf9-105">Methods</span></span>

| <span data-ttu-id="93cf9-106">Método</span><span class="sxs-lookup"><span data-stu-id="93cf9-106">Method</span></span>       | <span data-ttu-id="93cf9-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="93cf9-107">Return Type</span></span> | <span data-ttu-id="93cf9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="93cf9-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="93cf9-109">Obter workbookOperation</span><span class="sxs-lookup"><span data-stu-id="93cf9-109">Get workbookOperation</span></span>](../api/workbookoperation-get.md) | [<span data-ttu-id="93cf9-110">workbookOperation</span><span class="sxs-lookup"><span data-stu-id="93cf9-110">workbookOperation</span></span>](workbookoperation.md) | <span data-ttu-id="93cf9-111">Obter a operação com `{operation-id}` .</span><span class="sxs-lookup"><span data-stu-id="93cf9-111">Get the operation with `{operation-id}`.</span></span> |


## <a name="properties"></a><span data-ttu-id="93cf9-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93cf9-112">Properties</span></span>

| <span data-ttu-id="93cf9-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93cf9-113">Property</span></span>     | <span data-ttu-id="93cf9-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="93cf9-114">Type</span></span>        | <span data-ttu-id="93cf9-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="93cf9-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="93cf9-116">status</span><span class="sxs-lookup"><span data-stu-id="93cf9-116">status</span></span>|<span data-ttu-id="93cf9-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93cf9-117">String</span></span>| <span data-ttu-id="93cf9-118">O status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="93cf9-118">The current status of the operation.</span></span> <span data-ttu-id="93cf9-119">Os valores possíveis são: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="93cf9-119">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="93cf9-120">id</span><span class="sxs-lookup"><span data-stu-id="93cf9-120">id</span></span>|<span data-ttu-id="93cf9-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93cf9-121">String</span></span>| <span data-ttu-id="93cf9-122">A ID da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="93cf9-122">The operation id. Read-only.</span></span>|
|<span data-ttu-id="93cf9-123">erro</span><span class="sxs-lookup"><span data-stu-id="93cf9-123">error</span></span>|[<span data-ttu-id="93cf9-124">workbookOperationError</span><span class="sxs-lookup"><span data-stu-id="93cf9-124">workbookOperationError</span></span>](workbookoperationerror.md)| <span data-ttu-id="93cf9-125">O erro retornado pela operação.</span><span class="sxs-lookup"><span data-stu-id="93cf9-125">The error returned by the operation.</span></span>|
|<span data-ttu-id="93cf9-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="93cf9-126">resourceLocation</span></span>|<span data-ttu-id="93cf9-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93cf9-127">String</span></span>| <span data-ttu-id="93cf9-128">O URI do recurso para o resultado.</span><span class="sxs-lookup"><span data-stu-id="93cf9-128">The resource URI for the result.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93cf9-129">Relações</span><span class="sxs-lookup"><span data-stu-id="93cf9-129">Relationships</span></span>

<span data-ttu-id="93cf9-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93cf9-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93cf9-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93cf9-131">JSON representation</span></span>

<span data-ttu-id="93cf9-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93cf9-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperation",
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
