---
title: Tipo de recurso singleValueLegacyExtendedProperty
description: 'Uma propriedade estendida que contém um único valor. '
ms.openlocfilehash: 82a2ca848ba22381366016617c3fa6529ce4ee54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004465"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="e8e6e-103">Tipo de recurso singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="e8e6e-103">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="e8e6e-104">Uma propriedade estendida que contém um único valor.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-104">An extended property that contains a single value.</span></span> 

<span data-ttu-id="e8e6e-105">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="e8e6e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e8e6e-106">Methods</span></span>

| <span data-ttu-id="e8e6e-107">Método</span><span class="sxs-lookup"><span data-stu-id="e8e6e-107">Method</span></span>           | <span data-ttu-id="e8e6e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e8e6e-108">Return Type</span></span>    |<span data-ttu-id="e8e6e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8e6e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e8e6e-110">Post</span><span class="sxs-lookup"><span data-stu-id="e8e6e-110">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="e8e6e-111">Uma instância de recurso compatível: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md) ou [contactFolder](../resources/contactfolder.md), mas não o grupo [post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="e8e6e-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="e8e6e-112">Crie uma **singleValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-112">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="e8e6e-113">Get</span><span class="sxs-lookup"><span data-stu-id="e8e6e-113">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="e8e6e-114">Uma ou mais instâncias de recurso compatíveis ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md) ou o grupo [post](../resources/post.md)) ou uma instância expandida com um objeto [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md).</span><span class="sxs-lookup"><span data-stu-id="e8e6e-114">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="e8e6e-115">Obtenha uma instância de recurso com uma propriedade estendida usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-115">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="e8e6e-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8e6e-116">Properties</span></span>
| <span data-ttu-id="e8e6e-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8e6e-117">Property</span></span>     | <span data-ttu-id="e8e6e-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8e6e-118">Type</span></span>   |<span data-ttu-id="e8e6e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8e6e-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8e6e-120">id</span><span class="sxs-lookup"><span data-stu-id="e8e6e-120">id</span></span>|<span data-ttu-id="e8e6e-121">string</span><span class="sxs-lookup"><span data-stu-id="e8e6e-121">string</span></span>|<span data-ttu-id="e8e6e-p101">A ID da propriedade usada para identificar a propriedade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-p101">The property ID used to identify the property. Read-only.</span></span>|
|<span data-ttu-id="e8e6e-124">valor</span><span class="sxs-lookup"><span data-stu-id="e8e6e-124">value</span></span>|<span data-ttu-id="e8e6e-125">string</span><span class="sxs-lookup"><span data-stu-id="e8e6e-125">string</span></span>|<span data-ttu-id="e8e6e-126">Um valor de propriedade.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-126">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8e6e-127">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="e8e6e-127">Relationships</span></span>
<span data-ttu-id="e8e6e-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e8e6e-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e8e6e-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8e6e-129">JSON representation</span></span>

<span data-ttu-id="e8e6e-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8e6e-130">Here is a JSON representation of the resource.</span></span>

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