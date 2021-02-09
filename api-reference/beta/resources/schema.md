---
title: tipo de recurso schema
description: O esquema de conexão determina como o conteúdo adicionado a uma conexão será usado em várias experiências do Microsoft Graph.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 88509a885a528f9ef2d55cd84381db493e128003
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156354"
---
# <a name="schema-resource-type"></a><span data-ttu-id="9cef3-103">tipo de recurso schema</span><span class="sxs-lookup"><span data-stu-id="9cef3-103">schema resource type</span></span>

<span data-ttu-id="9cef3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cef3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cef3-105">O [esquema](externalconnection.md) de conexão determina como o conteúdo externo será usado em várias experiências do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9cef3-105">The [connection](externalconnection.md) schema determines how your external content will be used in various Microsoft Graph experiences.</span></span> <span data-ttu-id="9cef3-106">O esquema é uma lista simples de todas as propriedades que você planeja adicionar à conexão, juntamente com seus atributos, rótulos e aliases.</span><span class="sxs-lookup"><span data-stu-id="9cef3-106">Schema is a flat list of all the properties that you plan to add to the connection along with their attributes, labels, and aliases.</span></span> <span data-ttu-id="9cef3-107">Você deve registrá-lo antes de adicionar itens na conexão.</span><span class="sxs-lookup"><span data-stu-id="9cef3-107">You must register the schema before adding items into the connection.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="9cef3-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="9cef3-108">Methods</span></span>

| <span data-ttu-id="9cef3-109">Método</span><span class="sxs-lookup"><span data-stu-id="9cef3-109">Method</span></span>                                                    | <span data-ttu-id="9cef3-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9cef3-110">Return Type</span></span>                   | <span data-ttu-id="9cef3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cef3-111">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="9cef3-112">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="9cef3-112">Create schema</span></span>](../api/externalconnection-post-schema.md) | <span data-ttu-id="9cef3-113">Nenhum *ou* [esquema](schema.md)</span><span class="sxs-lookup"><span data-stu-id="9cef3-113">None *or* [schema](schema.md)</span></span> | <span data-ttu-id="9cef3-114">Registre o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="9cef3-114">Register connection schema.</span></span> |
| [<span data-ttu-id="9cef3-115">Obter esquema</span><span class="sxs-lookup"><span data-stu-id="9cef3-115">Get schema</span></span>](../api/schema-get.md)                        | [<span data-ttu-id="9cef3-116">schema</span><span class="sxs-lookup"><span data-stu-id="9cef3-116">schema</span></span>](schema.md)           | <span data-ttu-id="9cef3-117">Leia as propriedades de um objeto schema.</span><span class="sxs-lookup"><span data-stu-id="9cef3-117">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9cef3-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9cef3-118">Properties</span></span>

| <span data-ttu-id="9cef3-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9cef3-119">Property</span></span>   | <span data-ttu-id="9cef3-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9cef3-120">Type</span></span>                               | <span data-ttu-id="9cef3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9cef3-121">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="9cef3-122">baseType</span><span class="sxs-lookup"><span data-stu-id="9cef3-122">baseType</span></span>   | <span data-ttu-id="9cef3-123">String</span><span class="sxs-lookup"><span data-stu-id="9cef3-123">String</span></span>                             | <span data-ttu-id="9cef3-124">Deve ser definida como `microsoft.graph.externalItem`.</span><span class="sxs-lookup"><span data-stu-id="9cef3-124">Must be set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="9cef3-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9cef3-125">Required.</span></span> |
| <span data-ttu-id="9cef3-126">properties</span><span class="sxs-lookup"><span data-stu-id="9cef3-126">properties</span></span> | <span data-ttu-id="9cef3-127">[coleção de](property.md) propriedades</span><span class="sxs-lookup"><span data-stu-id="9cef3-127">[property](property.md) collection</span></span> | <span data-ttu-id="9cef3-128">As propriedades definidas para os itens na conexão.</span><span class="sxs-lookup"><span data-stu-id="9cef3-128">The properties defined for the items in the connection.</span></span> <span data-ttu-id="9cef3-129">O número mínimo de propriedades é um, o máximo é 128.</span><span class="sxs-lookup"><span data-stu-id="9cef3-129">The minimum number of properties is one, the maximum is 128.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9cef3-130">Relações</span><span class="sxs-lookup"><span data-stu-id="9cef3-130">Relationships</span></span>

<span data-ttu-id="9cef3-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9cef3-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9cef3-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9cef3-132">JSON representation</span></span>

<span data-ttu-id="9cef3-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9cef3-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schema",
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


