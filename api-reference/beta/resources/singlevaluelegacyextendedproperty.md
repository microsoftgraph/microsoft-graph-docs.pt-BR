---
title: Tipo de recurso singleValueLegacyExtendedProperty
description: 'Uma propriedade estendida que contém um único valor. '
ms.openlocfilehash: 1b9eeaa05ee15aab30c1761cd35f70f586dffb24
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039987"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="d62ff-103">Tipo de recurso singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="d62ff-103">singleValueLegacyExtendedProperty resource type</span></span>

> <span data-ttu-id="d62ff-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d62ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d62ff-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d62ff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d62ff-106">Uma propriedade estendida que contém um único valor.</span><span class="sxs-lookup"><span data-stu-id="d62ff-106">An extended property that contains a single value.</span></span> 

<span data-ttu-id="d62ff-107">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="d62ff-107">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="d62ff-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d62ff-108">Methods</span></span>

| <span data-ttu-id="d62ff-109">Método</span><span class="sxs-lookup"><span data-stu-id="d62ff-109">Method</span></span>           | <span data-ttu-id="d62ff-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d62ff-110">Return Type</span></span>    |<span data-ttu-id="d62ff-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d62ff-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d62ff-112">Post</span><span class="sxs-lookup"><span data-stu-id="d62ff-112">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="d62ff-113">Uma instância de recursos com suporte: [mensagem](../resources/message.md), [mailFolder](../resources/mailfolder.md), [evento](../resources/event.md), [calendário](../resources/calendar.md), [Contatos](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [tarefa do Outlook](../resources/outlooktask.md), ou [pasta de tarefas do Outlook](../resources/outlooktaskfolder.md), mas não o grupo [postar](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="d62ff-113">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="d62ff-114">Crie uma **singleValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível.</span><span class="sxs-lookup"><span data-stu-id="d62ff-114">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="d62ff-115">Get</span><span class="sxs-lookup"><span data-stu-id="d62ff-115">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="d62ff-116">Uma ou uma coleção de instância de recursos com suporte ([mensagem](../resources/message.md), [mailFolder](../resources/mailfolder.md), [evento](../resources/event.md), [calendário](../resources/calendar.md), [Contatos](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [tarefa do Outlook](../resources/outlooktask.md), [pasta de tarefas do Outlook](../resources/outlooktaskfolder.md)ou grupo [postar](../resources/post.md)), ou uma instância deste tipo expandida com um objeto [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="d62ff-116">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="d62ff-117">Obtenha uma instância de recurso com uma propriedade estendida usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="d62ff-117">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="d62ff-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d62ff-118">Properties</span></span>
| <span data-ttu-id="d62ff-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d62ff-119">Property</span></span>     | <span data-ttu-id="d62ff-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d62ff-120">Type</span></span>   |<span data-ttu-id="d62ff-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d62ff-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d62ff-122">id</span><span class="sxs-lookup"><span data-stu-id="d62ff-122">id</span></span>|<span data-ttu-id="d62ff-123">string</span><span class="sxs-lookup"><span data-stu-id="d62ff-123">string</span></span>|<span data-ttu-id="d62ff-p102">O identificador da propriedade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d62ff-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="d62ff-126">valor</span><span class="sxs-lookup"><span data-stu-id="d62ff-126">value</span></span>|<span data-ttu-id="d62ff-127">string</span><span class="sxs-lookup"><span data-stu-id="d62ff-127">string</span></span>|<span data-ttu-id="d62ff-128">Um valor de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d62ff-128">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d62ff-129">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="d62ff-129">Relationships</span></span>
<span data-ttu-id="d62ff-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d62ff-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d62ff-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d62ff-131">JSON representation</span></span>

<span data-ttu-id="d62ff-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d62ff-132">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->