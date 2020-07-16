---
title: tipo de recurso Property
description: Uma definição de propriedade de esquema para uma conexão do Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9862170dfcca0960ebd319089da70cca93782875
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990260"
---
# <a name="property-resource-type"></a><span data-ttu-id="14508-103">tipo de recurso Property</span><span class="sxs-lookup"><span data-stu-id="14508-103">property resource type</span></span>

<span data-ttu-id="14508-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14508-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14508-105">Uma definição de propriedade de [esquema](schema.md) para uma [conexão](externalconnection.md)do Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="14508-105">A [schema](schema.md) property definition for a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="14508-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14508-106">Properties</span></span>

| <span data-ttu-id="14508-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14508-107">Property</span></span>      | <span data-ttu-id="14508-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="14508-108">Type</span></span>              | <span data-ttu-id="14508-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="14508-109">Description</span></span>                                        |
|:--------------|:------------------|:---------------------------------------------------|
| <span data-ttu-id="14508-110">aliases</span><span class="sxs-lookup"><span data-stu-id="14508-110">aliases</span></span>       | <span data-ttu-id="14508-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="14508-111">String collection</span></span> | <span data-ttu-id="14508-112">Um conjunto de aliases ou um nome amigável para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="14508-112">A set of aliases or a friendly names for the property.</span></span> <span data-ttu-id="14508-113">Máximo de 32 caracteres.</span><span class="sxs-lookup"><span data-stu-id="14508-113">Maximum 32 characters.</span></span> <span data-ttu-id="14508-114">Cada cadeia de caracteres não deve conter caracteres de controle, espaço em branco ou qualquer um dos seguintes: `:` ,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, `;` `,` , `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` , `|` `` ` `` `^` ,,,,,,,,,</span><span class="sxs-lookup"><span data-stu-id="14508-114">Each string must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="14508-115">Opcional.</span><span class="sxs-lookup"><span data-stu-id="14508-115">Optional.</span></span>  |
| <span data-ttu-id="14508-116">IsQuery</span><span class="sxs-lookup"><span data-stu-id="14508-116">isQueryable</span></span>   | <span data-ttu-id="14508-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="14508-117">Boolean</span></span>           | <span data-ttu-id="14508-118">Especifica se a propriedade é consultável.</span><span class="sxs-lookup"><span data-stu-id="14508-118">Specifies if the property is queryable.</span></span> <span data-ttu-id="14508-119">Propriedades consultáveis podem ser usadas em [consultas de idioma de consulta de palavra-chave (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span><span class="sxs-lookup"><span data-stu-id="14508-119">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="14508-120">Opcional.</span><span class="sxs-lookup"><span data-stu-id="14508-120">Optional.</span></span>  |
| <span data-ttu-id="14508-121">isRefinable</span><span class="sxs-lookup"><span data-stu-id="14508-121">isRefinable</span></span>   | <span data-ttu-id="14508-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="14508-122">Boolean</span></span>           | <span data-ttu-id="14508-123">Especifica se a propriedade é refinável.</span><span class="sxs-lookup"><span data-stu-id="14508-123">Specifies if the property is refinable.</span></span>  <span data-ttu-id="14508-124">As propriedades refinável podem ser usadas para filtrar os resultados da pesquisa na [API de pesquisa](search-api-overview.md) e adicionar um controle de refinamento na experiência do usuário do Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="14508-124">Refinable properties can be used to filter search results in the [Search API](search-api-overview.md) and add a refiner control in the Microsoft Search user experience.</span></span> <span data-ttu-id="14508-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="14508-125">Optional.</span></span>  |
| <span data-ttu-id="14508-126">isretrievable</span><span class="sxs-lookup"><span data-stu-id="14508-126">isRetrievable</span></span> | <span data-ttu-id="14508-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="14508-127">Boolean</span></span>           | <span data-ttu-id="14508-128">Especifica se a propriedade é recuperável.</span><span class="sxs-lookup"><span data-stu-id="14508-128">Specifies if the property is retrievable.</span></span> <span data-ttu-id="14508-129">As propriedades recuperáveis são retornadas no conjunto de resultados quando os itens são retornados pela API de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="14508-129">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="14508-130">As propriedades recuperáveis também estão disponíveis para adicionar ao modelo de exibição usado para renderizar os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="14508-130">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="14508-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="14508-131">Optional.</span></span> |
| <span data-ttu-id="14508-132">IsSearchable</span><span class="sxs-lookup"><span data-stu-id="14508-132">isSearchable</span></span>  | <span data-ttu-id="14508-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="14508-133">Boolean</span></span>           | <span data-ttu-id="14508-134">Especifica se a propriedade é pesquisável.</span><span class="sxs-lookup"><span data-stu-id="14508-134">Specifies if the property is searchable.</span></span> <span data-ttu-id="14508-135">Somente propriedades do tipo `String` ou `StringCollection` podem ser pesquisáveis.</span><span class="sxs-lookup"><span data-stu-id="14508-135">Only properties of type `String` or `StringCollection` can be searchable.</span></span> <span data-ttu-id="14508-136">As propriedades não pesquisáveis não são adicionadas ao índice de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="14508-136">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="14508-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="14508-137">Optional.</span></span> |
| <span data-ttu-id="14508-138">Legendas</span><span class="sxs-lookup"><span data-stu-id="14508-138">labels</span></span>        | <span data-ttu-id="14508-139">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="14508-139">String collection</span></span> | <span data-ttu-id="14508-140">Especifica uma ou mais marcas conhecidas e adicionadas a uma propriedade.</span><span class="sxs-lookup"><span data-stu-id="14508-140">Specifies one or more well-known tags added against a property.</span></span> <span data-ttu-id="14508-141">Os rótulos ajudam a pesquisa da Microsoft a entender a semântica dos dados na conexão.</span><span class="sxs-lookup"><span data-stu-id="14508-141">Labels help Microsoft Search understand the semantics of the data in the connection.</span></span> <span data-ttu-id="14508-142">A adição de rótulos apropriados resultaria em uma experiência de pesquisa avançada (por exemplo, maior relevância).</span><span class="sxs-lookup"><span data-stu-id="14508-142">Adding appropriate labels would result in an enhanced search experience (e.g. better relevance).</span></span> <span data-ttu-id="14508-143">Rótulos com suporte:,,,,, `title` `url` `createdBy` `lastModifiedBy` `authors` `createdDateTime` , `lastModifiedDateTime` , `fileName` e `fileExtension` .</span><span class="sxs-lookup"><span data-stu-id="14508-143">Supported labels: `title`, `url`, `createdBy`, `lastModifiedBy`, `authors`, `createdDateTime`, `lastModifiedDateTime`, `fileName` and `fileExtension`.</span></span> <span data-ttu-id="14508-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="14508-144">Optional.</span></span> |
| <span data-ttu-id="14508-145">nome</span><span class="sxs-lookup"><span data-stu-id="14508-145">name</span></span>          | <span data-ttu-id="14508-146">String</span><span class="sxs-lookup"><span data-stu-id="14508-146">String</span></span>            | <span data-ttu-id="14508-147">O nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="14508-147">The name of the property.</span></span> <span data-ttu-id="14508-148">Máximo de 32 caracteres.</span><span class="sxs-lookup"><span data-stu-id="14508-148">Maximum 32 characters.</span></span> <span data-ttu-id="14508-149">Não deve conter caracteres de controle, espaço em branco ou qualquer um dos seguintes:,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` , `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` ,</span><span class="sxs-lookup"><span data-stu-id="14508-149">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="14508-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14508-150">Required.</span></span>                |
| <span data-ttu-id="14508-151">tipo</span><span class="sxs-lookup"><span data-stu-id="14508-151">type</span></span>          | <span data-ttu-id="14508-152">String</span><span class="sxs-lookup"><span data-stu-id="14508-152">String</span></span>            | <span data-ttu-id="14508-153">O tipo de dados da propriedade.</span><span class="sxs-lookup"><span data-stu-id="14508-153">The data type of the property.</span></span> <span data-ttu-id="14508-154">Os valores possíveis são: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`.</span><span class="sxs-lookup"><span data-stu-id="14508-154">Possible values are: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`.</span></span> <span data-ttu-id="14508-155">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14508-155">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="14508-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14508-156">JSON representation</span></span>

<span data-ttu-id="14508-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="14508-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.property",
  "baseType": null
}-->

```json
{
  "aliases": [ "String" ],
  "isQueryable": true,
  "isRefinable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "labels": [ "String" ],
  "name": "String",
  "type": "String"
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
