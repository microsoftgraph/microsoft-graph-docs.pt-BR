---
title: Tipo de recurso singleValueLegacyExtendedProperty
description: 'Uma propriedade estendida que contém um único valor. '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 030893ab3a5eaefad4637cfd50321f1653b41070
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334427"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="e8226-103">Tipo de recurso singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="e8226-103">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="e8226-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8226-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e8226-105">Uma propriedade estendida que contém um único valor.</span><span class="sxs-lookup"><span data-stu-id="e8226-105">An extended property that contains a single value.</span></span>

<span data-ttu-id="e8226-106">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="e8226-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>


## <a name="methods"></a><span data-ttu-id="e8226-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e8226-107">Methods</span></span>

| <span data-ttu-id="e8226-108">Método</span><span class="sxs-lookup"><span data-stu-id="e8226-108">Method</span></span>           | <span data-ttu-id="e8226-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e8226-109">Return Type</span></span>    |<span data-ttu-id="e8226-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8226-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e8226-111">Post</span><span class="sxs-lookup"><span data-stu-id="e8226-111">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="e8226-112">Uma instância de recurso compatível: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) ou [contactFolder](../resources/contactfolder.md), mas não o grupo [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="e8226-112">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="e8226-113">Crie uma **singleValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível.</span><span class="sxs-lookup"><span data-stu-id="e8226-113">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="e8226-114">Get</span><span class="sxs-lookup"><span data-stu-id="e8226-114">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="e8226-115">Uma ou mais instâncias de recurso compatíveis ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) ou o grupo [post](../resources/post.md)) ou uma instância expandida com um objeto [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="e8226-115">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="e8226-116">Obtenha uma instância de recurso com uma propriedade estendida usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="e8226-116">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="e8226-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8226-117">Properties</span></span>
| <span data-ttu-id="e8226-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8226-118">Property</span></span>     | <span data-ttu-id="e8226-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8226-119">Type</span></span>   |<span data-ttu-id="e8226-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8226-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8226-121">id</span><span class="sxs-lookup"><span data-stu-id="e8226-121">id</span></span>|<span data-ttu-id="e8226-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8226-122">string</span></span>|<span data-ttu-id="e8226-p101">A ID da propriedade usada para identificar a propriedade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e8226-p101">The property ID used to identify the property. Read-only.</span></span>|
|<span data-ttu-id="e8226-125">value</span><span class="sxs-lookup"><span data-stu-id="e8226-125">value</span></span>|<span data-ttu-id="e8226-126">string</span><span class="sxs-lookup"><span data-stu-id="e8226-126">string</span></span>|<span data-ttu-id="e8226-127">Um valor de propriedade.</span><span class="sxs-lookup"><span data-stu-id="e8226-127">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8226-128">Relações</span><span class="sxs-lookup"><span data-stu-id="e8226-128">Relationships</span></span>
<span data-ttu-id="e8226-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e8226-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e8226-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8226-130">JSON representation</span></span>

<span data-ttu-id="e8226-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8226-131">Here is a JSON representation of the resource.</span></span>

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

