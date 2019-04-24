---
title: Tipo de recurso multiValueLegacyExtendedProperty
description: Uma propriedade estendida que contém uma coleção de valores.
localization_priority: Normal
ms.openlocfilehash: 86ba1969e06dc549d1fca00148cbea96f94cf4b6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506254"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="43148-103">Tipo de recurso multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="43148-103">multiValueLegacyExtendedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43148-104">Uma propriedade estendida que contém uma coleção de valores.</span><span class="sxs-lookup"><span data-stu-id="43148-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="43148-105">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="43148-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="43148-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="43148-106">Methods</span></span>

| <span data-ttu-id="43148-107">Método</span><span class="sxs-lookup"><span data-stu-id="43148-107">Method</span></span>           | <span data-ttu-id="43148-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="43148-108">Return Type</span></span>    |<span data-ttu-id="43148-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="43148-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="43148-110">Post</span><span class="sxs-lookup"><span data-stu-id="43148-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="43148-111">Uma instância de recurso compatível [: Message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [evento](../resources/event.md), [calendário](../resources/calendar.md), [contato](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [tarefa do Outlook](../resources/outlooktask.md)ou pasta de tarefas do [Outlook](../resources/outlooktaskfolder.md).</span><span class="sxs-lookup"><span data-stu-id="43148-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="43148-112">Observe que o grupo [postar](../resources/post.md) não é compatível.</span><span class="sxs-lookup"><span data-stu-id="43148-112">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="43148-113">Crie uma **multiValueLegacyExtendedProperty** em uma instância nova ou existente de um recurso compatível.</span><span class="sxs-lookup"><span data-stu-id="43148-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="43148-114">Get</span><span class="sxs-lookup"><span data-stu-id="43148-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="43148-115">Uma instância de recurso compatível ([mensagem](../resources/message.md), [mailFolder](../resources/mailfolder.md), [evento](../resources/event.md), [calendário](../resources/calendar.md), [contato](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [tarefa do Outlook](../resources/outlooktask.md), pasta de tarefas do [Outlook](../resources/outlooktaskfolder.md)ou [postagem](../resources/post.md)de grupo) Expandida com um [ objeto multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="43148-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="43148-116">Obtenha uma instância de recurso com uma propriedade estendida usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="43148-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="43148-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43148-117">Properties</span></span>
| <span data-ttu-id="43148-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43148-118">Property</span></span>     | <span data-ttu-id="43148-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="43148-119">Type</span></span>   |<span data-ttu-id="43148-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="43148-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43148-121">id</span><span class="sxs-lookup"><span data-stu-id="43148-121">id</span></span>|<span data-ttu-id="43148-122">string</span><span class="sxs-lookup"><span data-stu-id="43148-122">string</span></span>|<span data-ttu-id="43148-p102">O identificador da propriedade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="43148-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="43148-125">valor</span><span class="sxs-lookup"><span data-stu-id="43148-125">value</span></span>|<span data-ttu-id="43148-126">coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="43148-126">string collection</span></span>|<span data-ttu-id="43148-127">Uma coleção de valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="43148-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43148-128">Relações</span><span class="sxs-lookup"><span data-stu-id="43148-128">Relationships</span></span>
<span data-ttu-id="43148-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="43148-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="43148-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43148-130">JSON representation</span></span>

<span data-ttu-id="43148-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43148-131">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/multivaluelegacyextendedproperty.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
