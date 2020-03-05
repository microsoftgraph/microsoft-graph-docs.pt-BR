---
title: tipo de recurso Property
description: Uma definição de propriedade de esquema para uma conexão do Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 48a61c9f26a7f5b90e41fc2cd36334d4061449dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521380"
---
# <a name="property-resource-type"></a><span data-ttu-id="2b20e-103">tipo de recurso Property</span><span class="sxs-lookup"><span data-stu-id="2b20e-103">property resource type</span></span>

<span data-ttu-id="2b20e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2b20e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b20e-105">Uma definição de propriedade de [esquema](schema.md) para uma [conexão](externalconnection.md)do Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="2b20e-105">A [schema](schema.md) property definition for a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="2b20e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b20e-106">Properties</span></span>

| <span data-ttu-id="2b20e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b20e-107">Property</span></span>      | <span data-ttu-id="2b20e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b20e-108">Type</span></span>    | <span data-ttu-id="2b20e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b20e-109">Description</span></span>                                        |
|:--------------|:--------|:---------------------------------------------------|
| <span data-ttu-id="2b20e-110">IsQuery</span><span class="sxs-lookup"><span data-stu-id="2b20e-110">isQueryable</span></span>   | <span data-ttu-id="2b20e-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b20e-111">Boolean</span></span> | <span data-ttu-id="2b20e-112">Especifica se a propriedade é consultável.</span><span class="sxs-lookup"><span data-stu-id="2b20e-112">Specifies if the property is queryable.</span></span> <span data-ttu-id="2b20e-113">Propriedades consultáveis podem ser usadas em [consultas de idioma de consulta de palavra-chave (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span><span class="sxs-lookup"><span data-stu-id="2b20e-113">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="2b20e-114">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2b20e-114">Optional.</span></span>  |
| <span data-ttu-id="2b20e-115">isretrievable</span><span class="sxs-lookup"><span data-stu-id="2b20e-115">isRetrievable</span></span> | <span data-ttu-id="2b20e-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b20e-116">Boolean</span></span> | <span data-ttu-id="2b20e-117">Especifica se a propriedade é recuperável.</span><span class="sxs-lookup"><span data-stu-id="2b20e-117">Specifies if the property is retrievable.</span></span> <span data-ttu-id="2b20e-118">As propriedades recuperáveis são retornadas no conjunto de resultados quando os itens são retornados pela API de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="2b20e-118">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="2b20e-119">As propriedades recuperáveis também estão disponíveis para adicionar ao modelo de exibição usado para renderizar os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="2b20e-119">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="2b20e-120">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2b20e-120">Optional.</span></span> |
| <span data-ttu-id="2b20e-121">IsSearchable</span><span class="sxs-lookup"><span data-stu-id="2b20e-121">isSearchable</span></span>  | <span data-ttu-id="2b20e-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b20e-122">Boolean</span></span> | <span data-ttu-id="2b20e-123">Especifica se a propriedade é pesquisável.</span><span class="sxs-lookup"><span data-stu-id="2b20e-123">Specifies if the property is searchable.</span></span> <span data-ttu-id="2b20e-124">Somente propriedades do tipo `String` ou `StringCollection` podem ser pesquisáveis.</span><span class="sxs-lookup"><span data-stu-id="2b20e-124">Only properties of type `String` or `StringCollection` can be searchable.</span></span> <span data-ttu-id="2b20e-125">As propriedades não pesquisáveis não são adicionadas ao índice de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="2b20e-125">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="2b20e-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2b20e-126">Optional.</span></span> |
| <span data-ttu-id="2b20e-127">nome</span><span class="sxs-lookup"><span data-stu-id="2b20e-127">name</span></span>          | <span data-ttu-id="2b20e-128">String</span><span class="sxs-lookup"><span data-stu-id="2b20e-128">String</span></span>  | <span data-ttu-id="2b20e-129">O nome da propriedade.</span><span class="sxs-lookup"><span data-stu-id="2b20e-129">The name of the property.</span></span> <span data-ttu-id="2b20e-130">Máximo de 32 caracteres.</span><span class="sxs-lookup"><span data-stu-id="2b20e-130">Maximum 32 characters.</span></span> <span data-ttu-id="2b20e-131">Não deve conter caracteres de controle, espaço em branco ou qualquer um dos `:`seguintes `;`: `,`, `(`, `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?`,,,,,,,,,,,,, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`,,,,,,,,,,,,,,,</span><span class="sxs-lookup"><span data-stu-id="2b20e-131">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="2b20e-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b20e-132">Required.</span></span>                |
| <span data-ttu-id="2b20e-133">type</span><span class="sxs-lookup"><span data-stu-id="2b20e-133">type</span></span>          | <span data-ttu-id="2b20e-134">String</span><span class="sxs-lookup"><span data-stu-id="2b20e-134">String</span></span>  | <span data-ttu-id="2b20e-135">O tipo de dados da propriedade.</span><span class="sxs-lookup"><span data-stu-id="2b20e-135">The data type of the property.</span></span> <span data-ttu-id="2b20e-136">Os valores possíveis são: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`.</span><span class="sxs-lookup"><span data-stu-id="2b20e-136">Possible values are: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`.</span></span> <span data-ttu-id="2b20e-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b20e-137">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2b20e-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b20e-138">JSON representation</span></span>

<span data-ttu-id="2b20e-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b20e-139">The following is a JSON representation of the resource.</span></span>

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
