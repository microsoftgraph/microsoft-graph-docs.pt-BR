---
title: Tipo de recurso TableSort
description: Gerencia operações de classificação em objetos Table.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5e5e93fb1cccb420e8da08015109c81dc45ae688
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966486"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="778bc-103">Tipo de recurso TableSort</span><span class="sxs-lookup"><span data-stu-id="778bc-103">TableSort resource type</span></span>

> <span data-ttu-id="778bc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="778bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="778bc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="778bc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="778bc-106">Gerencia operações de classificação em objetos Table.</span><span class="sxs-lookup"><span data-stu-id="778bc-106">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="778bc-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="778bc-107">Methods</span></span>

| <span data-ttu-id="778bc-108">Método</span><span class="sxs-lookup"><span data-stu-id="778bc-108">Method</span></span>           | <span data-ttu-id="778bc-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="778bc-109">Return Type</span></span>    |<span data-ttu-id="778bc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="778bc-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="778bc-111">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="778bc-111">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="778bc-112">TableSort</span><span class="sxs-lookup"><span data-stu-id="778bc-112">TableSort</span></span>](tablesort.md) |<span data-ttu-id="778bc-113">Leia as propriedades e os relacionamentos do objeto tableSort.</span><span class="sxs-lookup"><span data-stu-id="778bc-113">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="778bc-114">Aplicar</span><span class="sxs-lookup"><span data-stu-id="778bc-114">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="778bc-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="778bc-115">None</span></span>|<span data-ttu-id="778bc-116">Execute uma operação de classificação.</span><span class="sxs-lookup"><span data-stu-id="778bc-116">Perform a sort operation.</span></span>|
|[<span data-ttu-id="778bc-117">Clear</span><span class="sxs-lookup"><span data-stu-id="778bc-117">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="778bc-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="778bc-118">None</span></span>|<span data-ttu-id="778bc-p102">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="778bc-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="778bc-121">Reapply</span><span class="sxs-lookup"><span data-stu-id="778bc-121">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="778bc-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="778bc-122">None</span></span>|<span data-ttu-id="778bc-123">Reaplica os parâmetros de classificação atuais à tabela.</span><span class="sxs-lookup"><span data-stu-id="778bc-123">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="778bc-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="778bc-124">Properties</span></span>
| <span data-ttu-id="778bc-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="778bc-125">Property</span></span>     | <span data-ttu-id="778bc-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="778bc-126">Type</span></span>   |<span data-ttu-id="778bc-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="778bc-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="778bc-128">matchCase</span><span class="sxs-lookup"><span data-stu-id="778bc-128">matchCase</span></span>|<span data-ttu-id="778bc-129">booliano</span><span class="sxs-lookup"><span data-stu-id="778bc-129">boolean</span></span>|<span data-ttu-id="778bc-p103">Indica se o uso de maiúsculas ou minúsculas afetou a última classificação da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="778bc-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="778bc-132">method</span><span class="sxs-lookup"><span data-stu-id="778bc-132">method</span></span>|<span data-ttu-id="778bc-133">string</span><span class="sxs-lookup"><span data-stu-id="778bc-133">string</span></span>|<span data-ttu-id="778bc-p104">Indica o último método de ordenação de caracteres chineses usado para classificar a tabela. Os valores possíveis são: `PinYin` e `StrokeCount`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="778bc-p104">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="778bc-137">Relações</span><span class="sxs-lookup"><span data-stu-id="778bc-137">Relationships</span></span>
| <span data-ttu-id="778bc-138">Relação</span><span class="sxs-lookup"><span data-stu-id="778bc-138">Relationship</span></span> | <span data-ttu-id="778bc-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="778bc-139">Type</span></span>   |<span data-ttu-id="778bc-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="778bc-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="778bc-141">campos</span><span class="sxs-lookup"><span data-stu-id="778bc-141">fields</span></span>|[<span data-ttu-id="778bc-142">SortField</span><span class="sxs-lookup"><span data-stu-id="778bc-142">SortField</span></span>](sortfield.md)|<span data-ttu-id="778bc-p105">Representa as condições atuais usadas para a última classificação da tabela. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="778bc-p105">Represents the current conditions used to last sort the table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="778bc-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="778bc-145">JSON representation</span></span>

<span data-ttu-id="778bc-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="778bc-146">Here is a JSON representation of the resource.</span></span>

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
