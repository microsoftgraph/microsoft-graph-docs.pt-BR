---
title: Tipo de recurso singleValueLegacyExtendedProperty
description: 'Uma propriedade estendida que contém um único valor. '
localization_priority: Normal
ms.openlocfilehash: 51a42661ea3a19ea8e82ba78115bfa5290d99d15
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857411"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="99c14-103">Tipo de recurso singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="99c14-103">singleValueLegacyExtendedProperty resource type</span></span>

> <span data-ttu-id="99c14-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="99c14-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99c14-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="99c14-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99c14-106">Uma propriedade estendida que contém um único valor.</span><span class="sxs-lookup"><span data-stu-id="99c14-106">An extended property that contains a single value.</span></span> 

<span data-ttu-id="99c14-107">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="99c14-107">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="99c14-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="99c14-108">Methods</span></span>

| <span data-ttu-id="99c14-109">Método</span><span class="sxs-lookup"><span data-stu-id="99c14-109">Method</span></span>           | <span data-ttu-id="99c14-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="99c14-110">Return Type</span></span>    |<span data-ttu-id="99c14-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="99c14-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="99c14-112">Post</span><span class="sxs-lookup"><span data-stu-id="99c14-112">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="99c14-113">Uma instância de recursos com suporte: [mensagem](../resources/message.md), [mailFolder](../resources/mailfolder.md), [evento](../resources/event.md), [calendário](../resources/calendar.md), [Contatos](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [tarefa do Outlook](../resources/outlooktask.md), ou [pasta de tarefas do Outlook](../resources/outlooktaskfolder.md), mas não o grupo [postar](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="99c14-113">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="99c14-114">Crie uma **singleValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível.</span><span class="sxs-lookup"><span data-stu-id="99c14-114">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="99c14-115">Get</span><span class="sxs-lookup"><span data-stu-id="99c14-115">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="99c14-116">Uma ou uma coleção de instância de recursos com suporte ([mensagem](../resources/message.md), [mailFolder](../resources/mailfolder.md), [evento](../resources/event.md), [calendário](../resources/calendar.md), [Contatos](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [tarefa do Outlook](../resources/outlooktask.md), [pasta de tarefas do Outlook](../resources/outlooktaskfolder.md)ou grupo [postar](../resources/post.md)), ou uma instância deste tipo expandida com um objeto [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="99c14-116">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="99c14-117">Obtenha uma instância de recurso com uma propriedade estendida usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="99c14-117">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="99c14-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99c14-118">Properties</span></span>
| <span data-ttu-id="99c14-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99c14-119">Property</span></span>     | <span data-ttu-id="99c14-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="99c14-120">Type</span></span>   |<span data-ttu-id="99c14-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="99c14-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99c14-122">id</span><span class="sxs-lookup"><span data-stu-id="99c14-122">id</span></span>|<span data-ttu-id="99c14-123">string</span><span class="sxs-lookup"><span data-stu-id="99c14-123">string</span></span>|<span data-ttu-id="99c14-p102">O identificador da propriedade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="99c14-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="99c14-126">valor</span><span class="sxs-lookup"><span data-stu-id="99c14-126">value</span></span>|<span data-ttu-id="99c14-127">string</span><span class="sxs-lookup"><span data-stu-id="99c14-127">string</span></span>|<span data-ttu-id="99c14-128">Um valor de propriedade.</span><span class="sxs-lookup"><span data-stu-id="99c14-128">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99c14-129">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="99c14-129">Relationships</span></span>
<span data-ttu-id="99c14-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99c14-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="99c14-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99c14-131">JSON representation</span></span>

<span data-ttu-id="99c14-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99c14-132">Here is a JSON representation of the resource.</span></span>

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
