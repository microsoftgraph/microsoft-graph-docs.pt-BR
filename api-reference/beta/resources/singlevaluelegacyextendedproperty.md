---
title: Tipo de recurso singleValueLegacyExtendedProperty
description: 'Uma propriedade estendida que contém um único valor. '
localization_priority: Normal
ms.openlocfilehash: 0d889756204853a525269f28cfdd3cc1b40be8a4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523725"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="79e5b-103">Tipo de recurso singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="79e5b-103">singleValueLegacyExtendedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79e5b-104">Uma propriedade estendida que contém um único valor.</span><span class="sxs-lookup"><span data-stu-id="79e5b-104">An extended property that contains a single value.</span></span> 

<span data-ttu-id="79e5b-105">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="79e5b-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="79e5b-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="79e5b-106">Methods</span></span>

| <span data-ttu-id="79e5b-107">Método</span><span class="sxs-lookup"><span data-stu-id="79e5b-107">Method</span></span>           | <span data-ttu-id="79e5b-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="79e5b-108">Return Type</span></span>    |<span data-ttu-id="79e5b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="79e5b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="79e5b-110">Post</span><span class="sxs-lookup"><span data-stu-id="79e5b-110">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="79e5b-111">Uma instância de recurso compatível: [Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [evento](../resources/event.md), [calendário](../resources/calendar.md), [contato](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [tarefa do Outlook](../resources/outlooktask.md)ou pasta de tarefas do [Outlook](../resources/outlooktaskfolder.md), mas não a [postagem](../resources/post.md)de grupo.</span><span class="sxs-lookup"><span data-stu-id="79e5b-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="79e5b-112">Crie uma **singleValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível.</span><span class="sxs-lookup"><span data-stu-id="79e5b-112">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="79e5b-113">Get</span><span class="sxs-lookup"><span data-stu-id="79e5b-113">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="79e5b-114">Uma ou uma coleção de instância de recurso com suporte ([Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [Event](../resources/event.md), [Calendar](../resources/calendar.md), [Contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Task](../resources/outlooktask.md)do Outlook, pasta de [tarefas do Outlook](../resources/outlooktaskfolder.md)ou [postagem](../resources/post.md)de grupo), ou uma instância expandida com um objeto [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="79e5b-114">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="79e5b-115">Obtenha uma instância de recurso com uma propriedade estendida usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="79e5b-115">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="79e5b-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79e5b-116">Properties</span></span>
| <span data-ttu-id="79e5b-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79e5b-117">Property</span></span>     | <span data-ttu-id="79e5b-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="79e5b-118">Type</span></span>   |<span data-ttu-id="79e5b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="79e5b-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79e5b-120">id</span><span class="sxs-lookup"><span data-stu-id="79e5b-120">id</span></span>|<span data-ttu-id="79e5b-121">string</span><span class="sxs-lookup"><span data-stu-id="79e5b-121">string</span></span>|<span data-ttu-id="79e5b-p101">O identificador da propriedade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="79e5b-p101">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="79e5b-124">valor</span><span class="sxs-lookup"><span data-stu-id="79e5b-124">value</span></span>|<span data-ttu-id="79e5b-125">string</span><span class="sxs-lookup"><span data-stu-id="79e5b-125">string</span></span>|<span data-ttu-id="79e5b-126">Um valor de propriedade.</span><span class="sxs-lookup"><span data-stu-id="79e5b-126">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79e5b-127">Relações</span><span class="sxs-lookup"><span data-stu-id="79e5b-127">Relationships</span></span>
<span data-ttu-id="79e5b-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79e5b-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="79e5b-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79e5b-129">JSON representation</span></span>

<span data-ttu-id="79e5b-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79e5b-130">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/singlevaluelegacyextendedproperty.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
