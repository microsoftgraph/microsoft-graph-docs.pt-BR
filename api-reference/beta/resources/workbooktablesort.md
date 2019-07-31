---
title: tipo de recurso workbookTableSort
description: Gerencia operações de classificação em objetos Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ea0332f1ad00029cf511f2bc55aca80836e5ef2c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007029"
---
# <a name="workbooktablesort-resource-type"></a><span data-ttu-id="bd6c5-103">tipo de recurso workbookTableSort</span><span class="sxs-lookup"><span data-stu-id="bd6c5-103">workbookTableSort resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd6c5-104">Gerencia operações de classificação em objetos Table.</span><span class="sxs-lookup"><span data-stu-id="bd6c5-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="bd6c5-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="bd6c5-105">Methods</span></span>

| <span data-ttu-id="bd6c5-106">Método</span><span class="sxs-lookup"><span data-stu-id="bd6c5-106">Method</span></span>           | <span data-ttu-id="bd6c5-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bd6c5-107">Return Type</span></span>    |<span data-ttu-id="bd6c5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd6c5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bd6c5-109">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="bd6c5-109">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="bd6c5-110">workbookTableSort</span><span class="sxs-lookup"><span data-stu-id="bd6c5-110">workbookTableSort</span></span>](workbooktablesort.md) |<span data-ttu-id="bd6c5-111">Leia as propriedades e os relacionamentos do objeto tableSort.</span><span class="sxs-lookup"><span data-stu-id="bd6c5-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="bd6c5-112">Apply</span><span class="sxs-lookup"><span data-stu-id="bd6c5-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="bd6c5-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bd6c5-113">None</span></span>|<span data-ttu-id="bd6c5-114">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="bd6c5-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="bd6c5-115">Clear</span><span class="sxs-lookup"><span data-stu-id="bd6c5-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="bd6c5-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bd6c5-116">None</span></span>|<span data-ttu-id="bd6c5-p101">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="bd6c5-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="bd6c5-119">Reapply</span><span class="sxs-lookup"><span data-stu-id="bd6c5-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="bd6c5-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bd6c5-120">None</span></span>|<span data-ttu-id="bd6c5-121">Reaplica os parâmetros de classificação atuais à tabela.</span><span class="sxs-lookup"><span data-stu-id="bd6c5-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="bd6c5-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bd6c5-122">Properties</span></span>
| <span data-ttu-id="bd6c5-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd6c5-123">Property</span></span>     | <span data-ttu-id="bd6c5-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd6c5-124">Type</span></span>   |<span data-ttu-id="bd6c5-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd6c5-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd6c5-126">matchCase</span><span class="sxs-lookup"><span data-stu-id="bd6c5-126">matchCase</span></span>|<span data-ttu-id="bd6c5-127">booliano</span><span class="sxs-lookup"><span data-stu-id="bd6c5-127">boolean</span></span>|<span data-ttu-id="bd6c5-p102">Indica se o uso de maiúsculas ou minúsculas afetou a última classificação da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bd6c5-p102">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="bd6c5-130">method</span><span class="sxs-lookup"><span data-stu-id="bd6c5-130">method</span></span>|<span data-ttu-id="bd6c5-131">string</span><span class="sxs-lookup"><span data-stu-id="bd6c5-131">string</span></span>|<span data-ttu-id="bd6c5-p103">Indica o último método de ordenação de caracteres chineses usado para classificar a tabela. Os valores possíveis são: `PinYin` e `StrokeCount`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bd6c5-p103">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd6c5-135">Relações</span><span class="sxs-lookup"><span data-stu-id="bd6c5-135">Relationships</span></span>
| <span data-ttu-id="bd6c5-136">Relação</span><span class="sxs-lookup"><span data-stu-id="bd6c5-136">Relationship</span></span> | <span data-ttu-id="bd6c5-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd6c5-137">Type</span></span>   |<span data-ttu-id="bd6c5-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd6c5-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd6c5-139">campos</span><span class="sxs-lookup"><span data-stu-id="bd6c5-139">fields</span></span>|[<span data-ttu-id="bd6c5-140">workbookSortField</span><span class="sxs-lookup"><span data-stu-id="bd6c5-140">workbookSortField</span></span>](workbooksortfield.md)|<span data-ttu-id="bd6c5-141">Representa as condições atuais usadas para a última classificação da tabela.</span><span class="sxs-lookup"><span data-stu-id="bd6c5-141">Represents the current conditions used to last sort the table.</span></span> <span data-ttu-id="bd6c5-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bd6c5-142">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bd6c5-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bd6c5-143">JSON representation</span></span>

<span data-ttu-id="bd6c5-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bd6c5-144">Here is a JSON representation of the resource.</span></span>

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
