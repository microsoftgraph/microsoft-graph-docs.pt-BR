---
title: Tipo de recurso chatMessageAttachment
description: Representa um anexo a uma entidade de mensagem de chat.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: RamjotSingh
ms.openlocfilehash: b4660e92643d868fbd09c693187a486fc3937584
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582568"
---
# <a name="chatmessageattachment-resource-type"></a><span data-ttu-id="765f9-103">Tipo de recurso chatMessageAttachment</span><span class="sxs-lookup"><span data-stu-id="765f9-103">chatMessageAttachment resource type</span></span>

<span data-ttu-id="765f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="765f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="765f9-105">Representa um anexo a uma entidade de mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="765f9-105">Represents an attachment to a chat message entity.</span></span>

<span data-ttu-id="765f9-106">Uma entidade de tipo é retornada como parte da API Obter mensagens `chatMessageAttachment` [de](../api/channel-list-messages.md) canal, como parte da [entidade chatMessage.](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="765f9-106">An entity of type `chatMessageAttachment` is returned as part of the [Get channel messages](../api/channel-list-messages.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="765f9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="765f9-107">Properties</span></span>
| <span data-ttu-id="765f9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="765f9-108">Property</span></span>     | <span data-ttu-id="765f9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="765f9-109">Type</span></span>   |<span data-ttu-id="765f9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="765f9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="765f9-111">id</span><span class="sxs-lookup"><span data-stu-id="765f9-111">id</span></span>|<span data-ttu-id="765f9-112">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="765f9-112">string</span></span>| <span data-ttu-id="765f9-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="765f9-113">Read-only.</span></span> <span data-ttu-id="765f9-114">ID exclusiva do anexo.</span><span class="sxs-lookup"><span data-stu-id="765f9-114">Unique id of the attachment.</span></span>|
|<span data-ttu-id="765f9-115">contentType</span><span class="sxs-lookup"><span data-stu-id="765f9-115">contentType</span></span>| <span data-ttu-id="765f9-116">string</span><span class="sxs-lookup"><span data-stu-id="765f9-116">string</span></span> | <span data-ttu-id="765f9-117">O tipo de mídia do anexo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="765f9-117">The media type of the content attachment.</span></span> <span data-ttu-id="765f9-118">Ele pode ter os seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="765f9-118">It can have the following values:</span></span> <br><ul><li><span data-ttu-id="765f9-119">`reference`: Attachment é um link para outro arquivo.</span><span class="sxs-lookup"><span data-stu-id="765f9-119">`reference`: Attachment is a link to another file.</span></span> <span data-ttu-id="765f9-120">Preencha o contentURL com o link para o objeto.</span><span class="sxs-lookup"><span data-stu-id="765f9-120">Populate the contentURL with the link to the object.</span></span></li><li><span data-ttu-id="765f9-121">Quaisquer contentTypes suportados pelo objeto Attachment da Estrutura de [Bot](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?#attachment-object)</span><span class="sxs-lookup"><span data-stu-id="765f9-121">Any contentTypes supported by the Bot Framework's [Attachment object](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?#attachment-object)</span></span></li><li><span data-ttu-id="765f9-122">`application/vnd.microsoft.card.codesnippet`: Um trecho de código.</span><span class="sxs-lookup"><span data-stu-id="765f9-122">`application/vnd.microsoft.card.codesnippet`: A code snippet.</span></span> </li><li><span data-ttu-id="765f9-123">`application/vnd.microsoft.card.announcement`: Um header de comunicado.</span><span class="sxs-lookup"><span data-stu-id="765f9-123">`application/vnd.microsoft.card.announcement`: An announcement header.</span></span> </li>|
|<span data-ttu-id="765f9-124">contentUrl</span><span class="sxs-lookup"><span data-stu-id="765f9-124">contentUrl</span></span>|<span data-ttu-id="765f9-125">string</span><span class="sxs-lookup"><span data-stu-id="765f9-125">string</span></span>|<span data-ttu-id="765f9-126">URL do conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="765f9-126">URL for the content of the attachment.</span></span> <span data-ttu-id="765f9-127">Protocolos com suporte: http, https, arquivo e dados.</span><span class="sxs-lookup"><span data-stu-id="765f9-127">Supported protocols: http, https, file and data.</span></span>|
|<span data-ttu-id="765f9-128">conteúdo</span><span class="sxs-lookup"><span data-stu-id="765f9-128">content</span></span>|<span data-ttu-id="765f9-129">string</span><span class="sxs-lookup"><span data-stu-id="765f9-129">string</span></span>|<span data-ttu-id="765f9-130">O conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="765f9-130">The content of the attachment.</span></span> <span data-ttu-id="765f9-131">Se o anexo for um [cartão rich ,](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference)de definir a propriedade como o objeto rich card.</span><span class="sxs-lookup"><span data-stu-id="765f9-131">If the attachment is a [rich card](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference), set the property to the rich card object.</span></span> <span data-ttu-id="765f9-132">Essa propriedade e contentUrl são mutuamente exclusivos.</span><span class="sxs-lookup"><span data-stu-id="765f9-132">This property and contentUrl are mutually exclusive.</span></span>|
|<span data-ttu-id="765f9-133">nome</span><span class="sxs-lookup"><span data-stu-id="765f9-133">name</span></span>|<span data-ttu-id="765f9-134">string</span><span class="sxs-lookup"><span data-stu-id="765f9-134">string</span></span>|<span data-ttu-id="765f9-135">Nome do anexo.</span><span class="sxs-lookup"><span data-stu-id="765f9-135">Name of the attachment.</span></span>|
|<span data-ttu-id="765f9-136">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="765f9-136">thumbnailUrl</span></span>| <span data-ttu-id="765f9-137">string</span><span class="sxs-lookup"><span data-stu-id="765f9-137">string</span></span> |<span data-ttu-id="765f9-138">URL para uma imagem em miniatura que o canal pode usar se for compatível com o uso de uma forma alternativa, menor de conteúdo ou contentUrl.</span><span class="sxs-lookup"><span data-stu-id="765f9-138">URL to a thumbnail image that the channel can use if it supports using an alternative, smaller form of content or contentUrl.</span></span> <span data-ttu-id="765f9-139">Por exemplo, se você definir contentType como aplicativo/word e definir contentUrl como o local do documento do Word, poderá incluir uma imagem em miniatura que representa o documento.</span><span class="sxs-lookup"><span data-stu-id="765f9-139">For example, if you set contentType to application/word and set contentUrl to the location of the Word document, you might include a thumbnail image that represents the document.</span></span> <span data-ttu-id="765f9-140">O canal poderia exibir a imagem em miniatura em vez do documento.</span><span class="sxs-lookup"><span data-stu-id="765f9-140">The channel could display the thumbnail image instead of the document.</span></span> <span data-ttu-id="765f9-141">Quando o usuário clica na imagem, o canal abriria o documento.</span><span class="sxs-lookup"><span data-stu-id="765f9-141">When the user clicks the image, the channel would open the document.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="765f9-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="765f9-142">JSON representation</span></span>
 <span data-ttu-id="765f9-143">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="765f9-143">The following is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "thumbnailUrl",
    "content",
    "contentUrl"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageAttachment"
}-->

```json
{
  "id": "string (identifier)",
  "contentType": "string",
  "contentUrl": "string",
  "content": "string",
  "name": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


