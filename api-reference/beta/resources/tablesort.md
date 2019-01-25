---
title: Tipo de recurso TableSort
description: Gerencia operações de classificação em objetos Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 612e0cb7d59011f04ae992f80119fc1da572b582
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511741"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="fa9ae-103">Tipo de recurso TableSort</span><span class="sxs-lookup"><span data-stu-id="fa9ae-103">TableSort resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa9ae-104">Gerencia operações de classificação em objetos Table.</span><span class="sxs-lookup"><span data-stu-id="fa9ae-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="fa9ae-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="fa9ae-105">Methods</span></span>

| <span data-ttu-id="fa9ae-106">Método</span><span class="sxs-lookup"><span data-stu-id="fa9ae-106">Method</span></span>           | <span data-ttu-id="fa9ae-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fa9ae-107">Return Type</span></span>    |<span data-ttu-id="fa9ae-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa9ae-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa9ae-109">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="fa9ae-109">[Get TableSort](../api/tablesort-get.md)</span></span> | [<span data-ttu-id="fa9ae-110">TableSort</span><span class="sxs-lookup"><span data-stu-id="fa9ae-110">TableSort</span></span>](tablesort.md) |<span data-ttu-id="fa9ae-111">Leia as propriedades e os relacionamentos do objeto tableSort.</span><span class="sxs-lookup"><span data-stu-id="fa9ae-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="fa9ae-112">Aplicar</span><span class="sxs-lookup"><span data-stu-id="fa9ae-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="fa9ae-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fa9ae-113">None</span></span>|<span data-ttu-id="fa9ae-114">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="fa9ae-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="fa9ae-115">Clear</span><span class="sxs-lookup"><span data-stu-id="fa9ae-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="fa9ae-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fa9ae-116">None</span></span>|<span data-ttu-id="fa9ae-p101">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="fa9ae-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="fa9ae-119">Reapply</span><span class="sxs-lookup"><span data-stu-id="fa9ae-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="fa9ae-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fa9ae-120">None</span></span>|<span data-ttu-id="fa9ae-121">Reaplica os parâmetros de classificação atuais à tabela.</span><span class="sxs-lookup"><span data-stu-id="fa9ae-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="fa9ae-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa9ae-122">Properties</span></span>
| <span data-ttu-id="fa9ae-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa9ae-123">Property</span></span>     | <span data-ttu-id="fa9ae-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa9ae-124">Type</span></span>   |<span data-ttu-id="fa9ae-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa9ae-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa9ae-126">matchCase</span><span class="sxs-lookup"><span data-stu-id="fa9ae-126">matchCase</span></span>|<span data-ttu-id="fa9ae-127">booliano</span><span class="sxs-lookup"><span data-stu-id="fa9ae-127">boolean</span></span>|<span data-ttu-id="fa9ae-p102">Indica se o uso de maiúsculas ou minúsculas afetou a última classificação da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fa9ae-p102">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="fa9ae-130">method</span><span class="sxs-lookup"><span data-stu-id="fa9ae-130">method</span></span>|<span data-ttu-id="fa9ae-131">string</span><span class="sxs-lookup"><span data-stu-id="fa9ae-131">string</span></span>|<span data-ttu-id="fa9ae-p103">Indica o último método de ordenação de caracteres chineses usado para classificar a tabela. Os valores possíveis são: `PinYin` e `StrokeCount`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fa9ae-p103">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa9ae-135">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="fa9ae-135">Relationships</span></span>
| <span data-ttu-id="fa9ae-136">Relação</span><span class="sxs-lookup"><span data-stu-id="fa9ae-136">Relationship</span></span> | <span data-ttu-id="fa9ae-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa9ae-137">Type</span></span>   |<span data-ttu-id="fa9ae-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa9ae-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa9ae-139">campos</span><span class="sxs-lookup"><span data-stu-id="fa9ae-139">fields</span></span>|[<span data-ttu-id="fa9ae-140">SortField</span><span class="sxs-lookup"><span data-stu-id="fa9ae-140">SortField</span></span>](sortfield.md)|<span data-ttu-id="fa9ae-p104">Representa as condições atuais usadas para a última classificação da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fa9ae-p104">Represents the current conditions used to last sort the table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa9ae-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa9ae-143">JSON representation</span></span>

<span data-ttu-id="fa9ae-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa9ae-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableSort"
}-->

```json
{
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
  "suppressions": [
    "Error: /api-reference/beta/resources/tablesort.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
