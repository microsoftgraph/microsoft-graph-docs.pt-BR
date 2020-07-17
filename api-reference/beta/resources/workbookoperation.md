---
title: tipo de recurso workbookOperation
description: Representa o status de operações de uma pasta de trabalho de execução longa.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: bd015045b01d0a7f886ecf0f5165a347d76dc061
ms.sourcegitcommit: b469176f49aacbd02cd06838cc7c8d36cf5bc768
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2020
ms.locfileid: "45165119"
---
# <a name="workbookoperation-resource-type"></a><span data-ttu-id="7da3b-103">tipo de recurso workbookOperation</span><span class="sxs-lookup"><span data-stu-id="7da3b-103">workbookOperation resource type</span></span>

<span data-ttu-id="7da3b-104">Representa o status de uma operação de pasta de trabalho de execução longa.</span><span class="sxs-lookup"><span data-stu-id="7da3b-104">Represents the status of a long-running workbook operation.</span></span>

## <a name="methods"></a><span data-ttu-id="7da3b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="7da3b-105">Methods</span></span>

| <span data-ttu-id="7da3b-106">Método</span><span class="sxs-lookup"><span data-stu-id="7da3b-106">Method</span></span>       | <span data-ttu-id="7da3b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7da3b-107">Return Type</span></span> | <span data-ttu-id="7da3b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7da3b-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7da3b-109">Obter workbookOperation</span><span class="sxs-lookup"><span data-stu-id="7da3b-109">Get workbookOperation</span></span>](../api/workbookoperation-get.md) | [<span data-ttu-id="7da3b-110">workbookOperation</span><span class="sxs-lookup"><span data-stu-id="7da3b-110">workbookOperation</span></span>](workbookoperation.md) | <span data-ttu-id="7da3b-111">Recuperar o status de um objeto **workbookOperation** .</span><span class="sxs-lookup"><span data-stu-id="7da3b-111">Retrieve the status of a **workbookOperation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7da3b-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7da3b-112">Properties</span></span>

| <span data-ttu-id="7da3b-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7da3b-113">Property</span></span>     | <span data-ttu-id="7da3b-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="7da3b-114">Type</span></span>        | <span data-ttu-id="7da3b-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="7da3b-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7da3b-116">id</span><span class="sxs-lookup"><span data-stu-id="7da3b-116">id</span></span>|<span data-ttu-id="7da3b-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7da3b-117">String</span></span>| <span data-ttu-id="7da3b-118">A ID da operação. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7da3b-118">The operation id. Read-only.</span></span>|
|<span data-ttu-id="7da3b-119">status</span><span class="sxs-lookup"><span data-stu-id="7da3b-119">status</span></span>|<span data-ttu-id="7da3b-120">String</span><span class="sxs-lookup"><span data-stu-id="7da3b-120">String</span></span>| <span data-ttu-id="7da3b-121">O status atual da operação.</span><span class="sxs-lookup"><span data-stu-id="7da3b-121">The current status of the operation.</span></span> <span data-ttu-id="7da3b-122">Os valores possíveis são: `notStarted`, `running`, `succeeded`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="7da3b-122">Possible values are: `notStarted`, `running`, `succeeded`, `failed`.</span></span>|
|<span data-ttu-id="7da3b-123">erro</span><span class="sxs-lookup"><span data-stu-id="7da3b-123">error</span></span>|[<span data-ttu-id="7da3b-124">workbookOperationError</span><span class="sxs-lookup"><span data-stu-id="7da3b-124">workbookOperationError</span></span>](workbookoperationerror.md)| <span data-ttu-id="7da3b-125">O erro retornado pela operação.</span><span class="sxs-lookup"><span data-stu-id="7da3b-125">The error returned by the operation.</span></span>|
|<span data-ttu-id="7da3b-126">resourceLocation</span><span class="sxs-lookup"><span data-stu-id="7da3b-126">resourceLocation</span></span>|<span data-ttu-id="7da3b-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7da3b-127">String</span></span>| <span data-ttu-id="7da3b-128">O URI do recurso para o resultado.</span><span class="sxs-lookup"><span data-stu-id="7da3b-128">The resource URI for the result.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7da3b-129">Relações</span><span class="sxs-lookup"><span data-stu-id="7da3b-129">Relationships</span></span>

<span data-ttu-id="7da3b-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7da3b-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7da3b-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7da3b-131">JSON representation</span></span>

<span data-ttu-id="7da3b-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7da3b-132">The following is a JSON representation of the resource.</span></span>

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
  "resourceLocation": "String"
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
