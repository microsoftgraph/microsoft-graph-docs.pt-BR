---
author: JeremyKelley
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
description: A lookupColumn em um recurso columnDefinition indica que os valores da coluna são buscados em outra origem do site.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ec7da70a6f79793dbf12dbfea6c9fbfef53aaea9
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239342"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="19890-103">Tipo de recurso LookupColumn</span><span class="sxs-lookup"><span data-stu-id="19890-103">LookupColumn resource type</span></span>

<span data-ttu-id="19890-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19890-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19890-105">A **lookupColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são buscados em outra origem do site.</span><span class="sxs-lookup"><span data-stu-id="19890-105">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="19890-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="19890-106">JSON representation</span></span>

<span data-ttu-id="19890-107">Aqui está uma representação JSON de um recurso **lookupColumn**.</span><span class="sxs-lookup"><span data-stu-id="19890-107">Here is a JSON representation of a **lookupColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="19890-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="19890-108">Properties</span></span>

| <span data-ttu-id="19890-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="19890-109">Property name</span></span>             | <span data-ttu-id="19890-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="19890-110">Type</span></span>    | <span data-ttu-id="19890-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="19890-111">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="19890-112">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="19890-112">**allowMultipleValues**</span></span>   | <span data-ttu-id="19890-113">booliano</span><span class="sxs-lookup"><span data-stu-id="19890-113">boolean</span></span> | <span data-ttu-id="19890-114">Indica se vários valores podem ser selecionados da origem.</span><span class="sxs-lookup"><span data-stu-id="19890-114">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="19890-115">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="19890-115">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="19890-116">booliano</span><span class="sxs-lookup"><span data-stu-id="19890-116">boolean</span></span> | <span data-ttu-id="19890-117">Indica se os valores na coluna podem exceder o limite padrão de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="19890-117">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="19890-118">**columnName**</span><span class="sxs-lookup"><span data-stu-id="19890-118">**columnName**</span></span>            | <span data-ttu-id="19890-119">string</span><span class="sxs-lookup"><span data-stu-id="19890-119">string</span></span>  | <span data-ttu-id="19890-120">O nome da coluna de origem de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="19890-120">The name of the lookup source column.</span></span>
| <span data-ttu-id="19890-121">**listId**</span><span class="sxs-lookup"><span data-stu-id="19890-121">**listId**</span></span>                | <span data-ttu-id="19890-122">string</span><span class="sxs-lookup"><span data-stu-id="19890-122">string</span></span>  | <span data-ttu-id="19890-123">O identificador exclusivo da lista de origem de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="19890-123">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="19890-124">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="19890-124">**primaryLookupColumnId**</span></span> | <span data-ttu-id="19890-125">string</span><span class="sxs-lookup"><span data-stu-id="19890-125">string</span></span>  | <span data-ttu-id="19890-126">Se especificado, esta coluna é uma *pesquisa secundária*, obtendo um campo adicional da lista pesquisada pela *pesquisa primária*.</span><span class="sxs-lookup"><span data-stu-id="19890-126">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="19890-127">Use o item da lista procurado pela pesquisa *primária* como a fonte para a coluna nomeada aqui.</span><span class="sxs-lookup"><span data-stu-id="19890-127">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->

