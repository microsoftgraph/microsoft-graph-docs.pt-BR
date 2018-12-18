---
title: Tipo de recurso TableSort
description: Gerencia operações de classificação em objetos Table.
author: lumine2008
ms.openlocfilehash: 52ee5288698b236f7ee4d29eb75fdac5ad14fa0f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339820"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="446f3-103">Tipo de recurso TableSort</span><span class="sxs-lookup"><span data-stu-id="446f3-103">TableSort resource type</span></span>

> <span data-ttu-id="446f3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="446f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="446f3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="446f3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="446f3-106">Gerencia operações de classificação em objetos Table.</span><span class="sxs-lookup"><span data-stu-id="446f3-106">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="446f3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="446f3-107">Methods</span></span>

| <span data-ttu-id="446f3-108">Método</span><span class="sxs-lookup"><span data-stu-id="446f3-108">Method</span></span>           | <span data-ttu-id="446f3-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="446f3-109">Return Type</span></span>    |<span data-ttu-id="446f3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="446f3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="446f3-111">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="446f3-111">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="446f3-112">TableSort</span><span class="sxs-lookup"><span data-stu-id="446f3-112">TableSort</span></span>](tablesort.md) |<span data-ttu-id="446f3-113">Leia as propriedades e os relacionamentos do objeto tableSort.</span><span class="sxs-lookup"><span data-stu-id="446f3-113">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="446f3-114">Aplicar</span><span class="sxs-lookup"><span data-stu-id="446f3-114">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="446f3-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="446f3-115">None</span></span>|<span data-ttu-id="446f3-116">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="446f3-116">Perform a sort operation.</span></span>|
|[<span data-ttu-id="446f3-117">Clear</span><span class="sxs-lookup"><span data-stu-id="446f3-117">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="446f3-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="446f3-118">None</span></span>|<span data-ttu-id="446f3-p102">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="446f3-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="446f3-121">Reapply</span><span class="sxs-lookup"><span data-stu-id="446f3-121">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="446f3-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="446f3-122">None</span></span>|<span data-ttu-id="446f3-123">Reaplica os parâmetros de classificação atuais à tabela.</span><span class="sxs-lookup"><span data-stu-id="446f3-123">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="446f3-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="446f3-124">Properties</span></span>
| <span data-ttu-id="446f3-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="446f3-125">Property</span></span>     | <span data-ttu-id="446f3-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="446f3-126">Type</span></span>   |<span data-ttu-id="446f3-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="446f3-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="446f3-128">matchCase</span><span class="sxs-lookup"><span data-stu-id="446f3-128">matchCase</span></span>|<span data-ttu-id="446f3-129">booliano</span><span class="sxs-lookup"><span data-stu-id="446f3-129">boolean</span></span>|<span data-ttu-id="446f3-p103">Indica se o uso de maiúsculas ou minúsculas afetou a última classificação da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="446f3-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="446f3-132">method</span><span class="sxs-lookup"><span data-stu-id="446f3-132">method</span></span>|<span data-ttu-id="446f3-133">string</span><span class="sxs-lookup"><span data-stu-id="446f3-133">string</span></span>|<span data-ttu-id="446f3-p104">Indica o último método de ordenação de caracteres chineses usado para classificar a tabela. Os valores possíveis são: `PinYin` e `StrokeCount`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="446f3-p104">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="446f3-137">Relações</span><span class="sxs-lookup"><span data-stu-id="446f3-137">Relationships</span></span>
| <span data-ttu-id="446f3-138">Relação</span><span class="sxs-lookup"><span data-stu-id="446f3-138">Relationship</span></span> | <span data-ttu-id="446f3-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="446f3-139">Type</span></span>   |<span data-ttu-id="446f3-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="446f3-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="446f3-141">campos</span><span class="sxs-lookup"><span data-stu-id="446f3-141">fields</span></span>|[<span data-ttu-id="446f3-142">SortField</span><span class="sxs-lookup"><span data-stu-id="446f3-142">SortField</span></span>](sortfield.md)|<span data-ttu-id="446f3-p105">Representa as condições atuais usadas para a última classificação da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="446f3-p105">Represents the current conditions used to last sort the table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="446f3-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="446f3-145">JSON representation</span></span>

<span data-ttu-id="446f3-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="446f3-146">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->