---
title: tipo de recurso workbookTableSort
description: Gerencia operações de classificação em objetos Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 422c1836317d7299b2e485d578561dda6e1bab91
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519110"
---
# <a name="workbooktablesort-resource-type"></a><span data-ttu-id="396cb-103">tipo de recurso workbookTableSort</span><span class="sxs-lookup"><span data-stu-id="396cb-103">workbookTableSort resource type</span></span>

<span data-ttu-id="396cb-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="396cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="396cb-105">Gerencia operações de classificação em objetos Table.</span><span class="sxs-lookup"><span data-stu-id="396cb-105">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="396cb-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="396cb-106">Methods</span></span>

| <span data-ttu-id="396cb-107">Método</span><span class="sxs-lookup"><span data-stu-id="396cb-107">Method</span></span>           | <span data-ttu-id="396cb-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="396cb-108">Return Type</span></span>    |<span data-ttu-id="396cb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="396cb-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="396cb-110">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="396cb-110">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="396cb-111">workbookTableSort</span><span class="sxs-lookup"><span data-stu-id="396cb-111">workbookTableSort</span></span>](workbooktablesort.md) |<span data-ttu-id="396cb-112">Leia as propriedades e os relacionamentos do objeto tableSort.</span><span class="sxs-lookup"><span data-stu-id="396cb-112">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="396cb-113">Apply</span><span class="sxs-lookup"><span data-stu-id="396cb-113">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="396cb-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="396cb-114">None</span></span>|<span data-ttu-id="396cb-115">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="396cb-115">Perform a sort operation.</span></span>|
|[<span data-ttu-id="396cb-116">Clear</span><span class="sxs-lookup"><span data-stu-id="396cb-116">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="396cb-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="396cb-117">None</span></span>|<span data-ttu-id="396cb-p101">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="396cb-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="396cb-120">Reapply</span><span class="sxs-lookup"><span data-stu-id="396cb-120">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="396cb-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="396cb-121">None</span></span>|<span data-ttu-id="396cb-122">Reaplica os parâmetros de classificação atuais à tabela.</span><span class="sxs-lookup"><span data-stu-id="396cb-122">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="396cb-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="396cb-123">Properties</span></span>
| <span data-ttu-id="396cb-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="396cb-124">Property</span></span>     | <span data-ttu-id="396cb-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="396cb-125">Type</span></span>   |<span data-ttu-id="396cb-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="396cb-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="396cb-127">matchCase</span><span class="sxs-lookup"><span data-stu-id="396cb-127">matchCase</span></span>|<span data-ttu-id="396cb-128">booliano</span><span class="sxs-lookup"><span data-stu-id="396cb-128">boolean</span></span>|<span data-ttu-id="396cb-p102">Indica se o uso de maiúsculas ou minúsculas afetou a última classificação da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="396cb-p102">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="396cb-131">method</span><span class="sxs-lookup"><span data-stu-id="396cb-131">method</span></span>|<span data-ttu-id="396cb-132">string</span><span class="sxs-lookup"><span data-stu-id="396cb-132">string</span></span>|<span data-ttu-id="396cb-p103">Indica o último método de ordenação de caracteres chineses usado para classificar a tabela. Os valores possíveis são: `PinYin` e `StrokeCount`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="396cb-p103">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="396cb-136">Relações</span><span class="sxs-lookup"><span data-stu-id="396cb-136">Relationships</span></span>
| <span data-ttu-id="396cb-137">Relação</span><span class="sxs-lookup"><span data-stu-id="396cb-137">Relationship</span></span> | <span data-ttu-id="396cb-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="396cb-138">Type</span></span>   |<span data-ttu-id="396cb-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="396cb-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="396cb-140">campos</span><span class="sxs-lookup"><span data-stu-id="396cb-140">fields</span></span>|[<span data-ttu-id="396cb-141">workbookSortField</span><span class="sxs-lookup"><span data-stu-id="396cb-141">workbookSortField</span></span>](workbooksortfield.md)|<span data-ttu-id="396cb-142">Representa as condições atuais usadas para a última classificação da tabela.</span><span class="sxs-lookup"><span data-stu-id="396cb-142">Represents the current conditions used to last sort the table.</span></span> <span data-ttu-id="396cb-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="396cb-143">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="396cb-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="396cb-144">JSON representation</span></span>

<span data-ttu-id="396cb-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="396cb-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
 
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "id": "string",
  "matchCase": true,
  "method": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
