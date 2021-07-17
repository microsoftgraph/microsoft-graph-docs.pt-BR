---
title: tipo de recurso de esquema
description: O esquema de conexão determina como o conteúdo adicionado a uma conexão será usado em várias experiências Graph Microsoft.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c0ca5e88d9d4ac7d7b63dea49f8ff4aace8cc348
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467193"
---
# <a name="schema-resource-type"></a><span data-ttu-id="f99a7-103">tipo de recurso de esquema</span><span class="sxs-lookup"><span data-stu-id="f99a7-103">schema resource type</span></span>

<span data-ttu-id="f99a7-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="f99a7-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="f99a7-105">O [esquema](externalconnectors-externalconnection.md) de conexão determina como seu conteúdo externo será usado em várias experiências Graph Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f99a7-105">The [connection](externalconnectors-externalconnection.md) schema determines how your external content will be used in various Microsoft Graph experiences.</span></span> <span data-ttu-id="f99a7-106">O esquema é uma lista simples de todas as propriedades que você planeja adicionar à conexão, juntamente com seus atributos, rótulos e aliases.</span><span class="sxs-lookup"><span data-stu-id="f99a7-106">Schema is a flat list of all the properties that you plan to add to the connection along with their attributes, labels, and aliases.</span></span> <span data-ttu-id="f99a7-107">Você deve registrá-lo antes de adicionar itens na conexão.</span><span class="sxs-lookup"><span data-stu-id="f99a7-107">You must register the schema before adding items into the connection.</span></span>

## <a name="methods"></a><span data-ttu-id="f99a7-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="f99a7-108">Methods</span></span>
|<span data-ttu-id="f99a7-109">Método</span><span class="sxs-lookup"><span data-stu-id="f99a7-109">Method</span></span>|<span data-ttu-id="f99a7-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f99a7-110">Return type</span></span>|<span data-ttu-id="f99a7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f99a7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f99a7-112">Criar esquema</span><span class="sxs-lookup"><span data-stu-id="f99a7-112">Create schema</span></span>](../api/externalconnectors-schema-create.md)|[<span data-ttu-id="f99a7-113">schema</span><span class="sxs-lookup"><span data-stu-id="f99a7-113">schema</span></span>](../resources/externalconnectors-schema.md)|<span data-ttu-id="f99a7-114">Crie um novo [objeto de esquema.](../resources/externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="f99a7-114">Create a new [schema](../resources/externalconnectors-schema.md) object.</span></span>|
|[<span data-ttu-id="f99a7-115">Obter esquema</span><span class="sxs-lookup"><span data-stu-id="f99a7-115">Get schema</span></span>](../api/externalconnectors-schema-get.md)|[<span data-ttu-id="f99a7-116">schema</span><span class="sxs-lookup"><span data-stu-id="f99a7-116">schema</span></span>](../resources/externalconnectors-schema.md)|<span data-ttu-id="f99a7-117">Leia as propriedades e as relações de um [objeto de esquema.](../resources/externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="f99a7-117">Read the properties and relationships of a [schema](../resources/externalconnectors-schema.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f99a7-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f99a7-118">Properties</span></span>
|<span data-ttu-id="f99a7-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f99a7-119">Property</span></span>|<span data-ttu-id="f99a7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f99a7-120">Type</span></span>|<span data-ttu-id="f99a7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f99a7-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f99a7-122">baseType</span><span class="sxs-lookup"><span data-stu-id="f99a7-122">baseType</span></span>|<span data-ttu-id="f99a7-123">String</span><span class="sxs-lookup"><span data-stu-id="f99a7-123">String</span></span>|<span data-ttu-id="f99a7-124">Deve ser definida como `microsoft.graph.externalConnector.externalItem`.</span><span class="sxs-lookup"><span data-stu-id="f99a7-124">Must be set to `microsoft.graph.externalConnector.externalItem`.</span></span> <span data-ttu-id="f99a7-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f99a7-125">Required.</span></span>|
|<span data-ttu-id="f99a7-126">properties</span><span class="sxs-lookup"><span data-stu-id="f99a7-126">properties</span></span>|<span data-ttu-id="f99a7-127">[coleção property](../resources/externalconnectors-property.md)</span><span class="sxs-lookup"><span data-stu-id="f99a7-127">[property](../resources/externalconnectors-property.md) collection</span></span>|<span data-ttu-id="f99a7-128">As propriedades definidas para os itens na conexão.</span><span class="sxs-lookup"><span data-stu-id="f99a7-128">The properties defined for the items in the connection.</span></span> <span data-ttu-id="f99a7-129">O número mínimo de propriedades é um, o máximo é 128.</span><span class="sxs-lookup"><span data-stu-id="f99a7-129">The minimum number of properties is one, the maximum is 128.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f99a7-130">Relações</span><span class="sxs-lookup"><span data-stu-id="f99a7-130">Relationships</span></span>
<span data-ttu-id="f99a7-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f99a7-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f99a7-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f99a7-132">JSON representation</span></span>
<span data-ttu-id="f99a7-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f99a7-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.schema",
  "openType": false
}
-->
``` json
{
  "baseType": "String",
  "properties": [
    {
      "name": "String",
      "type": "String",
    }
  ]
}
```

