---
title: Tipo de recurso itemAttachment
description: 'Um contato, evento ou mensagem que está anexado a outro evento, mensagem ou postagem.  '
ms.openlocfilehash: 79097b10327d895a41090e068a2fd8e9681df125
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005293"
---
# <a name="itemattachment-resource-type"></a><span data-ttu-id="270ef-103">Tipo de recurso itemAttachment</span><span class="sxs-lookup"><span data-stu-id="270ef-103">itemAttachment resource type</span></span>

<span data-ttu-id="270ef-104">Um contato, evento ou mensagem que está anexado a outro evento, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="270ef-104">A contact, event, or message that's attached to another event, message, or post.</span></span>  

<span data-ttu-id="270ef-105">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="270ef-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="270ef-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="270ef-106">Methods</span></span>

| <span data-ttu-id="270ef-107">Método</span><span class="sxs-lookup"><span data-stu-id="270ef-107">Method</span></span>       | <span data-ttu-id="270ef-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="270ef-108">Return Type</span></span>  |<span data-ttu-id="270ef-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="270ef-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="270ef-110">Get</span><span class="sxs-lookup"><span data-stu-id="270ef-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="270ef-111">itemAttachment</span><span class="sxs-lookup"><span data-stu-id="270ef-111">itemAttachment</span></span>](itemattachment.md) |<span data-ttu-id="270ef-112">Leia as propriedades e os relacionamentos do objeto itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="270ef-112">Read properties and relationships of itemAttachment object.</span></span>|
|[<span data-ttu-id="270ef-113">Delete</span><span class="sxs-lookup"><span data-stu-id="270ef-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="270ef-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="270ef-114">None</span></span> |<span data-ttu-id="270ef-115">Exclua o objeto itemAttachment.</span><span class="sxs-lookup"><span data-stu-id="270ef-115">Delete itemAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="270ef-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="270ef-116">Properties</span></span>
| <span data-ttu-id="270ef-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="270ef-117">Property</span></span>     | <span data-ttu-id="270ef-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="270ef-118">Type</span></span>   |<span data-ttu-id="270ef-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="270ef-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="270ef-120">contentType</span><span class="sxs-lookup"><span data-stu-id="270ef-120">contentType</span></span>|<span data-ttu-id="270ef-121">String</span><span class="sxs-lookup"><span data-stu-id="270ef-121">String</span></span>|<span data-ttu-id="270ef-122">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="270ef-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="270ef-123">id</span><span class="sxs-lookup"><span data-stu-id="270ef-123">id</span></span>|<span data-ttu-id="270ef-124">String</span><span class="sxs-lookup"><span data-stu-id="270ef-124">String</span></span>| <span data-ttu-id="270ef-125">A ID do anexo.</span><span class="sxs-lookup"><span data-stu-id="270ef-125">The attachment ID.</span></span>|
|<span data-ttu-id="270ef-126">isInline</span><span class="sxs-lookup"><span data-stu-id="270ef-126">isInline</span></span>|<span data-ttu-id="270ef-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="270ef-127">Boolean</span></span>|<span data-ttu-id="270ef-128">Defina como verdadeiro se o anexo estiver embutido, como uma imagem incorporada no corpo do item.</span><span class="sxs-lookup"><span data-stu-id="270ef-128">Set to true if the attachment is inline, such as an embedded image within the body of the item.</span></span>|
|<span data-ttu-id="270ef-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="270ef-129">lastModifiedDateTime</span></span>|<span data-ttu-id="270ef-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="270ef-130">DateTimeOffset</span></span>|<span data-ttu-id="270ef-131">Última data e hora em que o anexo foi alterado.</span><span class="sxs-lookup"><span data-stu-id="270ef-131">The last time and date that the attachment was modified.</span></span>|
|<span data-ttu-id="270ef-132">name</span><span class="sxs-lookup"><span data-stu-id="270ef-132">name</span></span>|<span data-ttu-id="270ef-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="270ef-133">String</span></span>|<span data-ttu-id="270ef-134">O nome de exibição do anexo.</span><span class="sxs-lookup"><span data-stu-id="270ef-134">The display name of the attachment.</span></span>|
|<span data-ttu-id="270ef-135">size</span><span class="sxs-lookup"><span data-stu-id="270ef-135">size</span></span>|<span data-ttu-id="270ef-136">Int32</span><span class="sxs-lookup"><span data-stu-id="270ef-136">Int32</span></span>|<span data-ttu-id="270ef-137">O tamanho do anexo em bytes.</span><span class="sxs-lookup"><span data-stu-id="270ef-137">The size in bytes of the attachment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="270ef-138">Relações</span><span class="sxs-lookup"><span data-stu-id="270ef-138">Relationships</span></span>
| <span data-ttu-id="270ef-139">Relação</span><span class="sxs-lookup"><span data-stu-id="270ef-139">Relationship</span></span> | <span data-ttu-id="270ef-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="270ef-140">Type</span></span>   |<span data-ttu-id="270ef-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="270ef-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="270ef-142">item</span><span class="sxs-lookup"><span data-stu-id="270ef-142">item</span></span>|[<span data-ttu-id="270ef-143">OutlookItem</span><span class="sxs-lookup"><span data-stu-id="270ef-143">OutlookItem</span></span>](outlookitem.md)|<span data-ttu-id="270ef-p101">A mensagem ou evento anexado. Propriedade de navegação.</span><span class="sxs-lookup"><span data-stu-id="270ef-p101">The attached message or event. Navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="270ef-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="270ef-146">JSON representation</span></span>

<span data-ttu-id="270ef-147">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="270ef-147">Here is a JSON representation of the resource</span></span>

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
