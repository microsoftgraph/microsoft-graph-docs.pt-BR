---
title: Tipo de recurso itemAttachment
description: Um contato, evento ou mensagem anexado a outro evento,
localization_priority: Normal
ms.openlocfilehash: f7372db19a545bd7d6ae39121fd14be4c9f4436b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825001"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="b1f10-103">Tipo de recurso itemAttachment</span><span class="sxs-lookup"><span data-stu-id="b1f10-103">itemAttachment resource type</span></span>

> <span data-ttu-id="b1f10-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b1f10-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1f10-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b1f10-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1f10-106">Um contato, evento ou mensagem anexado a outro [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postar](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="b1f10-106">A contact, event, or message that's attached to another [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md).</span></span>  

<span data-ttu-id="b1f10-107">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="b1f10-107">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b1f10-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b1f10-108">Methods</span></span>

| <span data-ttu-id="b1f10-109">Método</span><span class="sxs-lookup"><span data-stu-id="b1f10-109">Method</span></span>       | <span data-ttu-id="b1f10-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b1f10-110">Return Type</span></span>  |<span data-ttu-id="b1f10-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1f10-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b1f10-112">Get</span><span class="sxs-lookup"><span data-stu-id="b1f10-112">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="b1f10-113">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="b1f10-113">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="b1f10-114">Leia as propriedades e os relacionamentos do objeto itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="b1f10-114">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="b1f10-115">Delete</span><span class="sxs-lookup"><span data-stu-id="b1f10-115">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="b1f10-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1f10-116">None</span></span> |<span data-ttu-id="b1f10-117">Exclua o objeto itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="b1f10-117">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b1f10-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1f10-118">Properties</span></span>
| <span data-ttu-id="b1f10-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1f10-119">Property</span></span>     | <span data-ttu-id="b1f10-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1f10-120">Type</span></span>   |<span data-ttu-id="b1f10-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1f10-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1f10-122">contentType</span><span class="sxs-lookup"><span data-stu-id="b1f10-122">contentType</span></span>|<span data-ttu-id="b1f10-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1f10-123">String</span></span>|<span data-ttu-id="b1f10-124">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="b1f10-124">The content type of the attachment.</span></span>|
|<span data-ttu-id="b1f10-125">id</span><span class="sxs-lookup"><span data-stu-id="b1f10-125">id</span></span>|<span data-ttu-id="b1f10-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1f10-126">String</span></span>| <span data-ttu-id="b1f10-127">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="b1f10-127">The attachment ID.</span></span>|
|<span data-ttu-id="b1f10-128">isInline</span><span class="sxs-lookup"><span data-stu-id="b1f10-128">isInline</span></span>|<span data-ttu-id="b1f10-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1f10-129">Boolean</span></span>|<span data-ttu-id="b1f10-130">Defina como verdadeiro se o anexo estiver embutido, como uma imagem incorporada no corpo do item.</span><span class="sxs-lookup"><span data-stu-id="b1f10-130">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="b1f10-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1f10-131">lastModifiedDateTime</span></span>|<span data-ttu-id="b1f10-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1f10-132">DateTimeOffset</span></span>|<span data-ttu-id="b1f10-133">Última data e hora em que o anexo foi alterado.</span><span class="sxs-lookup"><span data-stu-id="b1f10-133">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="b1f10-134">name</span><span class="sxs-lookup"><span data-stu-id="b1f10-134">name</span></span>|<span data-ttu-id="b1f10-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1f10-135">String</span></span>|<span data-ttu-id="b1f10-136">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="b1f10-136">The display name of the attachment.</span></span>|
|<span data-ttu-id="b1f10-137">size</span><span class="sxs-lookup"><span data-stu-id="b1f10-137">size</span></span>|<span data-ttu-id="b1f10-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b1f10-138">Int32</span></span>|<span data-ttu-id="b1f10-139">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="b1f10-139">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1f10-140">Relações</span><span class="sxs-lookup"><span data-stu-id="b1f10-140">Relationships</span></span>
| <span data-ttu-id="b1f10-141">Relação</span><span class="sxs-lookup"><span data-stu-id="b1f10-141">Relationship</span></span> | <span data-ttu-id="b1f10-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1f10-142">Type</span></span>   |<span data-ttu-id="b1f10-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1f10-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1f10-144">item</span><span class="sxs-lookup"><span data-stu-id="b1f10-144">item</span></span>|[<span data-ttu-id="b1f10-145">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="b1f10-145">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="b1f10-146">O contato anexado, mensagem ou evento.</span><span class="sxs-lookup"><span data-stu-id="b1f10-146">The attached contact, message or event.</span></span> <span data-ttu-id="b1f10-147">Propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="b1f10-147">Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1f10-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1f10-148">JSON representation</span></span>

<span data-ttu-id="b1f10-149">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b1f10-149">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
