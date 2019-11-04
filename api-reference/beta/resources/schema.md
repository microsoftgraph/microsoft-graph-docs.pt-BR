---
title: tipo de recurso de esquema
description: Descreve o tipo de conteúdo e como indexar cada propriedade em itens em uma conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8bd5d47f444d7054aecbf7b0a63e57643837a340
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938783"
---
# <a name="schema-resource-type"></a><span data-ttu-id="2ebae-103">tipo de recurso de esquema</span><span class="sxs-lookup"><span data-stu-id="2ebae-103">schema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ebae-104">Descreve o tipo de conteúdo e como indexar cada propriedade em itens em uma [conexão](externalconnection.md)de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2ebae-104">Describes the type of content and how to index each property in items in a Microsoft Search [connection](externalconnection.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2ebae-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="2ebae-105">Methods</span></span>

| <span data-ttu-id="2ebae-106">Método</span><span class="sxs-lookup"><span data-stu-id="2ebae-106">Method</span></span>                                                    | <span data-ttu-id="2ebae-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2ebae-107">Return Type</span></span>                   | <span data-ttu-id="2ebae-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ebae-108">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="2ebae-109">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="2ebae-109">Create schema</span></span>](../api/externalconnection-post-schema.md) | <span data-ttu-id="2ebae-110">Nenhum *ou* [esquema](schema.md)</span><span class="sxs-lookup"><span data-stu-id="2ebae-110">None *or* [schema](schema.md)</span></span> | <span data-ttu-id="2ebae-111">Registrar o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="2ebae-111">Register connection schema.</span></span> |
| [<span data-ttu-id="2ebae-112">Obter esquema</span><span class="sxs-lookup"><span data-stu-id="2ebae-112">Get schema</span></span>](../api/schema-get.md)                        | [<span data-ttu-id="2ebae-113">esquemas</span><span class="sxs-lookup"><span data-stu-id="2ebae-113">schema</span></span>](schema.md)           | <span data-ttu-id="2ebae-114">Ler as propriedades de um objeto Schema.</span><span class="sxs-lookup"><span data-stu-id="2ebae-114">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2ebae-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ebae-115">Properties</span></span>

| <span data-ttu-id="2ebae-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ebae-116">Property</span></span>   | <span data-ttu-id="2ebae-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ebae-117">Type</span></span>                               | <span data-ttu-id="2ebae-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ebae-118">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="2ebae-119">baseType</span><span class="sxs-lookup"><span data-stu-id="2ebae-119">baseType</span></span>   | <span data-ttu-id="2ebae-120">String</span><span class="sxs-lookup"><span data-stu-id="2ebae-120">String</span></span>                             | <span data-ttu-id="2ebae-121">Os valores possíveis são: `microsoft.graph.externalItem` e `microsoft.graph.externalFile`.</span><span class="sxs-lookup"><span data-stu-id="2ebae-121">Possible values are `microsoft.graph.externalItem` and `microsoft.graph.externalFile`.</span></span> <span data-ttu-id="2ebae-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ebae-122">Required.</span></span> |
| <span data-ttu-id="2ebae-123">properties</span><span class="sxs-lookup"><span data-stu-id="2ebae-123">properties</span></span> | <span data-ttu-id="2ebae-124">coleção [Property](property.md)</span><span class="sxs-lookup"><span data-stu-id="2ebae-124">[property](property.md) collection</span></span> | <span data-ttu-id="2ebae-125">As propriedades definidas para os itens na conexão.</span><span class="sxs-lookup"><span data-stu-id="2ebae-125">The properties defined for the items in the connection.</span></span> <span data-ttu-id="2ebae-126">O número mínimo de propriedades é um, o máximo é 64.</span><span class="sxs-lookup"><span data-stu-id="2ebae-126">The minimum number of properties is one, the maximum is 64.</span></span> <span data-ttu-id="2ebae-127">Obrigatório quando `baseType` está definido como `microsoft.graph.externalItem`.</span><span class="sxs-lookup"><span data-stu-id="2ebae-127">Required when `baseType` is set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="2ebae-128">Ignorado quando `baseType` está definido como `microsoft.graph.externalFile`.</span><span class="sxs-lookup"><span data-stu-id="2ebae-128">Ignored when `baseType` is set to `microsoft.graph.externalFile`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2ebae-129">Relações</span><span class="sxs-lookup"><span data-stu-id="2ebae-129">Relationships</span></span>

<span data-ttu-id="2ebae-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ebae-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ebae-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ebae-131">JSON representation</span></span>

<span data-ttu-id="2ebae-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ebae-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schema",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "baseType": "String",
  "id": "String (identifier)",
  "properties": [{"@odata.type": "microsoft.graph.property"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "schema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
