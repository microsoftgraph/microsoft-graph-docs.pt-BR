---
title: Tipo de recurso itemAttachment
description: Um contato, evento ou mensagem que está anexado a outro evento,
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 31fd3e74e7fc35589abc57a891678e9a129c2a2e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010081"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="c89ed-103">Tipo de recurso itemAttachment</span><span class="sxs-lookup"><span data-stu-id="c89ed-103">itemAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c89ed-104">Um contato, evento ou mensagem que está anexado a outro [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="c89ed-104">A contact, event, or message that's attached to another [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="c89ed-105">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="c89ed-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c89ed-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c89ed-106">Methods</span></span>

| <span data-ttu-id="c89ed-107">Método</span><span class="sxs-lookup"><span data-stu-id="c89ed-107">Method</span></span>       | <span data-ttu-id="c89ed-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c89ed-108">Return Type</span></span>  |<span data-ttu-id="c89ed-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c89ed-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c89ed-110">Get</span><span class="sxs-lookup"><span data-stu-id="c89ed-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="c89ed-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="c89ed-111">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="c89ed-112">Leia as propriedades e os relacionamentos do objeto itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="c89ed-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="c89ed-113">Delete</span><span class="sxs-lookup"><span data-stu-id="c89ed-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="c89ed-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c89ed-114">None</span></span> |<span data-ttu-id="c89ed-115">Exclua o objeto itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="c89ed-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c89ed-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c89ed-116">Properties</span></span>
| <span data-ttu-id="c89ed-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c89ed-117">Property</span></span>     | <span data-ttu-id="c89ed-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="c89ed-118">Type</span></span>   |<span data-ttu-id="c89ed-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c89ed-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c89ed-120">contentType</span><span class="sxs-lookup"><span data-stu-id="c89ed-120">contentType</span></span>|<span data-ttu-id="c89ed-121">String</span><span class="sxs-lookup"><span data-stu-id="c89ed-121">String</span></span>|<span data-ttu-id="c89ed-122">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="c89ed-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="c89ed-123">id</span><span class="sxs-lookup"><span data-stu-id="c89ed-123">id</span></span>|<span data-ttu-id="c89ed-124">String</span><span class="sxs-lookup"><span data-stu-id="c89ed-124">String</span></span>| <span data-ttu-id="c89ed-125">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="c89ed-125">The attachment ID.</span></span>|
|<span data-ttu-id="c89ed-126">isInline</span><span class="sxs-lookup"><span data-stu-id="c89ed-126">isInline</span></span>|<span data-ttu-id="c89ed-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="c89ed-127">Boolean</span></span>|<span data-ttu-id="c89ed-128">Defina como verdadeiro se o anexo estiver embutido, como uma imagem incorporada no corpo do item.</span><span class="sxs-lookup"><span data-stu-id="c89ed-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="c89ed-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c89ed-129">lastModifiedDateTime</span></span>|<span data-ttu-id="c89ed-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c89ed-130">DateTimeOffset</span></span>|<span data-ttu-id="c89ed-131">Última data e hora em que o anexo foi alterado.</span><span class="sxs-lookup"><span data-stu-id="c89ed-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="c89ed-132">name</span><span class="sxs-lookup"><span data-stu-id="c89ed-132">name</span></span>|<span data-ttu-id="c89ed-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c89ed-133">String</span></span>|<span data-ttu-id="c89ed-134">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="c89ed-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="c89ed-135">size</span><span class="sxs-lookup"><span data-stu-id="c89ed-135">size</span></span>|<span data-ttu-id="c89ed-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c89ed-136">Int32</span></span>|<span data-ttu-id="c89ed-137">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="c89ed-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c89ed-138">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="c89ed-138">Relationships</span></span>
| <span data-ttu-id="c89ed-139">Relação</span><span class="sxs-lookup"><span data-stu-id="c89ed-139">Relationship</span></span> | <span data-ttu-id="c89ed-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="c89ed-140">Type</span></span>   |<span data-ttu-id="c89ed-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="c89ed-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c89ed-142">item</span><span class="sxs-lookup"><span data-stu-id="c89ed-142">item</span></span>|[<span data-ttu-id="c89ed-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="c89ed-143">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="c89ed-144">O contato anexado, a mensagem ou o evento.</span><span class="sxs-lookup"><span data-stu-id="c89ed-144">The attached contact, message or event.</span></span> <span data-ttu-id="c89ed-145">Propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="c89ed-145">Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c89ed-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c89ed-146">JSON representation</span></span>

<span data-ttu-id="c89ed-147">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c89ed-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
