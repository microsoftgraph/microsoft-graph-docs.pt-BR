---
title: Tipo de recurso multiValueLegacyExtendedProperty
description: Uma propriedade estendida que contém uma coleção de valores.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: 2b0bfa2d8d5da5c3cca9479195a6649e25c8d7e8
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810518"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="38bdd-103">Tipo de recurso multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="38bdd-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="38bdd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38bdd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38bdd-105">Uma propriedade estendida que contém uma coleção de valores.</span><span class="sxs-lookup"><span data-stu-id="38bdd-105">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="38bdd-106">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="38bdd-106">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="38bdd-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="38bdd-107">Methods</span></span>

| <span data-ttu-id="38bdd-108">Método</span><span class="sxs-lookup"><span data-stu-id="38bdd-108">Method</span></span>           | <span data-ttu-id="38bdd-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="38bdd-109">Return Type</span></span>    |<span data-ttu-id="38bdd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="38bdd-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="38bdd-111">Post</span><span class="sxs-lookup"><span data-stu-id="38bdd-111">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="38bdd-112">Uma instância de recurso compatível [: Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [evento](../resources/event.md), [calendário](../resources/calendar.md), [contato](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [tarefa do Outlook](../resources/outlooktask.md)ou pasta de tarefas do [Outlook](../resources/outlooktaskfolder.md).</span><span class="sxs-lookup"><span data-stu-id="38bdd-112">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="38bdd-113">Observe que o grupo [postar](../resources/post.md) não é compatível.</span><span class="sxs-lookup"><span data-stu-id="38bdd-113">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="38bdd-114">Crie uma **multiValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível.</span><span class="sxs-lookup"><span data-stu-id="38bdd-114">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="38bdd-115">Get</span><span class="sxs-lookup"><span data-stu-id="38bdd-115">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="38bdd-116">Uma instância de recurso com suporte ([Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [Event](../resources/event.md), [Calendar](../resources/calendar.md), [Contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [tarefa do Outlook](../resources/outlooktask.md), pasta de tarefas do [Outlook](../resources/outlooktaskfolder.md)ou [postagem](../resources/post.md)de grupo) Expandida com um objeto [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="38bdd-116">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="38bdd-117">Obtenha uma instância de recurso com uma propriedade estendida usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="38bdd-117">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="38bdd-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38bdd-118">Properties</span></span>
| <span data-ttu-id="38bdd-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38bdd-119">Property</span></span>     | <span data-ttu-id="38bdd-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="38bdd-120">Type</span></span>   |<span data-ttu-id="38bdd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="38bdd-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38bdd-122">id</span><span class="sxs-lookup"><span data-stu-id="38bdd-122">id</span></span>|<span data-ttu-id="38bdd-123">string</span><span class="sxs-lookup"><span data-stu-id="38bdd-123">string</span></span>|<span data-ttu-id="38bdd-p102">O identificador da propriedade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38bdd-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="38bdd-126">valor</span><span class="sxs-lookup"><span data-stu-id="38bdd-126">value</span></span>|<span data-ttu-id="38bdd-127">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="38bdd-127">string collection</span></span>|<span data-ttu-id="38bdd-128">Uma coleção de valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="38bdd-128">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38bdd-129">Relações</span><span class="sxs-lookup"><span data-stu-id="38bdd-129">Relationships</span></span>
<span data-ttu-id="38bdd-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38bdd-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="38bdd-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38bdd-131">JSON representation</span></span>

<span data-ttu-id="38bdd-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38bdd-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
