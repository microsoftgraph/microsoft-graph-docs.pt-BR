---
title: tipo de recurso de esquema
description: Descreve o tipo de conteúdo e como indexar cada propriedade em itens em uma conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c7780cd7c31da98a618053febba1b75c5e318931
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990259"
---
# <a name="schema-resource-type"></a><span data-ttu-id="1a10c-103">tipo de recurso de esquema</span><span class="sxs-lookup"><span data-stu-id="1a10c-103">schema resource type</span></span>

<span data-ttu-id="1a10c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a10c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a10c-105">Descreve o tipo de conteúdo e como indexar cada propriedade em itens em uma [conexão](externalconnection.md)de pesquisa da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1a10c-105">Describes the type of content and how to index each property in items in a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="1a10c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="1a10c-106">Methods</span></span>

| <span data-ttu-id="1a10c-107">Método</span><span class="sxs-lookup"><span data-stu-id="1a10c-107">Method</span></span>                                                    | <span data-ttu-id="1a10c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1a10c-108">Return Type</span></span>                   | <span data-ttu-id="1a10c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a10c-109">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="1a10c-110">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="1a10c-110">Create schema</span></span>](../api/externalconnection-post-schema.md) | <span data-ttu-id="1a10c-111">Nenhum *ou* [esquema](schema.md)</span><span class="sxs-lookup"><span data-stu-id="1a10c-111">None *or* [schema](schema.md)</span></span> | <span data-ttu-id="1a10c-112">Registrar o esquema de conexão.</span><span class="sxs-lookup"><span data-stu-id="1a10c-112">Register connection schema.</span></span> |
| [<span data-ttu-id="1a10c-113">Obter esquema</span><span class="sxs-lookup"><span data-stu-id="1a10c-113">Get schema</span></span>](../api/schema-get.md)                        | [<span data-ttu-id="1a10c-114">schema</span><span class="sxs-lookup"><span data-stu-id="1a10c-114">schema</span></span>](schema.md)           | <span data-ttu-id="1a10c-115">Ler as propriedades de um objeto Schema.</span><span class="sxs-lookup"><span data-stu-id="1a10c-115">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1a10c-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a10c-116">Properties</span></span>

| <span data-ttu-id="1a10c-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a10c-117">Property</span></span>   | <span data-ttu-id="1a10c-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a10c-118">Type</span></span>                               | <span data-ttu-id="1a10c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a10c-119">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="1a10c-120">baseType</span><span class="sxs-lookup"><span data-stu-id="1a10c-120">baseType</span></span>   | <span data-ttu-id="1a10c-121">String</span><span class="sxs-lookup"><span data-stu-id="1a10c-121">String</span></span>                             | <span data-ttu-id="1a10c-122">Deve ser definida como `microsoft.graph.externalItem`.</span><span class="sxs-lookup"><span data-stu-id="1a10c-122">Must be set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="1a10c-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a10c-123">Required.</span></span> |
| <span data-ttu-id="1a10c-124">properties</span><span class="sxs-lookup"><span data-stu-id="1a10c-124">properties</span></span> | <span data-ttu-id="1a10c-125">coleção [Property](property.md)</span><span class="sxs-lookup"><span data-stu-id="1a10c-125">[property](property.md) collection</span></span> | <span data-ttu-id="1a10c-126">As propriedades definidas para os itens na conexão.</span><span class="sxs-lookup"><span data-stu-id="1a10c-126">The properties defined for the items in the connection.</span></span> <span data-ttu-id="1a10c-127">O número mínimo de propriedades é um, o máximo é 128.</span><span class="sxs-lookup"><span data-stu-id="1a10c-127">The minimum number of properties is one, the maximum is 128.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1a10c-128">Relações</span><span class="sxs-lookup"><span data-stu-id="1a10c-128">Relationships</span></span>

<span data-ttu-id="1a10c-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a10c-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a10c-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a10c-130">JSON representation</span></span>

<span data-ttu-id="1a10c-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a10c-131">The following is a JSON representation of the resource.</span></span>

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
