---
title: tipo de recurso chatMessageAttachment
description: Representa um anexo a uma entidade de mensagem de chat.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: clearab
ms.openlocfilehash: 2c343d3449365d34c0bda0fd35b58e029d89711f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064308"
---
# <a name="chatmessageattachment-resource-type"></a><span data-ttu-id="cf931-103">tipo de recurso chatMessageAttachment</span><span class="sxs-lookup"><span data-stu-id="cf931-103">chatMessageAttachment resource type</span></span>

<span data-ttu-id="cf931-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf931-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf931-105">Representa um anexo a uma entidade de mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="cf931-105">Represents an attachment to a chat message entity.</span></span>

<span data-ttu-id="cf931-106">Uma entidade do tipo `chatMessageAttachment` é retornada como parte da API [Get Channel messages](../api/channel-list-messages.md) , como parte da entidade [chat](chatmessage.md) .</span><span class="sxs-lookup"><span data-stu-id="cf931-106">An entity of type `chatMessageAttachment` is returned as part of the [Get channel messages](../api/channel-list-messages.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="cf931-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf931-107">Properties</span></span>
| <span data-ttu-id="cf931-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf931-108">Property</span></span>     | <span data-ttu-id="cf931-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf931-109">Type</span></span>   |<span data-ttu-id="cf931-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf931-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf931-111">id</span><span class="sxs-lookup"><span data-stu-id="cf931-111">id</span></span>|<span data-ttu-id="cf931-112">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf931-112">string</span></span>| <span data-ttu-id="cf931-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf931-113">Read-only.</span></span> <span data-ttu-id="cf931-114">ID exclusiva do anexo.</span><span class="sxs-lookup"><span data-stu-id="cf931-114">Unique id of the attachment.</span></span>|
|<span data-ttu-id="cf931-115">contentType</span><span class="sxs-lookup"><span data-stu-id="cf931-115">contentType</span></span>| <span data-ttu-id="cf931-116">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf931-116">string</span></span> | <span data-ttu-id="cf931-117">O tipo de mídia do anexo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="cf931-117">The media type of the content attachment.</span></span> <span data-ttu-id="cf931-118">Ele pode ter os seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="cf931-118">It can have the following values:</span></span> <br><ul><li><span data-ttu-id="cf931-119">`reference`: O anexo é um link para outro arquivo.</span><span class="sxs-lookup"><span data-stu-id="cf931-119">`reference`: Attachment is a link to another file.</span></span> <span data-ttu-id="cf931-120">Preencha o contentURL com o link para o objeto.</span><span class="sxs-lookup"><span data-stu-id="cf931-120">Populate the contentURL with the link to the object.</span></span></li><li><span data-ttu-id="cf931-121">Quaisquer contentTypes compatíveis com o [objeto Attachment](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?view=azure-bot-service-4.0#attachment-object) da estrutura de bot</span><span class="sxs-lookup"><span data-stu-id="cf931-121">Any contentTypes supported by the Bot Framework's [Attachment object](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?view=azure-bot-service-4.0#attachment-object)</span></span></li><li><span data-ttu-id="cf931-122">`application/vnd.microsoft.card.codesnippet`: Um trecho de código.</span><span class="sxs-lookup"><span data-stu-id="cf931-122">`application/vnd.microsoft.card.codesnippet`: A code snippet.</span></span> </li><li><span data-ttu-id="cf931-123">`application/vnd.microsoft.card.announcement`: Um cabeçalho de comunicado.</span><span class="sxs-lookup"><span data-stu-id="cf931-123">`application/vnd.microsoft.card.announcement`: An announcement header.</span></span> </li>|
|<span data-ttu-id="cf931-124">contentUrl</span><span class="sxs-lookup"><span data-stu-id="cf931-124">contentUrl</span></span>|<span data-ttu-id="cf931-125">string</span><span class="sxs-lookup"><span data-stu-id="cf931-125">string</span></span>|<span data-ttu-id="cf931-126">URL para o conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="cf931-126">URL for the content of the attachment.</span></span> <span data-ttu-id="cf931-127">Protocolos suportados: http, HTTPS, File e data.</span><span class="sxs-lookup"><span data-stu-id="cf931-127">Supported protocols: http, https, file and data.</span></span>|
|<span data-ttu-id="cf931-128">conteúdo</span><span class="sxs-lookup"><span data-stu-id="cf931-128">content</span></span>|<span data-ttu-id="cf931-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf931-129">string</span></span>|<span data-ttu-id="cf931-130">O conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="cf931-130">The content of the attachment.</span></span> <span data-ttu-id="cf931-131">Se o anexo for um [cartão rico](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference), defina a propriedade com o objeto ficha avançada.</span><span class="sxs-lookup"><span data-stu-id="cf931-131">If the attachment is a [rich card](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference), set the property to the rich card object.</span></span> <span data-ttu-id="cf931-132">Essa propriedade e contentUrl são mutuamente exclusivas.</span><span class="sxs-lookup"><span data-stu-id="cf931-132">This property and contentUrl are mutually exclusive.</span></span>|
|<span data-ttu-id="cf931-133">name</span><span class="sxs-lookup"><span data-stu-id="cf931-133">name</span></span>|<span data-ttu-id="cf931-134">string</span><span class="sxs-lookup"><span data-stu-id="cf931-134">string</span></span>|<span data-ttu-id="cf931-135">Nome do anexo.</span><span class="sxs-lookup"><span data-stu-id="cf931-135">Name of the attachment.</span></span>|
|<span data-ttu-id="cf931-136">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="cf931-136">thumbnailUrl</span></span>| <span data-ttu-id="cf931-137">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf931-137">string</span></span> |<span data-ttu-id="cf931-138">URL para uma imagem em miniatura que o canal pode usar se oferecer suporte ao uso de um formato de conteúdo ou de uma alternativa menor ou contentUrl.</span><span class="sxs-lookup"><span data-stu-id="cf931-138">URL to a thumbnail image that the channel can use if it supports using an alternative, smaller form of content or contentUrl.</span></span> <span data-ttu-id="cf931-139">Por exemplo, se você definir contentType como Application/Word e definir contentUrl como o local do documento do Word, você pode incluir uma imagem em miniatura que representa o documento.</span><span class="sxs-lookup"><span data-stu-id="cf931-139">For example, if you set contentType to application/word and set contentUrl to the location of the Word document, you might include a thumbnail image that represents the document.</span></span> <span data-ttu-id="cf931-140">O canal pode exibir a imagem em miniatura em vez do documento.</span><span class="sxs-lookup"><span data-stu-id="cf931-140">The channel could display the thumbnail image instead of the document.</span></span> <span data-ttu-id="cf931-141">Quando o usuário clica na imagem, o canal abre o documento.</span><span class="sxs-lookup"><span data-stu-id="cf931-141">When the user clicks the image, the channel would open the document.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf931-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf931-142">JSON representation</span></span>
 <span data-ttu-id="cf931-143">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="cf931-143">The following is a JSON representation of the resource</span></span>

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


