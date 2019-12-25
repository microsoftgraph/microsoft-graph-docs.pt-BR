---
title: tipo de recurso Property
description: Uma definição de propriedade de esquema para uma conexão do Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 087afe3e753ab68369899c0f0db07e93319e3687
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870149"
---
# <a name="property-resource-type"></a><span data-ttu-id="486a8-103">tipo de recurso Property</span><span class="sxs-lookup"><span data-stu-id="486a8-103">property resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="486a8-104">Uma definição de propriedade de [esquema](schema.md) para uma [conexão](externalconnection.md)do Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="486a8-104">A [schema](schema.md) property definition for a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="486a8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="486a8-105">Properties</span></span>

| <span data-ttu-id="486a8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="486a8-106">Property</span></span>      | <span data-ttu-id="486a8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="486a8-107">Type</span></span>    | <span data-ttu-id="486a8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="486a8-108">Description</span></span>                                        |
|:--------------|:--------|:---------------------------------------------------|
| <span data-ttu-id="486a8-109">IsQuery</span><span class="sxs-lookup"><span data-stu-id="486a8-109">isQueryable</span></span>   | <span data-ttu-id="486a8-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="486a8-110">Boolean</span></span> | <span data-ttu-id="486a8-111">Especifica se a propriedade é consultável.</span><span class="sxs-lookup"><span data-stu-id="486a8-111">Specifies if the property is queryable.</span></span> <span data-ttu-id="486a8-112">Propriedades consultáveis podem ser usadas em [consultas de idioma de consulta de palavra-chave (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span><span class="sxs-lookup"><span data-stu-id="486a8-112">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="486a8-113">Opcional.</span><span class="sxs-lookup"><span data-stu-id="486a8-113">Optional.</span></span>  |
| <span data-ttu-id="486a8-114">isretrievable</span><span class="sxs-lookup"><span data-stu-id="486a8-114">isRetrievable</span></span> | <span data-ttu-id="486a8-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="486a8-115">Boolean</span></span> | <span data-ttu-id="486a8-116">Especifica se a propriedade é recuperável.</span><span class="sxs-lookup"><span data-stu-id="486a8-116">Specifies if the property is retrievable.</span></span> <span data-ttu-id="486a8-117">As propriedades recuperáveis são retornadas no conjunto de resultados quando os itens são retornados pela API de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="486a8-117">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="486a8-118">As propriedades recuperáveis também estão disponíveis para adicionar ao modelo de exibição usado para renderizar os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="486a8-118">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="486a8-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="486a8-119">Optional.</span></span> |
| <span data-ttu-id="486a8-120">IsSearchable</span><span class="sxs-lookup"><span data-stu-id="486a8-120">isSearchable</span></span>  | <span data-ttu-id="486a8-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="486a8-121">Boolean</span></span> | <span data-ttu-id="486a8-122">Especifica se a propriedade é pesquisável.</span><span class="sxs-lookup"><span data-stu-id="486a8-122">Specifies if the property is searchable.</span></span> <span data-ttu-id="486a8-123">Somente propriedades do tipo `String` ou `StringCollection` podem ser pesquisáveis.</span><span class="sxs-lookup"><span data-stu-id="486a8-123">Only properties of type `String` or `StringCollection` can be searchable.</span></span> <span data-ttu-id="486a8-124">As propriedades não pesquisáveis não são adicionadas ao índice de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="486a8-124">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="486a8-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="486a8-125">Optional.</span></span> |
| <span data-ttu-id="486a8-126">nome</span><span class="sxs-lookup"><span data-stu-id="486a8-126">name</span></span>          | <span data-ttu-id="486a8-127">String</span><span class="sxs-lookup"><span data-stu-id="486a8-127">String</span></span>  | <span data-ttu-id="486a8-128">O nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="486a8-128">The name of the property.</span></span> <span data-ttu-id="486a8-129">Máximo de 32 caracteres.</span><span class="sxs-lookup"><span data-stu-id="486a8-129">Maximum 32 characters.</span></span> <span data-ttu-id="486a8-130">Não deve conter caracteres de controle, espaço em branco ou qualquer um dos `:`seguintes `;`: `,`, `(`, `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?`,,,,,,,,,,,,, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`,,,,,,,,,,,,,,,</span><span class="sxs-lookup"><span data-stu-id="486a8-130">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="486a8-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="486a8-131">Required.</span></span>                |
| <span data-ttu-id="486a8-132">type</span><span class="sxs-lookup"><span data-stu-id="486a8-132">type</span></span>          | <span data-ttu-id="486a8-133">String</span><span class="sxs-lookup"><span data-stu-id="486a8-133">String</span></span>  | <span data-ttu-id="486a8-134">O tipo de dados da propriedade.</span><span class="sxs-lookup"><span data-stu-id="486a8-134">The data type of the property.</span></span> <span data-ttu-id="486a8-135">Os valores possíveis são: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`.</span><span class="sxs-lookup"><span data-stu-id="486a8-135">Possible values are: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`.</span></span> <span data-ttu-id="486a8-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="486a8-136">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="486a8-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="486a8-137">JSON representation</span></span>

<span data-ttu-id="486a8-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="486a8-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.property",
  "baseType": null
}-->

```json
{
  "isQueryable": true,
  "isRetrievable": true,
  "isSearchable": true,
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
