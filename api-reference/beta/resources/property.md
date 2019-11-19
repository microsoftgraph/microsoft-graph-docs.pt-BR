---
title: tipo de recurso Property
description: Uma definição de propriedade de esquema para uma conexão do Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 465ad0824bf46949476304905bf0fea5c3ff6271
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703767"
---
# <a name="property-resource-type"></a><span data-ttu-id="651b2-103">tipo de recurso Property</span><span class="sxs-lookup"><span data-stu-id="651b2-103">property resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="651b2-104">Uma definição de propriedade de [esquema](schema.md) para uma [conexão](externalconnection.md)do Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="651b2-104">A [schema](schema.md) property definition for a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="651b2-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="651b2-105">Properties</span></span>

| <span data-ttu-id="651b2-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="651b2-106">Property</span></span>      | <span data-ttu-id="651b2-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="651b2-107">Type</span></span>    | <span data-ttu-id="651b2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="651b2-108">Description</span></span>                                        |
|:--------------|:--------|:---------------------------------------------------|
| <span data-ttu-id="651b2-109">IsQuery</span><span class="sxs-lookup"><span data-stu-id="651b2-109">isQueryable</span></span>   | <span data-ttu-id="651b2-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="651b2-110">Boolean</span></span> | <span data-ttu-id="651b2-111">Especifica se a propriedade é consultável.</span><span class="sxs-lookup"><span data-stu-id="651b2-111">Specifies if the property is queryable.</span></span> <span data-ttu-id="651b2-112">Propriedades consultáveis podem ser usadas em [consultas de idioma de consulta de palavra-chave (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span><span class="sxs-lookup"><span data-stu-id="651b2-112">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="651b2-113">Opcional.</span><span class="sxs-lookup"><span data-stu-id="651b2-113">Optional.</span></span>  |
| <span data-ttu-id="651b2-114">isretrievable</span><span class="sxs-lookup"><span data-stu-id="651b2-114">isRetrievable</span></span> | <span data-ttu-id="651b2-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="651b2-115">Boolean</span></span> | <span data-ttu-id="651b2-116">Especifica se a propriedade é recuperável.</span><span class="sxs-lookup"><span data-stu-id="651b2-116">Specifies if the property is retrievable.</span></span> <span data-ttu-id="651b2-117">As propriedades recuperáveis são retornadas no conjunto de resultados quando os itens são retornados pela API de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="651b2-117">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="651b2-118">As propriedades recuperáveis também estão disponíveis para adicionar ao modelo de exibição usado para renderizar os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="651b2-118">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="651b2-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="651b2-119">Optional.</span></span> |
| <span data-ttu-id="651b2-120">IsSearchable</span><span class="sxs-lookup"><span data-stu-id="651b2-120">isSearchable</span></span>  | <span data-ttu-id="651b2-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="651b2-121">Boolean</span></span> | <span data-ttu-id="651b2-122">Especifica se a propriedade é pesquisável.</span><span class="sxs-lookup"><span data-stu-id="651b2-122">Specifies if the property is searchable.</span></span> <span data-ttu-id="651b2-123">Somente propriedades do tipo `String` ou `Collection(String)` podem ser pesquisáveis.</span><span class="sxs-lookup"><span data-stu-id="651b2-123">Only properties of type `String` or `Collection(String)` can be searchable.</span></span> <span data-ttu-id="651b2-124">As propriedades não pesquisáveis não são adicionadas ao índice de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="651b2-124">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="651b2-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="651b2-125">Optional.</span></span> |
| <span data-ttu-id="651b2-126">name</span><span class="sxs-lookup"><span data-stu-id="651b2-126">name</span></span>          | <span data-ttu-id="651b2-127">String</span><span class="sxs-lookup"><span data-stu-id="651b2-127">String</span></span>  | <span data-ttu-id="651b2-128">O nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="651b2-128">The name of the property.</span></span> <span data-ttu-id="651b2-129">Máximo de 32 caracteres.</span><span class="sxs-lookup"><span data-stu-id="651b2-129">Maximum 32 characters.</span></span> <span data-ttu-id="651b2-130">Não deve conter caracteres de controle, espaço em branco ou qualquer um dos `:`seguintes `;`: `,`, `(`, `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?`,,,,,,,,,,,,, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`,,,,,,,,,,,,,,,</span><span class="sxs-lookup"><span data-stu-id="651b2-130">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="651b2-131">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="651b2-131">Required.</span></span>                |
| <span data-ttu-id="651b2-132">type</span><span class="sxs-lookup"><span data-stu-id="651b2-132">type</span></span>          | <span data-ttu-id="651b2-133">String</span><span class="sxs-lookup"><span data-stu-id="651b2-133">String</span></span>  | <span data-ttu-id="651b2-134">O tipo de dados da propriedade.</span><span class="sxs-lookup"><span data-stu-id="651b2-134">The data type of the property.</span></span> <span data-ttu-id="651b2-135">Os valores possíveis são: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `Collection(String)`, `Collection(Int64)`, `Collection(Double)`, `Collection(DateTime)`.</span><span class="sxs-lookup"><span data-stu-id="651b2-135">Possible values are: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `Collection(String)`, `Collection(Int64)`, `Collection(Double)`, `Collection(DateTime)`.</span></span> <span data-ttu-id="651b2-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="651b2-136">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="651b2-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="651b2-137">JSON representation</span></span>

<span data-ttu-id="651b2-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="651b2-138">The following is a JSON representation of the resource.</span></span>

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
