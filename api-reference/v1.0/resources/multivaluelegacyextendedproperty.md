---
title: Tipo de recurso multiValueLegacyExtendedProperty
description: Uma propriedade estendida que contém uma coleção de valores.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: da1a3aae766d3c8e223b8b34555529f7024e76ae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534210"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="2cc62-103">Tipo de recurso multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="2cc62-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="2cc62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cc62-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2cc62-105">Uma propriedade estendida que contém uma coleção de valores.</span><span class="sxs-lookup"><span data-stu-id="2cc62-105">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="2cc62-106">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="2cc62-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="2cc62-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="2cc62-107">Methods</span></span>

| <span data-ttu-id="2cc62-108">Método</span><span class="sxs-lookup"><span data-stu-id="2cc62-108">Method</span></span>           | <span data-ttu-id="2cc62-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2cc62-109">Return Type</span></span>    |<span data-ttu-id="2cc62-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cc62-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2cc62-111">Post</span><span class="sxs-lookup"><span data-stu-id="2cc62-111">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="2cc62-p101">Uma instância de recurso compatível: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) ou [contactFolder](../resources/contactfolder.md). Observe que o grupo [postar](../resources/post.md) não é compatível.</span><span class="sxs-lookup"><span data-stu-id="2cc62-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="2cc62-114">Crie uma **multiValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível.</span><span class="sxs-lookup"><span data-stu-id="2cc62-114">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="2cc62-115">Get</span><span class="sxs-lookup"><span data-stu-id="2cc62-115">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="2cc62-116">Uma instância de recurso compatível ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) ou o grupo [post](../resources/post.md)) expandida com um objeto [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="2cc62-116">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="2cc62-117">Obtenha uma instância de recurso com uma propriedade estendida usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="2cc62-117">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="2cc62-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2cc62-118">Properties</span></span>
| <span data-ttu-id="2cc62-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2cc62-119">Property</span></span>     | <span data-ttu-id="2cc62-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cc62-120">Type</span></span>   |<span data-ttu-id="2cc62-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cc62-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2cc62-122">id</span><span class="sxs-lookup"><span data-stu-id="2cc62-122">id</span></span>|<span data-ttu-id="2cc62-123">string</span><span class="sxs-lookup"><span data-stu-id="2cc62-123">string</span></span>|<span data-ttu-id="2cc62-p102">O identificador da propriedade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2cc62-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="2cc62-126">valor</span><span class="sxs-lookup"><span data-stu-id="2cc62-126">value</span></span>|<span data-ttu-id="2cc62-127">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2cc62-127">string collection</span></span>|<span data-ttu-id="2cc62-128">Uma coleção de valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="2cc62-128">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cc62-129">Relações</span><span class="sxs-lookup"><span data-stu-id="2cc62-129">Relationships</span></span>
<span data-ttu-id="2cc62-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2cc62-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2cc62-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2cc62-131">JSON representation</span></span>

<span data-ttu-id="2cc62-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2cc62-132">Here is a JSON representation of the resource.</span></span>

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
