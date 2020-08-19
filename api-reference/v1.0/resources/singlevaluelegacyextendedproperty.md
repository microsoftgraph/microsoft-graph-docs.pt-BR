---
title: Tipo de recurso singleValueLegacyExtendedProperty
description: 'Uma propriedade estendida que contém um único valor. '
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b13fa96cbfbb0e0eb6fefc97ef76e2278ca26640
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811235"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="daf5c-103">Tipo de recurso singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="daf5c-103">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="daf5c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daf5c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="daf5c-105">Uma propriedade estendida que contém um único valor.</span><span class="sxs-lookup"><span data-stu-id="daf5c-105">An extended property that contains a single value.</span></span>

<span data-ttu-id="daf5c-106">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="daf5c-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>


## <a name="methods"></a><span data-ttu-id="daf5c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="daf5c-107">Methods</span></span>

| <span data-ttu-id="daf5c-108">Método</span><span class="sxs-lookup"><span data-stu-id="daf5c-108">Method</span></span>           | <span data-ttu-id="daf5c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="daf5c-109">Return Type</span></span>    |<span data-ttu-id="daf5c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="daf5c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="daf5c-111">Post</span><span class="sxs-lookup"><span data-stu-id="daf5c-111">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="daf5c-112">Uma instância de recurso compatível: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) ou [contactFolder](../resources/contactfolder.md), mas não o grupo [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="daf5c-112">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="daf5c-113">Crie uma **singleValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível.</span><span class="sxs-lookup"><span data-stu-id="daf5c-113">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="daf5c-114">Get</span><span class="sxs-lookup"><span data-stu-id="daf5c-114">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="daf5c-115">Uma ou mais instâncias de recurso compatíveis ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) ou o grupo [post](../resources/post.md)) ou uma instância expandida com um objeto [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="daf5c-115">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="daf5c-116">Obtenha uma instância de recurso com uma propriedade estendida usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="daf5c-116">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="daf5c-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="daf5c-117">Properties</span></span>
| <span data-ttu-id="daf5c-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="daf5c-118">Property</span></span>     | <span data-ttu-id="daf5c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="daf5c-119">Type</span></span>   |<span data-ttu-id="daf5c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="daf5c-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="daf5c-121">id</span><span class="sxs-lookup"><span data-stu-id="daf5c-121">id</span></span>|<span data-ttu-id="daf5c-122">string</span><span class="sxs-lookup"><span data-stu-id="daf5c-122">string</span></span>|<span data-ttu-id="daf5c-p101">A ID da propriedade usada para identificar a propriedade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="daf5c-p101">The property ID used to identify the property. Read-only.</span></span>|
|<span data-ttu-id="daf5c-125">value</span><span class="sxs-lookup"><span data-stu-id="daf5c-125">value</span></span>|<span data-ttu-id="daf5c-126">string</span><span class="sxs-lookup"><span data-stu-id="daf5c-126">string</span></span>|<span data-ttu-id="daf5c-127">Um valor de propriedade.</span><span class="sxs-lookup"><span data-stu-id="daf5c-127">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="daf5c-128">Relações</span><span class="sxs-lookup"><span data-stu-id="daf5c-128">Relationships</span></span>
<span data-ttu-id="daf5c-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="daf5c-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="daf5c-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="daf5c-130">JSON representation</span></span>

<span data-ttu-id="daf5c-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="daf5c-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
