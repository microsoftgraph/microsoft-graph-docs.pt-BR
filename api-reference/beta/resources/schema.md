---
title: tipo de recurso de esquema
description: O esquema de conexão determina como o conteúdo adicionado a uma conexão será usado em várias experiências do Microsoft Graph.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: ff14f04adb31d99aadec15cb9368e09a098c7a26
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192865"
---
# <a name="schema-resource-type"></a><span data-ttu-id="9d9ca-103">tipo de recurso de esquema</span><span class="sxs-lookup"><span data-stu-id="9d9ca-103">schema resource type</span></span>

<span data-ttu-id="9d9ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d9ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d9ca-105">O esquema de [conexão](externalconnection.md) determina como o conteúdo externo será usado em várias experiências do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-105">The [connection](externalconnection.md) schema determines how your external content will be used in various Microsoft Graph experiences.</span></span> <span data-ttu-id="9d9ca-106">Schema é uma lista simples de todas as propriedades que você planeja adicionar à conexão junto com seus atributos, rótulos e aliases.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-106">Schema is a flat list of all the properties that you plan to add to the connection along with their attributes, labels, and aliases.</span></span> <span data-ttu-id="9d9ca-107">Você deve registrar o esquema antes de adicionar itens à conexão.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-107">You must register the schema before adding items into the connection.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="9d9ca-108">Methods</span><span class="sxs-lookup"><span data-stu-id="9d9ca-108">Methods</span></span>

| <span data-ttu-id="9d9ca-109">Método</span><span class="sxs-lookup"><span data-stu-id="9d9ca-109">Method</span></span>                                                    | <span data-ttu-id="9d9ca-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9d9ca-110">Return Type</span></span>                   | <span data-ttu-id="9d9ca-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d9ca-111">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="9d9ca-112">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="9d9ca-112">Create schema</span></span>](../api/externalconnection-post-schema.md) | <span data-ttu-id="9d9ca-113">Nenhum *ou* [esquema](schema.md)</span><span class="sxs-lookup"><span data-stu-id="9d9ca-113">None *or* [schema](schema.md)</span></span> | <span data-ttu-id="9d9ca-114">Registrar o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-114">Register connection schema.</span></span> |
| [<span data-ttu-id="9d9ca-115">Obter esquema</span><span class="sxs-lookup"><span data-stu-id="9d9ca-115">Get schema</span></span>](../api/schema-get.md)                        | [<span data-ttu-id="9d9ca-116">schema</span><span class="sxs-lookup"><span data-stu-id="9d9ca-116">schema</span></span>](schema.md)           | <span data-ttu-id="9d9ca-117">Ler as propriedades de um objeto Schema.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-117">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9d9ca-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d9ca-118">Properties</span></span>

| <span data-ttu-id="9d9ca-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d9ca-119">Property</span></span>   | <span data-ttu-id="9d9ca-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d9ca-120">Type</span></span>                               | <span data-ttu-id="9d9ca-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d9ca-121">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="9d9ca-122">baseType</span><span class="sxs-lookup"><span data-stu-id="9d9ca-122">baseType</span></span>   | <span data-ttu-id="9d9ca-123">String</span><span class="sxs-lookup"><span data-stu-id="9d9ca-123">String</span></span>                             | <span data-ttu-id="9d9ca-124">Deve ser definida como `microsoft.graph.externalItem`.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-124">Must be set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="9d9ca-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-125">Required.</span></span> |
| <span data-ttu-id="9d9ca-126">properties</span><span class="sxs-lookup"><span data-stu-id="9d9ca-126">properties</span></span> | <span data-ttu-id="9d9ca-127">coleção [Property](property.md)</span><span class="sxs-lookup"><span data-stu-id="9d9ca-127">[property](property.md) collection</span></span> | <span data-ttu-id="9d9ca-128">As propriedades definidas para os itens na conexão.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-128">The properties defined for the items in the connection.</span></span> <span data-ttu-id="9d9ca-129">O número mínimo de propriedades é um, o máximo é 128.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-129">The minimum number of properties is one, the maximum is 128.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9d9ca-130">Relações</span><span class="sxs-lookup"><span data-stu-id="9d9ca-130">Relationships</span></span>

<span data-ttu-id="9d9ca-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d9ca-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d9ca-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d9ca-132">JSON representation</span></span>

<span data-ttu-id="9d9ca-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d9ca-133">The following is a JSON representation of the resource.</span></span>

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


