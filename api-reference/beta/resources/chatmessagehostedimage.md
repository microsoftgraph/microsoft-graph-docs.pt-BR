---
title: tipo de recurso chatMessageHostedImage
description: Representa uma imagem hospedada dentro de um chat.
localization_priority: Normal
author: clearab
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e217234b8ea6c6510b85af1bf1002e589e4366e0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974000"
---
# <a name="chatmessagehostedimage-resource-type"></a><span data-ttu-id="79a7b-103">tipo de recurso chatMessageHostedImage</span><span class="sxs-lookup"><span data-stu-id="79a7b-103">chatMessageHostedImage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79a7b-104">Representa uma imagem hospedada dentro de um [chat](../resources/chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="79a7b-104">Represents a hosted image inside a [chatMessage](../resources/chatmessage.md).</span></span>

<span data-ttu-id="79a7b-105">Imagens hospedadas são as imagens que aparecem no corpo da mensagem **. o conteúdo** em \<uma marca img> com um atributo src que começa `https://graph.microsoft.com`com.</span><span class="sxs-lookup"><span data-stu-id="79a7b-105">Hosted images are the images that appear in the message's **body.content** in an \<img> tag with a src attribute that starts with `https://graph.microsoft.com`.</span></span>

<span data-ttu-id="79a7b-106">Nem todas as imagens em uma mensagem são hospedadas, o Microsoft Teams também oferece suporte a imagens públicas (onde o atributo img src aponta para um site público).</span><span class="sxs-lookup"><span data-stu-id="79a7b-106">Not all images in a message are hosted images, Microsoft Teams also supports public images (where the img src attribute points to a public website).</span></span>

## <a name="methods"></a><span data-ttu-id="79a7b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="79a7b-107">Methods</span></span>

| <span data-ttu-id="79a7b-108">Método</span><span class="sxs-lookup"><span data-stu-id="79a7b-108">Method</span></span>       | <span data-ttu-id="79a7b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="79a7b-109">Return Type</span></span>  |<span data-ttu-id="79a7b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="79a7b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="79a7b-111">Listar chatMessageHostedImages em um chat</span><span class="sxs-lookup"><span data-stu-id="79a7b-111">List chatMessageHostedImages in a chatMessage</span></span>](../api/chatmessagehostedimage-list-hostedimages.md) | <span data-ttu-id="79a7b-112">coleção [chatMessageHostedImage](chatmessagehostedimage.md)</span><span class="sxs-lookup"><span data-stu-id="79a7b-112">[chatMessageHostedImage](chatmessagehostedimage.md) collection</span></span> | <span data-ttu-id="79a7b-113">Lista de todas as imagens hospedadas em um **chat**.</span><span class="sxs-lookup"><span data-stu-id="79a7b-113">List of all hosted images in a **chatMessage**.</span></span>|
|[<span data-ttu-id="79a7b-114">Obter chatMessageHostedImage</span><span class="sxs-lookup"><span data-stu-id="79a7b-114">Get chatMessageHostedImage</span></span>](../api/chatmessagehostedimage-get.md) | [<span data-ttu-id="79a7b-115">chatMessageHostedImage</span><span class="sxs-lookup"><span data-stu-id="79a7b-115">chatMessageHostedImage</span></span>](chatmessagehostedimage.md) | <span data-ttu-id="79a7b-116">Obtenha uma única imagem hospedada.</span><span class="sxs-lookup"><span data-stu-id="79a7b-116">Get a single hosted image.</span></span>|
|[<span data-ttu-id="79a7b-117">chatMessageHostedImage: GetBytes</span><span class="sxs-lookup"><span data-stu-id="79a7b-117">chatMessageHostedImage: getBytes</span></span>](../api/chatmessagehostedimage-getbytes.md) | <span data-ttu-id="79a7b-118">Tipo de conteúdo: image/jpeg</span><span class="sxs-lookup"><span data-stu-id="79a7b-118">Content-type: image/jpeg</span></span> | <span data-ttu-id="79a7b-119">Obtenha os bytes brutos da imagem hospedada.</span><span class="sxs-lookup"><span data-stu-id="79a7b-119">Get the raw bytes of the hosted image.</span></span>|

## <a name="properties"></a><span data-ttu-id="79a7b-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79a7b-120">Properties</span></span>

| <span data-ttu-id="79a7b-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79a7b-121">Property</span></span>     | <span data-ttu-id="79a7b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="79a7b-122">Type</span></span>   |<span data-ttu-id="79a7b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="79a7b-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79a7b-124">id</span><span class="sxs-lookup"><span data-stu-id="79a7b-124">id</span></span>|<span data-ttu-id="79a7b-125">String</span><span class="sxs-lookup"><span data-stu-id="79a7b-125">String</span></span>| <span data-ttu-id="79a7b-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="79a7b-126">Read-only.</span></span> <span data-ttu-id="79a7b-127">ID única da mensagem.</span><span class="sxs-lookup"><span data-stu-id="79a7b-127">Unique ID of the message.</span></span>|
|<span data-ttu-id="79a7b-128">URL</span><span class="sxs-lookup"><span data-stu-id="79a7b-128">URL</span></span>| <span data-ttu-id="79a7b-129">string</span><span class="sxs-lookup"><span data-stu-id="79a7b-129">string</span></span> | <span data-ttu-id="79a7b-130">A URL da qual recuperar o conteúdo da imagem.</span><span class="sxs-lookup"><span data-stu-id="79a7b-130">The url to retrieve the image contents from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="79a7b-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79a7b-131">JSON representation</span></span>

<span data-ttu-id="79a7b-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79a7b-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageHostedImage"
}-->

```json
{
  "id": "string (identifier)",
  "url": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
