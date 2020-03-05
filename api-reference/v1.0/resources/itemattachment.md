---
title: Tipo de recurso itemAttachment
description: 'Um contato, evento ou mensagem que está anexado a outro evento, mensagem ou postagem.  '
localization_priority: Priority
ms.prod: outlook
author: angelgolfer-ms
doc_type: resourcePageType
ms.openlocfilehash: c5c565e81ed9218d3d04f15585236b87a362d5e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447637"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="6bac8-103">Tipo de recurso itemAttachment</span><span class="sxs-lookup"><span data-stu-id="6bac8-103">itemAttachment resource type</span></span>

<span data-ttu-id="6bac8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bac8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6bac8-105">Um contato, evento ou mensagem anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md) ou [postagem](../resources/post.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="6bac8-105">A contact, event, or message that's attached to a user [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="6bac8-106">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="6bac8-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6bac8-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6bac8-107">Methods</span></span>

| <span data-ttu-id="6bac8-108">Método</span><span class="sxs-lookup"><span data-stu-id="6bac8-108">Method</span></span>       | <span data-ttu-id="6bac8-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6bac8-109">Return Type</span></span>  |<span data-ttu-id="6bac8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bac8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6bac8-111">Get</span><span class="sxs-lookup"><span data-stu-id="6bac8-111">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="6bac8-112">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="6bac8-112">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="6bac8-113">Leia as propriedades, os relacionamentos ou o conteúdo bruto de um objeto itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="6bac8-113">Read the properties, relationships, or raw contents of an itemAttachment object.</span></span>|
|[<span data-ttu-id="6bac8-114">Delete</span><span class="sxs-lookup"><span data-stu-id="6bac8-114">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="6bac8-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6bac8-115">None</span></span> |<span data-ttu-id="6bac8-116">Exclua o objeto itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="6bac8-116">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6bac8-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6bac8-117">Properties</span></span>
| <span data-ttu-id="6bac8-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6bac8-118">Property</span></span>     | <span data-ttu-id="6bac8-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bac8-119">Type</span></span>   |<span data-ttu-id="6bac8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bac8-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6bac8-121">contentType</span><span class="sxs-lookup"><span data-stu-id="6bac8-121">contentType</span></span>|<span data-ttu-id="6bac8-122">String</span><span class="sxs-lookup"><span data-stu-id="6bac8-122">String</span></span>|<span data-ttu-id="6bac8-123">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="6bac8-123">The content type of the attachment.</span></span>|
|<span data-ttu-id="6bac8-124">id</span><span class="sxs-lookup"><span data-stu-id="6bac8-124">id</span></span>|<span data-ttu-id="6bac8-125">String</span><span class="sxs-lookup"><span data-stu-id="6bac8-125">String</span></span>| <span data-ttu-id="6bac8-126">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="6bac8-126">The attachment ID.</span></span>|
|<span data-ttu-id="6bac8-127">isInline</span><span class="sxs-lookup"><span data-stu-id="6bac8-127">isInline</span></span>|<span data-ttu-id="6bac8-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="6bac8-128">Boolean</span></span>|<span data-ttu-id="6bac8-129">Defina como verdadeiro se o anexo estiver embutido, como uma imagem incorporada no corpo do item.</span><span class="sxs-lookup"><span data-stu-id="6bac8-129">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="6bac8-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6bac8-130">lastModifiedDateTime</span></span>|<span data-ttu-id="6bac8-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bac8-131">DateTimeOffset</span></span>|<span data-ttu-id="6bac8-132">Última data e hora em que o anexo foi alterado.</span><span class="sxs-lookup"><span data-stu-id="6bac8-132">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="6bac8-133">name</span><span class="sxs-lookup"><span data-stu-id="6bac8-133">name</span></span>|<span data-ttu-id="6bac8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6bac8-134">String</span></span>|<span data-ttu-id="6bac8-135">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="6bac8-135">The display name of the attachment.</span></span>|
|<span data-ttu-id="6bac8-136">size</span><span class="sxs-lookup"><span data-stu-id="6bac8-136">size</span></span>|<span data-ttu-id="6bac8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6bac8-137">Int32</span></span>|<span data-ttu-id="6bac8-138">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="6bac8-138">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bac8-139">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="6bac8-139">Relationships</span></span>
| <span data-ttu-id="6bac8-140">Relação</span><span class="sxs-lookup"><span data-stu-id="6bac8-140">Relationship</span></span> | <span data-ttu-id="6bac8-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bac8-141">Type</span></span>   |<span data-ttu-id="6bac8-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bac8-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6bac8-143">item</span><span class="sxs-lookup"><span data-stu-id="6bac8-143">item</span></span>|[<span data-ttu-id="6bac8-144">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="6bac8-144">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="6bac8-p101">A mensagem ou evento anexado. Propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="6bac8-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6bac8-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6bac8-147">JSON representation</span></span>

<span data-ttu-id="6bac8-148">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6bac8-148">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.itemAttachment",
  "@odata.annotations": [
    {
      "property": "item",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024,
  "item": { "@odata.type": "microsoft.graph.outlookItem" }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
