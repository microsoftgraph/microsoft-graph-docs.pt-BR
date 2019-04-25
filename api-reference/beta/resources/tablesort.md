---
title: Tipo de recurso TableSort
description: Gerencia operações de classificação em objetos Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 612e0cb7d59011f04ae992f80119fc1da572b582
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583204"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="0a359-103">Tipo de recurso TableSort</span><span class="sxs-lookup"><span data-stu-id="0a359-103">TableSort resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a359-104">Gerencia operações de classificação em objetos Table.</span><span class="sxs-lookup"><span data-stu-id="0a359-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="0a359-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="0a359-105">Methods</span></span>

| <span data-ttu-id="0a359-106">Método</span><span class="sxs-lookup"><span data-stu-id="0a359-106">Method</span></span>           | <span data-ttu-id="0a359-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0a359-107">Return Type</span></span>    |<span data-ttu-id="0a359-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a359-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0a359-109">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="0a359-109">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="0a359-110">TableSort</span><span class="sxs-lookup"><span data-stu-id="0a359-110">TableSort</span></span>](tablesort.md) |<span data-ttu-id="0a359-111">Leia as propriedades e os relacionamentos do objeto tableSort.</span><span class="sxs-lookup"><span data-stu-id="0a359-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="0a359-112">Apply</span><span class="sxs-lookup"><span data-stu-id="0a359-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="0a359-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0a359-113">None</span></span>|<span data-ttu-id="0a359-114">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="0a359-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="0a359-115">Clear</span><span class="sxs-lookup"><span data-stu-id="0a359-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="0a359-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0a359-116">None</span></span>|<span data-ttu-id="0a359-p101">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="0a359-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="0a359-119">Reapply</span><span class="sxs-lookup"><span data-stu-id="0a359-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="0a359-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0a359-120">None</span></span>|<span data-ttu-id="0a359-121">Reaplica os parâmetros de classificação atuais à tabela.</span><span class="sxs-lookup"><span data-stu-id="0a359-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="0a359-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a359-122">Properties</span></span>
| <span data-ttu-id="0a359-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a359-123">Property</span></span>     | <span data-ttu-id="0a359-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a359-124">Type</span></span>   |<span data-ttu-id="0a359-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a359-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a359-126">matchCase</span><span class="sxs-lookup"><span data-stu-id="0a359-126">matchCase</span></span>|<span data-ttu-id="0a359-127">booliano</span><span class="sxs-lookup"><span data-stu-id="0a359-127">boolean</span></span>|<span data-ttu-id="0a359-p102">Indica se o uso de maiúsculas ou minúsculas afetou a última classificação da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0a359-p102">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="0a359-130">method</span><span class="sxs-lookup"><span data-stu-id="0a359-130">method</span></span>|<span data-ttu-id="0a359-131">string</span><span class="sxs-lookup"><span data-stu-id="0a359-131">string</span></span>|<span data-ttu-id="0a359-p103">Indica o último método de ordenação de caracteres chineses usado para classificar a tabela. Os valores possíveis são: `PinYin` e `StrokeCount`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0a359-p103">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a359-135">Relações</span><span class="sxs-lookup"><span data-stu-id="0a359-135">Relationships</span></span>
| <span data-ttu-id="0a359-136">Relação</span><span class="sxs-lookup"><span data-stu-id="0a359-136">Relationship</span></span> | <span data-ttu-id="0a359-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a359-137">Type</span></span>   |<span data-ttu-id="0a359-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a359-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a359-139">campos</span><span class="sxs-lookup"><span data-stu-id="0a359-139">fields</span></span>|[<span data-ttu-id="0a359-140">SortField</span><span class="sxs-lookup"><span data-stu-id="0a359-140">SortField</span></span>](sortfield.md)|<span data-ttu-id="0a359-p104">Representa as condições atuais usadas para a última classificação da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0a359-p104">Represents the current conditions used to last sort the table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a359-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a359-143">JSON representation</span></span>

<span data-ttu-id="0a359-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0a359-144">Here is a JSON representation of the resource.</span></span>

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
