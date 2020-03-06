---
title: Tipo de recurso TableSort
description: Gerencia operações de classificação em objetos Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3772d0063fc19eb3a3c46953d5c85d8085f0a72a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533570"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="35143-103">Tipo de recurso TableSort</span><span class="sxs-lookup"><span data-stu-id="35143-103">TableSort resource type</span></span>

<span data-ttu-id="35143-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35143-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35143-105">Gerencia operações de classificação em objetos Table.</span><span class="sxs-lookup"><span data-stu-id="35143-105">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="35143-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="35143-106">Methods</span></span>

| <span data-ttu-id="35143-107">Método</span><span class="sxs-lookup"><span data-stu-id="35143-107">Method</span></span>           | <span data-ttu-id="35143-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="35143-108">Return Type</span></span>    |<span data-ttu-id="35143-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="35143-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35143-110">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="35143-110">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="35143-111">WorkbookTableSort</span><span class="sxs-lookup"><span data-stu-id="35143-111">WorkbookTableSort</span></span>](tablesort.md) |<span data-ttu-id="35143-112">Leia as propriedades e os relacionamentos do objeto tableSort.</span><span class="sxs-lookup"><span data-stu-id="35143-112">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="35143-113">Apply</span><span class="sxs-lookup"><span data-stu-id="35143-113">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="35143-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35143-114">None</span></span>|<span data-ttu-id="35143-115">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="35143-115">Perform a sort operation.</span></span>|
|[<span data-ttu-id="35143-116">Clear</span><span class="sxs-lookup"><span data-stu-id="35143-116">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="35143-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35143-117">None</span></span>|<span data-ttu-id="35143-p101">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="35143-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="35143-120">Reapply</span><span class="sxs-lookup"><span data-stu-id="35143-120">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="35143-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35143-121">None</span></span>|<span data-ttu-id="35143-122">Reaplica os parâmetros de classificação atuais à tabela.</span><span class="sxs-lookup"><span data-stu-id="35143-122">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="35143-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35143-123">Properties</span></span>
| <span data-ttu-id="35143-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35143-124">Property</span></span>     | <span data-ttu-id="35143-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="35143-125">Type</span></span>   |<span data-ttu-id="35143-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="35143-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35143-127">campos</span><span class="sxs-lookup"><span data-stu-id="35143-127">fields</span></span>|<span data-ttu-id="35143-128">Coleção [WorkbookSortField](sortfield.md)</span><span class="sxs-lookup"><span data-stu-id="35143-128">[WorkbookSortField](sortfield.md) collection</span></span>|<span data-ttu-id="35143-129">Representa as condições atuais usadas para a última classificação da tabela.</span><span class="sxs-lookup"><span data-stu-id="35143-129">Represents the current conditions used to last sort the table.</span></span> <span data-ttu-id="35143-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35143-130">Read-only.</span></span>|
|<span data-ttu-id="35143-131">matchCase</span><span class="sxs-lookup"><span data-stu-id="35143-131">matchCase</span></span>|<span data-ttu-id="35143-132">booliano</span><span class="sxs-lookup"><span data-stu-id="35143-132">boolean</span></span>|<span data-ttu-id="35143-p103">Indica se o uso de maiúsculas ou minúsculas afetou a última classificação da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35143-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="35143-135">method</span><span class="sxs-lookup"><span data-stu-id="35143-135">method</span></span>|<span data-ttu-id="35143-136">string</span><span class="sxs-lookup"><span data-stu-id="35143-136">string</span></span>|<span data-ttu-id="35143-137">Indica o último método de ordenação de caracteres chineses usado para classificar a tabela.</span><span class="sxs-lookup"><span data-stu-id="35143-137">Represents Chinese character ordering method last used to sort the table.</span></span> <span data-ttu-id="35143-138">Os valores possíveis são: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="35143-138">The possible values are: `PinYin`, `StrokeCount`.</span></span> <span data-ttu-id="35143-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35143-139">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35143-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35143-140">JSON representation</span></span>

<span data-ttu-id="35143-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35143-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
