---
title: Tipo de recurso multiValueLegacyExtendedProperty
description: Uma propriedade estendida que contém uma coleção de valores.
ms.openlocfilehash: 9aa94465ca1a0fb30c4461b99336040c72e2c5c0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004691"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="e5567-103">Tipo de recurso multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="e5567-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="e5567-104">Uma propriedade estendida que contém uma coleção de valores.</span><span class="sxs-lookup"><span data-stu-id="e5567-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="e5567-105">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="e5567-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="e5567-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e5567-106">Methods</span></span>

| <span data-ttu-id="e5567-107">Método</span><span class="sxs-lookup"><span data-stu-id="e5567-107">Method</span></span>           | <span data-ttu-id="e5567-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e5567-108">Return Type</span></span>    |<span data-ttu-id="e5567-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5567-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e5567-110">Post</span><span class="sxs-lookup"><span data-stu-id="e5567-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="e5567-p101">Uma instância de recurso compatível: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) ou [contactFolder](../resources/contactfolder.md). Observe que o grupo [postar](../resources/post.md) não é compatível.</span><span class="sxs-lookup"><span data-stu-id="e5567-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="e5567-113">Crie uma **multiValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível.</span><span class="sxs-lookup"><span data-stu-id="e5567-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="e5567-114">Get</span><span class="sxs-lookup"><span data-stu-id="e5567-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="e5567-115">Uma instância de recurso compatível ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) ou o grupo [post](../resources/post.md)) expandida com um objeto [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="e5567-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="e5567-116">Obtenha uma instância de recurso com uma propriedade estendida usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="e5567-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5567-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5567-117">Properties</span></span>
| <span data-ttu-id="e5567-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5567-118">Property</span></span>     | <span data-ttu-id="e5567-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5567-119">Type</span></span>   |<span data-ttu-id="e5567-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5567-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5567-121">id</span><span class="sxs-lookup"><span data-stu-id="e5567-121">id</span></span>|<span data-ttu-id="e5567-122">string</span><span class="sxs-lookup"><span data-stu-id="e5567-122">string</span></span>|<span data-ttu-id="e5567-p102">O identificador da propriedade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e5567-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="e5567-125">valor</span><span class="sxs-lookup"><span data-stu-id="e5567-125">value</span></span>|<span data-ttu-id="e5567-126">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5567-126">string collection</span></span>|<span data-ttu-id="e5567-127">Uma coleção de valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="e5567-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5567-128">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="e5567-128">Relationships</span></span>
<span data-ttu-id="e5567-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5567-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e5567-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5567-130">JSON representation</span></span>

<span data-ttu-id="e5567-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5567-131">Here is a JSON representation of the resource.</span></span>

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