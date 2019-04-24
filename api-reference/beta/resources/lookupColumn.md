---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: LookupColumn
localization_priority: Normal
ms.openlocfilehash: 1a38cc3e08917b0d4aa2a8df4943ebc932c937d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506224"
---
# <a name="lookupcolumn-resource-type"></a><span data-ttu-id="e83ec-102">Tipo de recurso LookupColumn</span><span class="sxs-lookup"><span data-stu-id="e83ec-102">LookupColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e83ec-103">A **lookupColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são buscados em outra origem do site.</span><span class="sxs-lookup"><span data-stu-id="e83ec-103">The **lookupColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are looked up from another source in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e83ec-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e83ec-104">JSON representation</span></span>

<span data-ttu-id="e83ec-105">Aqui está uma representação JSON de um recurso **lookupColumn**.</span><span class="sxs-lookup"><span data-stu-id="e83ec-105">Here is a JSON representation of a **lookupColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="e83ec-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e83ec-106">Properties</span></span>

| <span data-ttu-id="e83ec-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e83ec-107">Property name</span></span>             | <span data-ttu-id="e83ec-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e83ec-108">Type</span></span>    | <span data-ttu-id="e83ec-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e83ec-109">Description</span></span>
|:--------------------------|:--------|:---------------------------------------
| <span data-ttu-id="e83ec-110">**allowMultipleValues**</span><span class="sxs-lookup"><span data-stu-id="e83ec-110">**allowMultipleValues**</span></span>   | <span data-ttu-id="e83ec-111">booliano</span><span class="sxs-lookup"><span data-stu-id="e83ec-111">boolean</span></span> | <span data-ttu-id="e83ec-112">Indica se vários valores podem ser selecionados da origem.</span><span class="sxs-lookup"><span data-stu-id="e83ec-112">Indicates whether multiple values can be selected from the source.</span></span>
| <span data-ttu-id="e83ec-113">**allowUnlimitedLength**</span><span class="sxs-lookup"><span data-stu-id="e83ec-113">**allowUnlimitedLength**</span></span>  | <span data-ttu-id="e83ec-114">booliano</span><span class="sxs-lookup"><span data-stu-id="e83ec-114">boolean</span></span> | <span data-ttu-id="e83ec-115">Indica se os valores na coluna podem exceder o limite padrão de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="e83ec-115">Indicates whether values in the column should be able to exceed the standard limit of 255 characters.</span></span>
| <span data-ttu-id="e83ec-116">**columnName**</span><span class="sxs-lookup"><span data-stu-id="e83ec-116">**columnName**</span></span>            | <span data-ttu-id="e83ec-117">string</span><span class="sxs-lookup"><span data-stu-id="e83ec-117">string</span></span>  | <span data-ttu-id="e83ec-118">O nome da coluna de origem de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="e83ec-118">The name of the lookup source column.</span></span>
| <span data-ttu-id="e83ec-119">**listId**</span><span class="sxs-lookup"><span data-stu-id="e83ec-119">**listId**</span></span>                | <span data-ttu-id="e83ec-120">string</span><span class="sxs-lookup"><span data-stu-id="e83ec-120">string</span></span>  | <span data-ttu-id="e83ec-121">O identificador exclusivo da lista de origem de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="e83ec-121">The unique identifier of the lookup source list.</span></span>
| <span data-ttu-id="e83ec-122">**primaryLookupColumnId**</span><span class="sxs-lookup"><span data-stu-id="e83ec-122">**primaryLookupColumnId**</span></span> | <span data-ttu-id="e83ec-123">string</span><span class="sxs-lookup"><span data-stu-id="e83ec-123">string</span></span>  | <span data-ttu-id="e83ec-124">Se especificado, esta coluna é uma *pesquisa secundária*, obtendo um campo adicional da lista pesquisada pela *pesquisa primária*.</span><span class="sxs-lookup"><span data-stu-id="e83ec-124">If specified, this column is a *secondary lookup*, pulling an additional field from the list item looked up by the *primary lookup*.</span></span> <span data-ttu-id="e83ec-125">Use o item da lista procurado pela pesquisa *primária* como a fonte para a coluna nomeada aqui.</span><span class="sxs-lookup"><span data-stu-id="e83ec-125">Use the list item looked up by the *primary* as the source for the column named here.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/LookupColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/lookupColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
