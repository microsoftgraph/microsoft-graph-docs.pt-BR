---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: LookupColumn
ms.openlocfilehash: 07dba3c223ffc3993be1fc284572810a7aa3ccf8
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="7edc8-102">Tipo de recurso LookupColumn</span><span class="sxs-lookup"><span data-stu-id="7edc8-102">LookupColumn resource type</span></span>

<span data-ttu-id="7edc8-103">A **lookupColumn** em um recurso [columnDefinition](columnDefinition.md) indica que os valores da coluna são buscados em outra origem do site.</span><span class="sxs-lookup"><span data-stu-id="7edc8-103">The **lookupColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7edc8-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7edc8-104">JSON representation</span></span>

<span data-ttu-id="7edc8-105">Aqui está uma representação JSON de um recurso **lookupColumn**.</span><span class="sxs-lookup"><span data-stu-id="7edc8-105">Here is a JSON representation of a **driveItem** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="7edc8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7edc8-106">Properties</span></span>

| <span data-ttu-id="7edc8-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7edc8-107">Property name</span></span>             | <span data-ttu-id="7edc8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7edc8-108">Type</span></span>    | <span data-ttu-id="7edc8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7edc8-109">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="7edc8-110">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="7edc8-110">**allowMultipleValues**</span></span>   | <span data-ttu-id="7edc8-111">booliano</span><span class="sxs-lookup"><span data-stu-id="7edc8-111">boolean</span></span> | <span data-ttu-id="7edc8-112">Indica se vários valores podem ser selecionados da origem.</span><span class="sxs-lookup"><span data-stu-id="7edc8-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="7edc8-113">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="7edc8-113">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="7edc8-114">booliano</span><span class="sxs-lookup"><span data-stu-id="7edc8-114">boolean</span></span> | <span data-ttu-id="7edc8-115">Indica se os valores na coluna podem exceder o limite padrão de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="7edc8-115">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="7edc8-116">**columnName**</span><span class="sxs-lookup"><span data-stu-id="7edc8-116">**columnName**</span></span>            | <span data-ttu-id="7edc8-117">string</span><span class="sxs-lookup"><span data-stu-id="7edc8-117">string</span></span>  | <span data-ttu-id="7edc8-118">O nome da coluna de origem de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7edc8-118">The name of the lookup source column.</span></span>
| <span data-ttu-id="7edc8-119">**listId**</span><span class="sxs-lookup"><span data-stu-id="7edc8-119">**listId**</span></span>                | <span data-ttu-id="7edc8-120">string</span><span class="sxs-lookup"><span data-stu-id="7edc8-120">string</span></span>  | <span data-ttu-id="7edc8-121">O identificador exclusivo da lista de origem de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7edc8-121">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="7edc8-122">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="7edc8-122">**primaryLookupColumnId**</span></span> | <span data-ttu-id="7edc8-123">string</span><span class="sxs-lookup"><span data-stu-id="7edc8-123">string</span></span>  | <span data-ttu-id="7edc8-124">Se especificado, esta coluna é uma *pesquisa secundária*, obtendo um campo adicional da lista pesquisada pela *pesquisa primária*.</span><span class="sxs-lookup"><span data-stu-id="7edc8-124">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="7edc8-125">Use o item da lista procurado pela pesquisa *primária* como a fonte para a coluna nomeada aqui.</span><span class="sxs-lookup"><span data-stu-id="7edc8-125">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn"
} -->
