---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
description: A lookupColumn em um recurso columnDefinition indica que os valores da coluna são buscados em outra origem do site.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5f0299816a1ea53338053708dbd99f7be8428051
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036340"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="d26f2-103">Tipo de recurso LookupColumn</span><span class="sxs-lookup"><span data-stu-id="d26f2-103">LookupColumn resource type</span></span>

<span data-ttu-id="d26f2-104">A **lookupColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são buscados em outra origem do site.</span><span class="sxs-lookup"><span data-stu-id="d26f2-104">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d26f2-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d26f2-105">JSON representation</span></span>

<span data-ttu-id="d26f2-106">Aqui está uma representação JSON de um recurso **lookupColumn**.</span><span class="sxs-lookup"><span data-stu-id="d26f2-106">Here is a JSON representation of a **lookupColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.lookupColumn" } -->

```json
{
  "allowMultipleValues": true,
  "allowUnlimitedLength": false,
  "columnName": "string",
  "listId": "string",
  "primaryLookupColumnId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="d26f2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d26f2-107">Properties</span></span>

| <span data-ttu-id="d26f2-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="d26f2-108">Property name</span></span>             | <span data-ttu-id="d26f2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d26f2-109">Type</span></span>    | <span data-ttu-id="d26f2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d26f2-110">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="d26f2-111">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="d26f2-111">**allowMultipleValues**</span></span>   | <span data-ttu-id="d26f2-112">booliano</span><span class="sxs-lookup"><span data-stu-id="d26f2-112">boolean</span></span> | <span data-ttu-id="d26f2-113">Indica se vários valores podem ser selecionados da origem.</span><span class="sxs-lookup"><span data-stu-id="d26f2-113">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="d26f2-114">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="d26f2-114">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="d26f2-115">booliano</span><span class="sxs-lookup"><span data-stu-id="d26f2-115">boolean</span></span> | <span data-ttu-id="d26f2-116">Indica se os valores na coluna podem exceder o limite padrão de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="d26f2-116">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="d26f2-117">**columnName**</span><span class="sxs-lookup"><span data-stu-id="d26f2-117">**columnName**</span></span>            | <span data-ttu-id="d26f2-118">string</span><span class="sxs-lookup"><span data-stu-id="d26f2-118">string</span></span>  | <span data-ttu-id="d26f2-119">O nome da coluna de origem de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="d26f2-119">The name of the lookup source column.</span></span>
| <span data-ttu-id="d26f2-120">**listId**</span><span class="sxs-lookup"><span data-stu-id="d26f2-120">**listId**</span></span>                | <span data-ttu-id="d26f2-121">string</span><span class="sxs-lookup"><span data-stu-id="d26f2-121">string</span></span>  | <span data-ttu-id="d26f2-122">O identificador exclusivo da lista de origem de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="d26f2-122">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="d26f2-123">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="d26f2-123">**primaryLookupColumnId**</span></span> | <span data-ttu-id="d26f2-124">string</span><span class="sxs-lookup"><span data-stu-id="d26f2-124">string</span></span>  | <span data-ttu-id="d26f2-125">Se especificado, esta coluna é uma *pesquisa secundária*, obtendo um campo adicional da lista pesquisada pela *pesquisa primária*.</span><span class="sxs-lookup"><span data-stu-id="d26f2-125">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="d26f2-126">Use o item da lista procurado pela pesquisa *primária* como a fonte para a coluna nomeada aqui.</span><span class="sxs-lookup"><span data-stu-id="d26f2-126">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
