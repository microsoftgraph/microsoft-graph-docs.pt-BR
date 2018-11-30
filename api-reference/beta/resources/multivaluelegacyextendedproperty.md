---
title: Tipo de recurso multiValueLegacyExtendedProperty
description: Uma propriedade estendida que contém uma coleção de valores.
ms.openlocfilehash: efb871594028b5c2d54b1c081f901717b754c8ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037024"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="d2f93-103">Tipo de recurso multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="d2f93-103">multiValueLegacyExtendedProperty resource type</span></span>

> <span data-ttu-id="d2f93-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d2f93-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2f93-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d2f93-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2f93-106">Uma propriedade estendida que contém uma coleção de valores.</span><span class="sxs-lookup"><span data-stu-id="d2f93-106">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="d2f93-107">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="d2f93-107">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="d2f93-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d2f93-108">Methods</span></span>

| <span data-ttu-id="d2f93-109">Método</span><span class="sxs-lookup"><span data-stu-id="d2f93-109">Method</span></span>           | <span data-ttu-id="d2f93-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d2f93-110">Return Type</span></span>    |<span data-ttu-id="d2f93-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2f93-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2f93-112">Post</span><span class="sxs-lookup"><span data-stu-id="d2f93-112">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="d2f93-113">Uma instância de recursos com suporte: [mensagem](../resources/message.md), [mailFolder](../resources/mailfolder.md), [evento](../resources/event.md), [calendário](../resources/calendar.md), [Contatos](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [tarefa do Outlook](../resources/outlooktask.md)ou [pasta de tarefas do Outlook](../resources/outlooktaskfolder.md).</span><span class="sxs-lookup"><span data-stu-id="d2f93-113">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="d2f93-114">Observe que não há suporte para esse grupo de [postagem](../resources/post.md) .</span><span class="sxs-lookup"><span data-stu-id="d2f93-114">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="d2f93-115">Crie uma **multiValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível.</span><span class="sxs-lookup"><span data-stu-id="d2f93-115">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="d2f93-116">Get</span><span class="sxs-lookup"><span data-stu-id="d2f93-116">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="d2f93-117">Uma instância de recursos com suporte ([mensagem](../resources/message.md), [mailFolder](../resources/mailfolder.md), [evento](../resources/event.md), [calendário](../resources/calendar.md), [Contatos](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [tarefa do Outlook](../resources/outlooktask.md), [pasta de tarefas do Outlook](../resources/outlooktaskfolder.md)ou grupo [postar](../resources/post.md)) expandida com um [ multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) objeto.</span><span class="sxs-lookup"><span data-stu-id="d2f93-117">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="d2f93-118">Obtenha uma instância de recurso com uma propriedade estendida usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="d2f93-118">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2f93-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2f93-119">Properties</span></span>
| <span data-ttu-id="d2f93-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2f93-120">Property</span></span>     | <span data-ttu-id="d2f93-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2f93-121">Type</span></span>   |<span data-ttu-id="d2f93-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2f93-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2f93-123">id</span><span class="sxs-lookup"><span data-stu-id="d2f93-123">id</span></span>|<span data-ttu-id="d2f93-124">string</span><span class="sxs-lookup"><span data-stu-id="d2f93-124">string</span></span>|<span data-ttu-id="d2f93-p103">O identificador da propriedade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d2f93-p103">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="d2f93-127">valor</span><span class="sxs-lookup"><span data-stu-id="d2f93-127">value</span></span>|<span data-ttu-id="d2f93-128">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d2f93-128">string collection</span></span>|<span data-ttu-id="d2f93-129">Uma coleção de valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d2f93-129">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2f93-130">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="d2f93-130">Relationships</span></span>
<span data-ttu-id="d2f93-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2f93-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d2f93-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2f93-132">JSON representation</span></span>

<span data-ttu-id="d2f93-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2f93-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.multivaluelegacyextendedproperty"
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