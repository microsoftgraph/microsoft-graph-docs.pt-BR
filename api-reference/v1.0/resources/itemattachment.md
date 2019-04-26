---
title: Tipo de recurso itemAttachment
description: 'Um contato, evento ou mensagem que está anexado a outro evento, mensagem ou postagem.  '
localization_priority: Priority
ms.openlocfilehash: df996175e545b78f4ca9a1b6271b9cb012ffffce
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584814"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="173b2-103">Tipo de recurso itemAttachment</span><span class="sxs-lookup"><span data-stu-id="173b2-103">itemAttachment resource type</span></span>

<span data-ttu-id="173b2-104">Um contato, evento ou mensagem que está anexado a outro evento, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="173b2-104">A contact, event, or message that's attached to another event, message, or post.</span></span>  

<span data-ttu-id="173b2-105">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="173b2-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="173b2-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="173b2-106">Methods</span></span>

| <span data-ttu-id="173b2-107">Método</span><span class="sxs-lookup"><span data-stu-id="173b2-107">Method</span></span>       | <span data-ttu-id="173b2-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="173b2-108">Return Type</span></span>  |<span data-ttu-id="173b2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="173b2-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="173b2-110">Get</span><span class="sxs-lookup"><span data-stu-id="173b2-110">Get</span></span>](../api/attachment-get.md) | <span data-ttu-id="173b2-111">[itemAttachment](itemattachment.md)</span><span class="sxs-lookup"><span data-stu-id="173b2-111">[itemAttachment](itemattachment.md),</span></span> |<span data-ttu-id="173b2-112">Leia as propriedades e os relacionamentos do objeto itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="173b2-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="173b2-113">Delete</span><span class="sxs-lookup"><span data-stu-id="173b2-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="173b2-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="173b2-114">None</span></span> |<span data-ttu-id="173b2-115">Exclua o objeto itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="173b2-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="173b2-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="173b2-116">Properties</span></span>
| <span data-ttu-id="173b2-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="173b2-117">Property</span></span>     | <span data-ttu-id="173b2-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="173b2-118">Type</span></span>   |<span data-ttu-id="173b2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="173b2-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="173b2-120">contentType</span><span class="sxs-lookup"><span data-stu-id="173b2-120">contentType</span></span>|<span data-ttu-id="173b2-121">String</span><span class="sxs-lookup"><span data-stu-id="173b2-121">String</span></span>|<span data-ttu-id="173b2-122">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="173b2-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="173b2-123">id</span><span class="sxs-lookup"><span data-stu-id="173b2-123">id</span></span>|<span data-ttu-id="173b2-124">String</span><span class="sxs-lookup"><span data-stu-id="173b2-124">String</span></span>| <span data-ttu-id="173b2-125">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="173b2-125">The attachment ID.</span></span>|
|<span data-ttu-id="173b2-126">isInline</span><span class="sxs-lookup"><span data-stu-id="173b2-126">isInline</span></span>|<span data-ttu-id="173b2-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="173b2-127">Boolean</span></span>|<span data-ttu-id="173b2-128">Defina como verdadeiro se o anexo estiver embutido, como uma imagem incorporada no corpo do item.</span><span class="sxs-lookup"><span data-stu-id="173b2-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="173b2-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="173b2-129">lastModifiedDateTime</span></span>|<span data-ttu-id="173b2-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="173b2-130">DateTimeOffset</span></span>|<span data-ttu-id="173b2-131">Última data e hora em que o anexo foi alterado.</span><span class="sxs-lookup"><span data-stu-id="173b2-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="173b2-132">name</span><span class="sxs-lookup"><span data-stu-id="173b2-132">name</span></span>|<span data-ttu-id="173b2-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="173b2-133">String</span></span>|<span data-ttu-id="173b2-134">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="173b2-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="173b2-135">size</span><span class="sxs-lookup"><span data-stu-id="173b2-135">size</span></span>|<span data-ttu-id="173b2-136">Int32</span><span class="sxs-lookup"><span data-stu-id="173b2-136">Int32</span></span>|<span data-ttu-id="173b2-137">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="173b2-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="173b2-138">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="173b2-138">Relationships</span></span>
| <span data-ttu-id="173b2-139">Relação</span><span class="sxs-lookup"><span data-stu-id="173b2-139">Relationship</span></span> | <span data-ttu-id="173b2-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="173b2-140">Type</span></span>   |<span data-ttu-id="173b2-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="173b2-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="173b2-142">item</span><span class="sxs-lookup"><span data-stu-id="173b2-142">item</span></span>|[<span data-ttu-id="173b2-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="173b2-143">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="173b2-p101">A mensagem ou evento anexado. Propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="173b2-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="173b2-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="173b2-146">JSON representation</span></span>

<span data-ttu-id="173b2-147">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="173b2-147">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "baseType": "microsoft.graph.attachment",
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
