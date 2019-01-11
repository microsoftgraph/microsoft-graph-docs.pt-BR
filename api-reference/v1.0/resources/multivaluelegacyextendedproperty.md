---
title: Tipo de recurso multiValueLegacyExtendedProperty
description: Uma propriedade estendida que contém uma coleção de valores.
localization_priority: Normal
ms.openlocfilehash: 87823559bad3e149ef3c4d4d6f21f43cf66c41fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827031"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="35186-103">Tipo de recurso multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="35186-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="35186-104">Uma propriedade estendida que contém uma coleção de valores.</span><span class="sxs-lookup"><span data-stu-id="35186-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="35186-105">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="35186-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="35186-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="35186-106">Methods</span></span>

| <span data-ttu-id="35186-107">Método</span><span class="sxs-lookup"><span data-stu-id="35186-107">Method</span></span>           | <span data-ttu-id="35186-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="35186-108">Return Type</span></span>    |<span data-ttu-id="35186-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="35186-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35186-110">Post</span><span class="sxs-lookup"><span data-stu-id="35186-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="35186-p101">Uma instância de recurso compatível: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) ou [contactFolder](../resources/contactfolder.md). Observe que o grupo [postar](../resources/post.md) não é compatível.</span><span class="sxs-lookup"><span data-stu-id="35186-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="35186-113">Crie uma **multiValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível.</span><span class="sxs-lookup"><span data-stu-id="35186-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="35186-114">Get</span><span class="sxs-lookup"><span data-stu-id="35186-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="35186-115">Uma instância de recurso compatível ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) ou o grupo [post](../resources/post.md)) expandida com um objeto [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="35186-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="35186-116">Obtenha uma instância de recurso com uma propriedade estendida usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="35186-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="35186-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35186-117">Properties</span></span>
| <span data-ttu-id="35186-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35186-118">Property</span></span>     | <span data-ttu-id="35186-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="35186-119">Type</span></span>   |<span data-ttu-id="35186-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="35186-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35186-121">id</span><span class="sxs-lookup"><span data-stu-id="35186-121">id</span></span>|<span data-ttu-id="35186-122">string</span><span class="sxs-lookup"><span data-stu-id="35186-122">string</span></span>|<span data-ttu-id="35186-p102">O identificador da propriedade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35186-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="35186-125">valor</span><span class="sxs-lookup"><span data-stu-id="35186-125">value</span></span>|<span data-ttu-id="35186-126">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="35186-126">string collection</span></span>|<span data-ttu-id="35186-127">Uma coleção de valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="35186-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35186-128">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="35186-128">Relationships</span></span>
<span data-ttu-id="35186-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35186-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="35186-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35186-130">JSON representation</span></span>

<span data-ttu-id="35186-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35186-131">Here is a JSON representation of the resource.</span></span>

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
