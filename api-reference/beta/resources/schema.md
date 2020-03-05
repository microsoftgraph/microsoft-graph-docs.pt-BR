---
title: tipo de recurso de esquema
description: Descreve o tipo de conteúdo e como indexar cada propriedade em itens em uma conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 40c31536f8d53c46563fda4205d34deee0501beb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520953"
---
# <a name="schema-resource-type"></a><span data-ttu-id="32652-103">tipo de recurso de esquema</span><span class="sxs-lookup"><span data-stu-id="32652-103">schema resource type</span></span>

<span data-ttu-id="32652-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="32652-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32652-105">Descreve o tipo de conteúdo e como indexar cada propriedade em itens em uma [conexão](externalconnection.md)de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="32652-105">Describes the type of content and how to index each property in items in a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="32652-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="32652-106">Methods</span></span>

| <span data-ttu-id="32652-107">Método</span><span class="sxs-lookup"><span data-stu-id="32652-107">Method</span></span>                                                    | <span data-ttu-id="32652-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="32652-108">Return Type</span></span>                   | <span data-ttu-id="32652-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="32652-109">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="32652-110">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="32652-110">Create schema</span></span>](../api/externalconnection-post-schema.md) | <span data-ttu-id="32652-111">Nenhum *ou* [esquema](schema.md)</span><span class="sxs-lookup"><span data-stu-id="32652-111">None *or* [schema](schema.md)</span></span> | <span data-ttu-id="32652-112">Registrar o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="32652-112">Register connection schema.</span></span> |
| [<span data-ttu-id="32652-113">Obter esquema</span><span class="sxs-lookup"><span data-stu-id="32652-113">Get schema</span></span>](../api/schema-get.md)                        | [<span data-ttu-id="32652-114">schema</span><span class="sxs-lookup"><span data-stu-id="32652-114">schema</span></span>](schema.md)           | <span data-ttu-id="32652-115">Ler as propriedades de um objeto Schema.</span><span class="sxs-lookup"><span data-stu-id="32652-115">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="32652-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32652-116">Properties</span></span>

| <span data-ttu-id="32652-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32652-117">Property</span></span>   | <span data-ttu-id="32652-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="32652-118">Type</span></span>                               | <span data-ttu-id="32652-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="32652-119">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="32652-120">baseType</span><span class="sxs-lookup"><span data-stu-id="32652-120">baseType</span></span>   | <span data-ttu-id="32652-121">String</span><span class="sxs-lookup"><span data-stu-id="32652-121">String</span></span>                             | <span data-ttu-id="32652-122">Os valores possíveis são: `microsoft.graph.externalItem` e `microsoft.graph.externalFile`.</span><span class="sxs-lookup"><span data-stu-id="32652-122">Possible values are `microsoft.graph.externalItem` and `microsoft.graph.externalFile`.</span></span> <span data-ttu-id="32652-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32652-123">Required.</span></span> |
| <span data-ttu-id="32652-124">properties</span><span class="sxs-lookup"><span data-stu-id="32652-124">properties</span></span> | <span data-ttu-id="32652-125">coleção [Property](property.md)</span><span class="sxs-lookup"><span data-stu-id="32652-125">[property](property.md) collection</span></span> | <span data-ttu-id="32652-126">As propriedades definidas para os itens na conexão.</span><span class="sxs-lookup"><span data-stu-id="32652-126">The properties defined for the items in the connection.</span></span> <span data-ttu-id="32652-127">O número mínimo de propriedades é um, o máximo é 64.</span><span class="sxs-lookup"><span data-stu-id="32652-127">The minimum number of properties is one, the maximum is 64.</span></span> <span data-ttu-id="32652-128">Obrigatório quando `baseType` está definido como `microsoft.graph.externalItem`.</span><span class="sxs-lookup"><span data-stu-id="32652-128">Required when `baseType` is set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="32652-129">Ignorado quando `baseType` está definido como `microsoft.graph.externalFile`.</span><span class="sxs-lookup"><span data-stu-id="32652-129">Ignored when `baseType` is set to `microsoft.graph.externalFile`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="32652-130">Relações</span><span class="sxs-lookup"><span data-stu-id="32652-130">Relationships</span></span>

<span data-ttu-id="32652-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="32652-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32652-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32652-132">JSON representation</span></span>

<span data-ttu-id="32652-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32652-133">The following is a JSON representation of the resource.</span></span>

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
