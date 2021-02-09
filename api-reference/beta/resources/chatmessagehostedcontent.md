---
title: Tipo de recurso chatMessageHostedContent
description: Um conteúdo hospedado em uma mensagem de chat
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cc4f61fb0b0e6c174be50c988d1cbb22576c4f27
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159616"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="6da77-103">Tipo de recurso chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="6da77-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="6da77-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6da77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6da77-105">Representa o conteúdo do Teams hospedado em uma mensagem de chat, como imagens ou trechos de código.</span><span class="sxs-lookup"><span data-stu-id="6da77-105">Represents Teams content hosted in a chat message, such as images or code snippets.</span></span>
<span data-ttu-id="6da77-106">[Anexos de arquivo](chatmessageattachment.md) não são conteúdo hospedado; eles são armazenados no SharePoint ou no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6da77-106">[File attachments](chatmessageattachment.md) are not hosted content; they are stored in SharePoint or OneDrive.</span></span>

## <a name="methods"></a><span data-ttu-id="6da77-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6da77-107">Methods</span></span>

| <span data-ttu-id="6da77-108">Método</span><span class="sxs-lookup"><span data-stu-id="6da77-108">Method</span></span>       | <span data-ttu-id="6da77-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6da77-109">Return Type</span></span> | <span data-ttu-id="6da77-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6da77-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6da77-111">Listar chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="6da77-111">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | [<span data-ttu-id="6da77-112">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="6da77-112">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="6da77-113">Recupere a lista de **chatMessageHostedContent** para uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="6da77-113">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="6da77-114">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="6da77-114">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="6da77-115">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="6da77-115">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="6da77-116">Leia as propriedades e os relacionamentos de um **objeto chatMessageHostedContent.**</span><span class="sxs-lookup"><span data-stu-id="6da77-116">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6da77-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6da77-117">Properties</span></span>

| <span data-ttu-id="6da77-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6da77-118">Property</span></span>     | <span data-ttu-id="6da77-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6da77-119">Type</span></span>        | <span data-ttu-id="6da77-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6da77-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6da77-121">id</span><span class="sxs-lookup"><span data-stu-id="6da77-121">id</span></span>            |<span data-ttu-id="6da77-122">String</span><span class="sxs-lookup"><span data-stu-id="6da77-122">String</span></span>       | <span data-ttu-id="6da77-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6da77-123">Read-only.</span></span> <span data-ttu-id="6da77-124">Representa o identificador de conteúdo hospedado da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="6da77-124">Represents the chat message hosted content identifier.</span></span>|
|<span data-ttu-id="6da77-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="6da77-125">contentBytes</span></span>  |<span data-ttu-id="6da77-126">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="6da77-126">Edm.Binary</span></span>   | <span data-ttu-id="6da77-127">Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="6da77-127">Write-only.</span></span> <span data-ttu-id="6da77-128">Ao postar conteúdo hospedado na nova mensagem de chat, representa os bytes da carga.</span><span class="sxs-lookup"><span data-stu-id="6da77-128">When posting new chat message hosted content, represents the bytes of the payload.</span></span> <span data-ttu-id="6da77-129">Eles são representados como uma cadeia de caracteres base64Encoded.</span><span class="sxs-lookup"><span data-stu-id="6da77-129">These are represented as a base64Encoded string.</span></span>|
|<span data-ttu-id="6da77-130">contentType</span><span class="sxs-lookup"><span data-stu-id="6da77-130">contentType</span></span>   |<span data-ttu-id="6da77-131">String</span><span class="sxs-lookup"><span data-stu-id="6da77-131">String</span></span>       | <span data-ttu-id="6da77-132">Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="6da77-132">Write-only.</span></span> <span data-ttu-id="6da77-133">Ao postar novo conteúdo hospedado de mensagem de chat, representa o tipo de conteúdo, como imagem/png.</span><span class="sxs-lookup"><span data-stu-id="6da77-133">When posting new chat message hosted content, represents the type of content, such as image/png.</span></span>|

### <a name="instance-attributes"></a><span data-ttu-id="6da77-134">Atributos de instância</span><span class="sxs-lookup"><span data-stu-id="6da77-134">Instance attributes</span></span>

<span data-ttu-id="6da77-135">Atributos de instância são propriedades com comportamentos especiais.</span><span class="sxs-lookup"><span data-stu-id="6da77-135">Instance attributes are properties with special behaviors.</span></span>
<span data-ttu-id="6da77-136">Essas propriedades são temporárias e definem o comportamento que o serviço deve executar ou fornecer valores de propriedade de curto prazo, como uma URL de download para um item que expira.</span><span class="sxs-lookup"><span data-stu-id="6da77-136">These properties are temporary and either define behavior the service should perform or provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="6da77-137">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6da77-137">Property name</span></span>                     | <span data-ttu-id="6da77-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="6da77-138">Type</span></span>   | <span data-ttu-id="6da77-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="6da77-139">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="6da77-140">@microsoft.graph.temporaryId</span><span class="sxs-lookup"><span data-stu-id="6da77-140">@microsoft.graph.temporaryId</span></span>      | <span data-ttu-id="6da77-141">string</span><span class="sxs-lookup"><span data-stu-id="6da77-141">string</span></span> | <span data-ttu-id="6da77-142">Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="6da77-142">Write-only.</span></span> <span data-ttu-id="6da77-143">Representa a temporaryId do conteúdo hospedado enquanto publica uma mensagem para se referir ao conteúdo hospedado no recurso **chatMessage** que está sendo enviado.</span><span class="sxs-lookup"><span data-stu-id="6da77-143">Represents the temporaryId for the hosted content while posting a message to refer to the hosted content in **chatMessage** resource being sent.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6da77-144">Relações</span><span class="sxs-lookup"><span data-stu-id="6da77-144">Relationships</span></span>

<span data-ttu-id="6da77-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6da77-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6da77-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6da77-146">JSON representation</span></span>

<span data-ttu-id="6da77-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6da77-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "keyProperty": "id"
}-->

```json
{
  "@microsoft.graph.temporaryId": "String (identifier)",
  "id": "String (identifier)",
  "contentBytes": "String (binary)",
  "contentType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageHostedContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


