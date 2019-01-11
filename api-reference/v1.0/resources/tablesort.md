---
title: Tipo de recurso TableSort
description: Gerencia operações de classificação em objetos Table.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: d56d739a51b78ad7fdfd9f5cc8033b544ebb87ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835074"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="8e321-103">Tipo de recurso TableSort</span><span class="sxs-lookup"><span data-stu-id="8e321-103">TableSort resource type</span></span>

<span data-ttu-id="8e321-104">Gerencia operações de classificação em objetos Table.</span><span class="sxs-lookup"><span data-stu-id="8e321-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="8e321-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="8e321-105">Methods</span></span>

| <span data-ttu-id="8e321-106">Método</span><span class="sxs-lookup"><span data-stu-id="8e321-106">Method</span></span>           | <span data-ttu-id="8e321-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8e321-107">Return Type</span></span>    |<span data-ttu-id="8e321-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e321-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8e321-109">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="8e321-109">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="8e321-110">WorkbookTableSort</span><span class="sxs-lookup"><span data-stu-id="8e321-110">WorkbookTableSort</span></span>](tablesort.md) |<span data-ttu-id="8e321-111">Leia as propriedades e os relacionamentos do objeto tableSort.</span><span class="sxs-lookup"><span data-stu-id="8e321-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="8e321-112">Aplicar</span><span class="sxs-lookup"><span data-stu-id="8e321-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="8e321-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e321-113">None</span></span>|<span data-ttu-id="8e321-114">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="8e321-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="8e321-115">Clear</span><span class="sxs-lookup"><span data-stu-id="8e321-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="8e321-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e321-116">None</span></span>|<span data-ttu-id="8e321-p101">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="8e321-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="8e321-119">Reapply</span><span class="sxs-lookup"><span data-stu-id="8e321-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="8e321-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e321-120">None</span></span>|<span data-ttu-id="8e321-121">Reaplica os parâmetros de classificação atuais à tabela.</span><span class="sxs-lookup"><span data-stu-id="8e321-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="8e321-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e321-122">Properties</span></span>
| <span data-ttu-id="8e321-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e321-123">Property</span></span>     | <span data-ttu-id="8e321-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e321-124">Type</span></span>   |<span data-ttu-id="8e321-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e321-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e321-126">campos</span><span class="sxs-lookup"><span data-stu-id="8e321-126">fields</span></span>|<span data-ttu-id="8e321-127">Coleção [WorkbookSortField](sortfield.md)</span><span class="sxs-lookup"><span data-stu-id="8e321-127">[WorkbookSortField](sortfield.md) collection</span></span>|<span data-ttu-id="8e321-p102">Representa as condições atuais usadas para a última classificação da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e321-p102">Represents the current conditions used to last sort the table. Read-only.</span></span>|
|<span data-ttu-id="8e321-130">matchCase</span><span class="sxs-lookup"><span data-stu-id="8e321-130">matchCase</span></span>|<span data-ttu-id="8e321-131">booliano</span><span class="sxs-lookup"><span data-stu-id="8e321-131">boolean</span></span>|<span data-ttu-id="8e321-p103">Indica se o uso de maiúsculas ou minúsculas afetou a última classificação da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e321-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="8e321-134">method</span><span class="sxs-lookup"><span data-stu-id="8e321-134">method</span></span>|<span data-ttu-id="8e321-135">string</span><span class="sxs-lookup"><span data-stu-id="8e321-135">string</span></span>|<span data-ttu-id="8e321-136">Representa caracteres do chinês método última usado para classificar a tabela de pedidos.</span><span class="sxs-lookup"><span data-stu-id="8e321-136">Represents Chinese character ordering method last used to sort the table.</span></span> <span data-ttu-id="8e321-137">Os valores possíveis são: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="8e321-137">The possible values are: `PinYin`, `StrokeCount`.</span></span> <span data-ttu-id="8e321-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e321-138">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8e321-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e321-139">JSON representation</span></span>

<span data-ttu-id="8e321-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e321-140">Here is a JSON representation of the resource.</span></span>

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
