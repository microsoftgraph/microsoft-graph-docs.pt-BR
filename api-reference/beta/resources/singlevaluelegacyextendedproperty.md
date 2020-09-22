---
title: Tipo de recurso singleValueLegacyExtendedProperty
description: 'Uma propriedade estendida que contém um único valor. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: bb602443589faf61bbd66033e1c462d8e30f2e0b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092290"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="a465c-103">Tipo de recurso singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="a465c-103">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="a465c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a465c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="a465c-105">Uma propriedade estendida que contém um único valor.</span><span class="sxs-lookup"><span data-stu-id="a465c-105">An extended property that contains a single value.</span></span>

<span data-ttu-id="a465c-106">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="a465c-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>


## <a name="methods"></a><span data-ttu-id="a465c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a465c-107">Methods</span></span>

| <span data-ttu-id="a465c-108">Método</span><span class="sxs-lookup"><span data-stu-id="a465c-108">Method</span></span>           | <span data-ttu-id="a465c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a465c-109">Return Type</span></span>    |<span data-ttu-id="a465c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a465c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a465c-111">Post</span><span class="sxs-lookup"><span data-stu-id="a465c-111">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="a465c-112">Uma instância de recurso compatível: [Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [evento](../resources/event.md), [calendário](../resources/calendar.md), [contato](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [tarefa do Outlook](../resources/outlooktask.md)ou pasta de tarefas do [Outlook](../resources/outlooktaskfolder.md), mas não a [postagem](../resources/post.md)de grupo.</span><span class="sxs-lookup"><span data-stu-id="a465c-112">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="a465c-113">Crie uma **singleValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível.</span><span class="sxs-lookup"><span data-stu-id="a465c-113">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="a465c-114">Get</span><span class="sxs-lookup"><span data-stu-id="a465c-114">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="a465c-115">Uma ou uma coleção de instância de recurso compatível[(Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [Event](../resources/event.md), [Calendar](../resources/calendar.md), [Contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Task](../resources/outlooktask.md)do Outlook, pasta de [tarefas do Outlook](../resources/outlooktaskfolder.md)ou [postagem](../resources/post.md)de grupo) ou uma instância expandida com um objeto [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="a465c-115">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="a465c-116">Obtenha uma instância de recurso com uma propriedade estendida usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="a465c-116">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="a465c-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a465c-117">Properties</span></span>
| <span data-ttu-id="a465c-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a465c-118">Property</span></span>     | <span data-ttu-id="a465c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a465c-119">Type</span></span>   |<span data-ttu-id="a465c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a465c-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a465c-121">id</span><span class="sxs-lookup"><span data-stu-id="a465c-121">id</span></span>|<span data-ttu-id="a465c-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a465c-122">string</span></span>|<span data-ttu-id="a465c-p101">O identificador da propriedade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a465c-p101">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="a465c-125">valor</span><span class="sxs-lookup"><span data-stu-id="a465c-125">value</span></span>|<span data-ttu-id="a465c-126">string</span><span class="sxs-lookup"><span data-stu-id="a465c-126">string</span></span>|<span data-ttu-id="a465c-127">Um valor de propriedade.</span><span class="sxs-lookup"><span data-stu-id="a465c-127">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a465c-128">Relações</span><span class="sxs-lookup"><span data-stu-id="a465c-128">Relationships</span></span>
<span data-ttu-id="a465c-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a465c-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a465c-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a465c-130">JSON representation</span></span>

<span data-ttu-id="a465c-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a465c-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


