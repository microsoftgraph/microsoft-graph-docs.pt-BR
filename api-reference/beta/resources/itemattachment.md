---
title: Tipo de recurso itemAttachment
description: Um contato, evento ou mensagem que está anexado a outro evento,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 9cce3ac77838867d70d2bd847e8a9d631e7f3b5a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075620"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="95be0-103">Tipo de recurso itemAttachment</span><span class="sxs-lookup"><span data-stu-id="95be0-103">itemAttachment resource type</span></span>

<span data-ttu-id="95be0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95be0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

<span data-ttu-id="95be0-105">Um contato, evento ou mensagem anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="95be0-105">A contact, event, or message that's attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="95be0-106">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="95be0-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="95be0-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="95be0-107">Methods</span></span>

| <span data-ttu-id="95be0-108">Método</span><span class="sxs-lookup"><span data-stu-id="95be0-108">Method</span></span>       | <span data-ttu-id="95be0-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="95be0-109">Return Type</span></span>  |<span data-ttu-id="95be0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="95be0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="95be0-111">Get</span><span class="sxs-lookup"><span data-stu-id="95be0-111">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="95be0-112">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="95be0-112">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="95be0-113">Leia as propriedades, os relacionamentos ou o conteúdo bruto de um objeto itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="95be0-113">Read the properties, relationships, or raw contents of an itemAttachment object.</span></span>|
|[<span data-ttu-id="95be0-114">Delete</span><span class="sxs-lookup"><span data-stu-id="95be0-114">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="95be0-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="95be0-115">None</span></span> |<span data-ttu-id="95be0-116">Exclua o objeto itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="95be0-116">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="95be0-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95be0-117">Properties</span></span>
| <span data-ttu-id="95be0-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95be0-118">Property</span></span>     | <span data-ttu-id="95be0-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="95be0-119">Type</span></span>   |<span data-ttu-id="95be0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="95be0-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95be0-121">contentType</span><span class="sxs-lookup"><span data-stu-id="95be0-121">contentType</span></span>|<span data-ttu-id="95be0-122">String</span><span class="sxs-lookup"><span data-stu-id="95be0-122">String</span></span>|<span data-ttu-id="95be0-123">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="95be0-123">The content type of the attachment.</span></span>|
|<span data-ttu-id="95be0-124">id</span><span class="sxs-lookup"><span data-stu-id="95be0-124">id</span></span>|<span data-ttu-id="95be0-125">String</span><span class="sxs-lookup"><span data-stu-id="95be0-125">String</span></span>| <span data-ttu-id="95be0-126">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="95be0-126">The attachment ID.</span></span>|
|<span data-ttu-id="95be0-127">isInline</span><span class="sxs-lookup"><span data-stu-id="95be0-127">isInline</span></span>|<span data-ttu-id="95be0-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="95be0-128">Boolean</span></span>|<span data-ttu-id="95be0-129">Defina como verdadeiro se o anexo estiver embutido, como uma imagem incorporada no corpo do item.</span><span class="sxs-lookup"><span data-stu-id="95be0-129">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="95be0-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95be0-130">lastModifiedDateTime</span></span>|<span data-ttu-id="95be0-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95be0-131">DateTimeOffset</span></span>|<span data-ttu-id="95be0-132">Última data e hora em que o anexo foi alterado.</span><span class="sxs-lookup"><span data-stu-id="95be0-132">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="95be0-133">name</span><span class="sxs-lookup"><span data-stu-id="95be0-133">name</span></span>|<span data-ttu-id="95be0-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95be0-134">String</span></span>|<span data-ttu-id="95be0-135">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="95be0-135">The display name of the attachment.</span></span>|
|<span data-ttu-id="95be0-136">size</span><span class="sxs-lookup"><span data-stu-id="95be0-136">size</span></span>|<span data-ttu-id="95be0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="95be0-137">Int32</span></span>|<span data-ttu-id="95be0-138">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="95be0-138">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95be0-139">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="95be0-139">Relationships</span></span>
| <span data-ttu-id="95be0-140">Relação</span><span class="sxs-lookup"><span data-stu-id="95be0-140">Relationship</span></span> | <span data-ttu-id="95be0-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="95be0-141">Type</span></span>   |<span data-ttu-id="95be0-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="95be0-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95be0-143">item</span><span class="sxs-lookup"><span data-stu-id="95be0-143">item</span></span>|[<span data-ttu-id="95be0-144">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="95be0-144">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="95be0-p101">O contato anexado, a mensagem ou o evento. Propriedade Navigation.</span><span class="sxs-lookup"><span data-stu-id="95be0-p101">The attached contact, message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95be0-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95be0-147">JSON representation</span></span>

<span data-ttu-id="95be0-148">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="95be0-148">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "optionalProperties": [
    "item"
  ],
  "@odata.type": "microsoft.graph.itemAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


