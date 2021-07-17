---
title: tipo de recurso de esquema
description: O esquema de conexão determina como o conteúdo adicionado a uma conexão será usado em várias experiências Graph Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 649f9e0ae8e0162e9fa4f976d5158e23bfb49b05
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467597"
---
# <a name="schema-resource-type"></a><span data-ttu-id="ef1da-103">tipo de recurso de esquema</span><span class="sxs-lookup"><span data-stu-id="ef1da-103">schema resource type</span></span>

<span data-ttu-id="ef1da-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="ef1da-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef1da-105">O [esquema](externalconnectors-externalconnection.md) de conexão determina como seu conteúdo externo será usado em várias experiências Graph Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ef1da-105">The [connection](externalconnectors-externalconnection.md) schema determines how your external content will be used in various Microsoft Graph experiences.</span></span> <span data-ttu-id="ef1da-106">O esquema é uma lista simples de todas as propriedades que você planeja adicionar à conexão, juntamente com seus atributos, rótulos e aliases.</span><span class="sxs-lookup"><span data-stu-id="ef1da-106">Schema is a flat list of all the properties that you plan to add to the connection along with their attributes, labels, and aliases.</span></span> <span data-ttu-id="ef1da-107">Você deve registrá-lo antes de adicionar itens na conexão.</span><span class="sxs-lookup"><span data-stu-id="ef1da-107">You must register the schema before adding items into the connection.</span></span>

## <a name="methods"></a><span data-ttu-id="ef1da-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="ef1da-108">Methods</span></span>

| <span data-ttu-id="ef1da-109">Método</span><span class="sxs-lookup"><span data-stu-id="ef1da-109">Method</span></span>                                                    | <span data-ttu-id="ef1da-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ef1da-110">Return Type</span></span>                   | <span data-ttu-id="ef1da-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef1da-111">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="ef1da-112">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="ef1da-112">Create schema</span></span>](../api/externalconnectors-externalconnection-post-schema.md) | <span data-ttu-id="ef1da-113">Nenhum *ou* [esquema](externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="ef1da-113">None *or* [schema](externalconnectors-schema.md)</span></span> | <span data-ttu-id="ef1da-114">Registrar esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="ef1da-114">Register connection schema.</span></span> |
| [<span data-ttu-id="ef1da-115">Obter esquema</span><span class="sxs-lookup"><span data-stu-id="ef1da-115">Get schema</span></span>](../api/externalconnectors-schema-get.md)                        | [<span data-ttu-id="ef1da-116">schema</span><span class="sxs-lookup"><span data-stu-id="ef1da-116">schema</span></span>](externalconnectors-schema.md)           | <span data-ttu-id="ef1da-117">Ler propriedades de um objeto de esquema.</span><span class="sxs-lookup"><span data-stu-id="ef1da-117">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ef1da-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef1da-118">Properties</span></span>

| <span data-ttu-id="ef1da-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef1da-119">Property</span></span>   | <span data-ttu-id="ef1da-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef1da-120">Type</span></span>                               | <span data-ttu-id="ef1da-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef1da-121">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="ef1da-122">baseType</span><span class="sxs-lookup"><span data-stu-id="ef1da-122">baseType</span></span>   | <span data-ttu-id="ef1da-123">String</span><span class="sxs-lookup"><span data-stu-id="ef1da-123">String</span></span>                             | <span data-ttu-id="ef1da-124">Deve ser definida como `microsoft.graph.externalItem`.</span><span class="sxs-lookup"><span data-stu-id="ef1da-124">Must be set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="ef1da-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef1da-125">Required.</span></span> |
| <span data-ttu-id="ef1da-126">properties</span><span class="sxs-lookup"><span data-stu-id="ef1da-126">properties</span></span> | <span data-ttu-id="ef1da-127">[coleção property](externalconnectors-property.md)</span><span class="sxs-lookup"><span data-stu-id="ef1da-127">[property](externalconnectors-property.md) collection</span></span> | <span data-ttu-id="ef1da-128">As propriedades definidas para os itens na conexão.</span><span class="sxs-lookup"><span data-stu-id="ef1da-128">The properties defined for the items in the connection.</span></span> <span data-ttu-id="ef1da-129">O número mínimo de propriedades é um, o máximo é 128.</span><span class="sxs-lookup"><span data-stu-id="ef1da-129">The minimum number of properties is one, the maximum is 128.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ef1da-130">Relações</span><span class="sxs-lookup"><span data-stu-id="ef1da-130">Relationships</span></span>

<span data-ttu-id="ef1da-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ef1da-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef1da-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef1da-132">JSON representation</span></span>

<span data-ttu-id="ef1da-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ef1da-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.externalConnectors.schema",
  "keyProperty": "id"
}-->

```json
{
  "baseType": "String",
  "id": "String (identifier)",
  "properties": [
    {
      "name": "String",
      "type": "String",
    }
  ]
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
