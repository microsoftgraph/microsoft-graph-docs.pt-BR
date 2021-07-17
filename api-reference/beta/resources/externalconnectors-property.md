---
title: tipo de recurso de propriedade
description: Uma definição de propriedade de esquema para uma Pesquisa da Microsoft conexão.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 68dfe94d81f4ae5347322ba17c02eb3dab5c15d7
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467599"
---
# <a name="property-resource-type"></a><span data-ttu-id="feced-103">tipo de recurso de propriedade</span><span class="sxs-lookup"><span data-stu-id="feced-103">property resource type</span></span>

<span data-ttu-id="feced-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="feced-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="feced-105">Uma [definição de propriedade](externalconnectors-schema.md) de esquema para uma Pesquisa da Microsoft [conexão](externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="feced-105">A [schema](externalconnectors-schema.md) property definition for a Microsoft Search [connection](externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="feced-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="feced-106">Properties</span></span>

| <span data-ttu-id="feced-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="feced-107">Property</span></span>      | <span data-ttu-id="feced-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="feced-108">Type</span></span>              | <span data-ttu-id="feced-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="feced-109">Description</span></span>                                        |
|:--------------|:------------------|:---------------------------------------------------|
| <span data-ttu-id="feced-110">aliases</span><span class="sxs-lookup"><span data-stu-id="feced-110">aliases</span></span>       | <span data-ttu-id="feced-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="feced-111">String collection</span></span> | <span data-ttu-id="feced-112">Um conjunto de aliases ou nomes amigáveis para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="feced-112">A set of aliases or a friendly names for the property.</span></span> <span data-ttu-id="feced-113">Máximo de 32 caracteres.</span><span class="sxs-lookup"><span data-stu-id="feced-113">Maximum 32 characters.</span></span> <span data-ttu-id="feced-114">Cada cadeia de caracteres não deve conter caracteres de controle, espaço em branco ou qualquer um dos seguintes: `:` , , , , `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` , , , , `*` , `=` `&` `?` `@` , `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` .</span><span class="sxs-lookup"><span data-stu-id="feced-114">Each string must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="feced-115">Opcional.</span><span class="sxs-lookup"><span data-stu-id="feced-115">Optional.</span></span>  |
| <span data-ttu-id="feced-116">isQueryable</span><span class="sxs-lookup"><span data-stu-id="feced-116">isQueryable</span></span>   | <span data-ttu-id="feced-117">booliano</span><span class="sxs-lookup"><span data-stu-id="feced-117">boolean</span></span>           | <span data-ttu-id="feced-118">Especifica se a propriedade pode ser consultada.</span><span class="sxs-lookup"><span data-stu-id="feced-118">Specifies if the property is queryable.</span></span> <span data-ttu-id="feced-119">As propriedades queryable podem ser usadas em consultas [KQL (Keyword Query Language).](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)</span><span class="sxs-lookup"><span data-stu-id="feced-119">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="feced-120">Opcional.</span><span class="sxs-lookup"><span data-stu-id="feced-120">Optional.</span></span>  |
| <span data-ttu-id="feced-121">isRefinable</span><span class="sxs-lookup"><span data-stu-id="feced-121">isRefinable</span></span>   | <span data-ttu-id="feced-122">booliano</span><span class="sxs-lookup"><span data-stu-id="feced-122">boolean</span></span>           | <span data-ttu-id="feced-123">Especifica se a propriedade é refinável.</span><span class="sxs-lookup"><span data-stu-id="feced-123">Specifies if the property is refinable.</span></span>  <span data-ttu-id="feced-124">As propriedades refináveis podem ser usadas para filtrar os resultados da pesquisa na [API](search-api-overview.md) de Pesquisa e adicionar um controle refinador na experiência Pesquisa da Microsoft usuário.</span><span class="sxs-lookup"><span data-stu-id="feced-124">Refinable properties can be used to filter search results in the [Search API](search-api-overview.md) and add a refiner control in the Microsoft Search user experience.</span></span> <span data-ttu-id="feced-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="feced-125">Optional.</span></span>  |
| <span data-ttu-id="feced-126">isRetrievable</span><span class="sxs-lookup"><span data-stu-id="feced-126">isRetrievable</span></span> | <span data-ttu-id="feced-127">booliano</span><span class="sxs-lookup"><span data-stu-id="feced-127">boolean</span></span>           | <span data-ttu-id="feced-128">Especifica se a propriedade é recuperável.</span><span class="sxs-lookup"><span data-stu-id="feced-128">Specifies if the property is retrievable.</span></span> <span data-ttu-id="feced-129">As propriedades recuperáveis são retornadas no conjunto de resultados quando os itens são retornados pela API de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="feced-129">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="feced-130">Propriedades recuperáveis também estão disponíveis para adicionar ao modelo de exibição usado para renderizar os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="feced-130">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="feced-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="feced-131">Optional.</span></span> |
| <span data-ttu-id="feced-132">isSearchable</span><span class="sxs-lookup"><span data-stu-id="feced-132">isSearchable</span></span>  | <span data-ttu-id="feced-133">booliano</span><span class="sxs-lookup"><span data-stu-id="feced-133">boolean</span></span>           | <span data-ttu-id="feced-134">Especifica se a propriedade é pesquisável.</span><span class="sxs-lookup"><span data-stu-id="feced-134">Specifies if the property is searchable.</span></span> <span data-ttu-id="feced-135">Somente propriedades do tipo `string` ou `stringCollection` podem ser pesquisáveis.</span><span class="sxs-lookup"><span data-stu-id="feced-135">Only properties of type `string` or `stringCollection` can be searchable.</span></span> <span data-ttu-id="feced-136">Propriedades não pesquisáveis não são adicionadas ao índice de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="feced-136">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="feced-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="feced-137">Optional.</span></span> |
| <span data-ttu-id="feced-138">labels</span><span class="sxs-lookup"><span data-stu-id="feced-138">labels</span></span>        | <span data-ttu-id="feced-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="feced-139">String collection</span></span> | <span data-ttu-id="feced-140">Especifica uma ou mais marcas conhecidas adicionadas a uma propriedade.</span><span class="sxs-lookup"><span data-stu-id="feced-140">Specifies one or more well-known tags added against a property.</span></span> <span data-ttu-id="feced-141">Os rótulos Pesquisa da Microsoft entender a semântica dos dados na conexão.</span><span class="sxs-lookup"><span data-stu-id="feced-141">Labels help Microsoft Search understand the semantics of the data in the connection.</span></span> <span data-ttu-id="feced-142">Adicionar rótulos apropriados resultaria em uma experiência de pesquisa aprimorada (por exemplo, melhor relevância).</span><span class="sxs-lookup"><span data-stu-id="feced-142">Adding appropriate labels would result in an enhanced search experience (e.g. better relevance).</span></span> <span data-ttu-id="feced-143">Rótulos com `title` suporte: `url` , , , , , , , , `createdBy` , , , , , `lastModifiedBy` e `authors` `createdDateTime` `lastModifiedDateTime` `fileName` `fileExtension` `iconUrl` `containerName` `containerUrl` .</span><span class="sxs-lookup"><span data-stu-id="feced-143">Supported labels: `title`, `url`, `createdBy`, `lastModifiedBy`, `authors`, `createdDateTime`, `lastModifiedDateTime`, `fileName`, `fileExtension`, `iconUrl`, `containerName`, and `containerUrl`.</span></span> <span data-ttu-id="feced-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="feced-144">Optional.</span></span> |
| <span data-ttu-id="feced-145">nome</span><span class="sxs-lookup"><span data-stu-id="feced-145">name</span></span>          | <span data-ttu-id="feced-146">String</span><span class="sxs-lookup"><span data-stu-id="feced-146">String</span></span>            | <span data-ttu-id="feced-147">O nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="feced-147">The name of the property.</span></span> <span data-ttu-id="feced-148">Máximo de 32 caracteres.</span><span class="sxs-lookup"><span data-stu-id="feced-148">Maximum 32 characters.</span></span> <span data-ttu-id="feced-149">Não deve conter caracteres de controle, espaço em branco ou qualquer um dos seguintes: `:` , , , , , `;` `,` `(` `)` `[` `]` , `{` `}` , , `%` , , , `$` `+` `!` `*` `=` `&` `?` `@` `#` , `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` .</span><span class="sxs-lookup"><span data-stu-id="feced-149">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="feced-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="feced-150">Required.</span></span>                |
| <span data-ttu-id="feced-151">tipo</span><span class="sxs-lookup"><span data-stu-id="feced-151">type</span></span>          | <span data-ttu-id="feced-152">String</span><span class="sxs-lookup"><span data-stu-id="feced-152">String</span></span>            | <span data-ttu-id="feced-153">O tipo de dados da propriedade.</span><span class="sxs-lookup"><span data-stu-id="feced-153">The data type of the property.</span></span> <span data-ttu-id="feced-154">Os valores possíveis são: `string`, `int64`, `double`, `dateTime`, `boolean`, `stringCollection`, `int64Collection`, `doubleCollection`, `dateTimeCollection`.</span><span class="sxs-lookup"><span data-stu-id="feced-154">Possible values are: `string`, `int64`, `double`, `dateTime`, `boolean`, `stringCollection`, `int64Collection`, `doubleCollection`, `dateTimeCollection`.</span></span> <span data-ttu-id="feced-155">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="feced-155">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="feced-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="feced-156">JSON representation</span></span>

<span data-ttu-id="feced-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="feced-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.property",
  "baseType": null
}-->

```json
{
  "aliases": [ "String" ],
  "isQueryable": true,
  "isRefinable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "labels": [ "string" ],
  "name": "string",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "property resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
