---
title: Tipo de recurso itemAttachment
description: Um contato, evento ou mensagem que está anexado a outro evento,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 166cd8eb5d6add0d96705ae59f38819c64b1465b
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036295"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="0f3ec-103">Tipo de recurso itemAttachment</span><span class="sxs-lookup"><span data-stu-id="0f3ec-103">itemAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f3ec-104">Um contato, evento ou mensagem anexado a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="0f3ec-104">A contact, event, or message that's attached to a user [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="0f3ec-105">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="0f3ec-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0f3ec-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="0f3ec-106">Methods</span></span>

| <span data-ttu-id="0f3ec-107">Método</span><span class="sxs-lookup"><span data-stu-id="0f3ec-107">Method</span></span>       | <span data-ttu-id="0f3ec-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0f3ec-108">Return Type</span></span>  |<span data-ttu-id="0f3ec-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f3ec-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0f3ec-110">Get</span><span class="sxs-lookup"><span data-stu-id="0f3ec-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="0f3ec-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="0f3ec-111">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="0f3ec-112">Leia as propriedades, relações ou conteúdo bruto de um objeto de item de anexo.</span><span class="sxs-lookup"><span data-stu-id="0f3ec-112">Read the properties, relationships, or raw contents of an itemAttachment object.</span></span>|
|[<span data-ttu-id="0f3ec-113">Delete</span><span class="sxs-lookup"><span data-stu-id="0f3ec-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="0f3ec-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0f3ec-114">None</span></span> |<span data-ttu-id="0f3ec-115">Exclua o objeto itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="0f3ec-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0f3ec-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f3ec-116">Properties</span></span>
| <span data-ttu-id="0f3ec-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f3ec-117">Property</span></span>     | <span data-ttu-id="0f3ec-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f3ec-118">Type</span></span>   |<span data-ttu-id="0f3ec-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f3ec-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f3ec-120">contentType</span><span class="sxs-lookup"><span data-stu-id="0f3ec-120">contentType</span></span>|<span data-ttu-id="0f3ec-121">String</span><span class="sxs-lookup"><span data-stu-id="0f3ec-121">String</span></span>|<span data-ttu-id="0f3ec-122">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="0f3ec-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="0f3ec-123">id</span><span class="sxs-lookup"><span data-stu-id="0f3ec-123">id</span></span>|<span data-ttu-id="0f3ec-124">String</span><span class="sxs-lookup"><span data-stu-id="0f3ec-124">String</span></span>| <span data-ttu-id="0f3ec-125">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="0f3ec-125">The attachment ID.</span></span>|
|<span data-ttu-id="0f3ec-126">isInline</span><span class="sxs-lookup"><span data-stu-id="0f3ec-126">isInline</span></span>|<span data-ttu-id="0f3ec-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f3ec-127">Boolean</span></span>|<span data-ttu-id="0f3ec-128">Defina como verdadeiro se o anexo estiver embutido, como uma imagem incorporada no corpo do item.</span><span class="sxs-lookup"><span data-stu-id="0f3ec-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="0f3ec-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f3ec-129">lastModifiedDateTime</span></span>|<span data-ttu-id="0f3ec-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f3ec-130">DateTimeOffset</span></span>|<span data-ttu-id="0f3ec-131">Última data e hora em que o anexo foi alterado.</span><span class="sxs-lookup"><span data-stu-id="0f3ec-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="0f3ec-132">name</span><span class="sxs-lookup"><span data-stu-id="0f3ec-132">name</span></span>|<span data-ttu-id="0f3ec-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f3ec-133">String</span></span>|<span data-ttu-id="0f3ec-134">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="0f3ec-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="0f3ec-135">size</span><span class="sxs-lookup"><span data-stu-id="0f3ec-135">size</span></span>|<span data-ttu-id="0f3ec-136">Int32</span><span class="sxs-lookup"><span data-stu-id="0f3ec-136">Int32</span></span>|<span data-ttu-id="0f3ec-137">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="0f3ec-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f3ec-138">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="0f3ec-138">Relationships</span></span>
| <span data-ttu-id="0f3ec-139">Relação</span><span class="sxs-lookup"><span data-stu-id="0f3ec-139">Relationship</span></span> | <span data-ttu-id="0f3ec-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f3ec-140">Type</span></span>   |<span data-ttu-id="0f3ec-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f3ec-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f3ec-142">item</span><span class="sxs-lookup"><span data-stu-id="0f3ec-142">item</span></span>|[<span data-ttu-id="0f3ec-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="0f3ec-143">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="0f3ec-144">O contato anexado, a mensagem ou o evento.</span><span class="sxs-lookup"><span data-stu-id="0f3ec-144">The attached contact, message or event.</span></span> <span data-ttu-id="0f3ec-145">Propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="0f3ec-145">Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f3ec-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f3ec-146">JSON representation</span></span>

<span data-ttu-id="0f3ec-147">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0f3ec-147">Here is a JSON representation of the resource</span></span>

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
