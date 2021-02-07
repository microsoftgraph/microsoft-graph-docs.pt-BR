---
title: Tipo de recurso multiValueLegacyExtendedProperty
description: Uma propriedade estendida que contém uma coleção de valores.
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4d6139259616c6d347387b515f16e4b9ef5e4ddf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131520"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="688e8-103">Tipo de recurso multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="688e8-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="688e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="688e8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="688e8-105">Uma propriedade estendida que contém uma coleção de valores.</span><span class="sxs-lookup"><span data-stu-id="688e8-105">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="688e8-106">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="688e8-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="688e8-107">Methods</span><span class="sxs-lookup"><span data-stu-id="688e8-107">Methods</span></span>

| <span data-ttu-id="688e8-108">Método</span><span class="sxs-lookup"><span data-stu-id="688e8-108">Method</span></span>           | <span data-ttu-id="688e8-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="688e8-109">Return Type</span></span>    |<span data-ttu-id="688e8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="688e8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="688e8-111">Post</span><span class="sxs-lookup"><span data-stu-id="688e8-111">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="688e8-p101">Uma instância de recurso compatível: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) ou [contactFolder](../resources/contactfolder.md). Observe que o grupo [postar](../resources/post.md) não é compatível.</span><span class="sxs-lookup"><span data-stu-id="688e8-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="688e8-114">Crie uma **multiValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível.</span><span class="sxs-lookup"><span data-stu-id="688e8-114">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="688e8-115">Get</span><span class="sxs-lookup"><span data-stu-id="688e8-115">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="688e8-116">Uma instância de recurso compatível ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) ou o grupo [post](../resources/post.md)) expandida com um objeto [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="688e8-116">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="688e8-117">Obtenha uma instância de recurso com uma propriedade estendida usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="688e8-117">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="688e8-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="688e8-118">Properties</span></span>
| <span data-ttu-id="688e8-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="688e8-119">Property</span></span>     | <span data-ttu-id="688e8-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="688e8-120">Type</span></span>   |<span data-ttu-id="688e8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="688e8-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="688e8-122">id</span><span class="sxs-lookup"><span data-stu-id="688e8-122">id</span></span>|<span data-ttu-id="688e8-123">string</span><span class="sxs-lookup"><span data-stu-id="688e8-123">string</span></span>|<span data-ttu-id="688e8-p102">O identificador da propriedade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="688e8-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="688e8-126">valor</span><span class="sxs-lookup"><span data-stu-id="688e8-126">value</span></span>|<span data-ttu-id="688e8-127">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="688e8-127">string collection</span></span>|<span data-ttu-id="688e8-128">Uma coleção de valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="688e8-128">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="688e8-129">Relações</span><span class="sxs-lookup"><span data-stu-id="688e8-129">Relationships</span></span>
<span data-ttu-id="688e8-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="688e8-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="688e8-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="688e8-131">JSON representation</span></span>

<span data-ttu-id="688e8-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="688e8-132">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

