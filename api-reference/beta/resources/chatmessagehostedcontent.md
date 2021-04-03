---
title: Tipo de recurso chatMessageHostedContent
description: Um conteúdo hospedado em uma mensagem de chat
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 842ccdcad3f185eb64572c91ce5b82d673a1d43f
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582561"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="3aea3-103">Tipo de recurso chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="3aea3-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="3aea3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aea3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3aea3-105">Representa o conteúdo do Teams hospedado em uma mensagem de chat, como imagens ou trechos de código.</span><span class="sxs-lookup"><span data-stu-id="3aea3-105">Represents Teams content hosted in a chat message, such as images or code snippets.</span></span>
<span data-ttu-id="3aea3-106">[Anexos de arquivo](chatmessageattachment.md) não são conteúdo hospedado; eles são armazenados no SharePoint ou no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3aea3-106">[File attachments](chatmessageattachment.md) are not hosted content; they are stored in SharePoint or OneDrive.</span></span>

## <a name="methods"></a><span data-ttu-id="3aea3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="3aea3-107">Methods</span></span>

| <span data-ttu-id="3aea3-108">Método</span><span class="sxs-lookup"><span data-stu-id="3aea3-108">Method</span></span>       | <span data-ttu-id="3aea3-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3aea3-109">Return Type</span></span> | <span data-ttu-id="3aea3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3aea3-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3aea3-111">Listar chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="3aea3-111">List chatMessageHostedContent</span></span>](../api/chatmessage-list-hostedcontents.md) | <span data-ttu-id="3aea3-112">[coleção chatMessageHostedContent](chatmessagehostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="3aea3-112">[chatMessageHostedContent](chatmessagehostedcontent.md) collection</span></span> | <span data-ttu-id="3aea3-113">Recupere a lista de **chatMessageHostedContent** para uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="3aea3-113">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="3aea3-114">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="3aea3-114">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="3aea3-115">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="3aea3-115">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="3aea3-116">Leia as propriedades e as relações de um **objeto chatMessageHostedContent.**</span><span class="sxs-lookup"><span data-stu-id="3aea3-116">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3aea3-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3aea3-117">Properties</span></span>

<span data-ttu-id="3aea3-118">chatMessageHostedContent deriva do trabalho em [equipeHostedContent](teamworkhostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="3aea3-118">chatMessageHostedContent derives from [teamworkHostedContent](teamworkhostedcontent.md)</span></span>

| <span data-ttu-id="3aea3-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3aea3-119">Property</span></span>     | <span data-ttu-id="3aea3-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="3aea3-120">Type</span></span>        | <span data-ttu-id="3aea3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3aea3-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3aea3-122">id</span><span class="sxs-lookup"><span data-stu-id="3aea3-122">id</span></span>            |<span data-ttu-id="3aea3-123">String</span><span class="sxs-lookup"><span data-stu-id="3aea3-123">String</span></span>       | <span data-ttu-id="3aea3-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3aea3-124">Read-only.</span></span> <span data-ttu-id="3aea3-125">Representa o identificador de conteúdo hospedado da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="3aea3-125">Represents the chat message hosted content identifier.</span></span>|
|<span data-ttu-id="3aea3-126">contentBytes</span><span class="sxs-lookup"><span data-stu-id="3aea3-126">contentBytes</span></span>  |<span data-ttu-id="3aea3-127">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="3aea3-127">Edm.Binary</span></span>   | <span data-ttu-id="3aea3-128">Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="3aea3-128">Write-only.</span></span> <span data-ttu-id="3aea3-129">Ao postar o conteúdo hospedado da nova mensagem de chat, representa os bytes da carga.</span><span class="sxs-lookup"><span data-stu-id="3aea3-129">When posting new chat message hosted content, represents the bytes of the payload.</span></span> <span data-ttu-id="3aea3-130">Eles são representados como uma cadeia de caracteres base64Encoded.</span><span class="sxs-lookup"><span data-stu-id="3aea3-130">These are represented as a base64Encoded string.</span></span>|
|<span data-ttu-id="3aea3-131">contentType</span><span class="sxs-lookup"><span data-stu-id="3aea3-131">contentType</span></span>   |<span data-ttu-id="3aea3-132">String</span><span class="sxs-lookup"><span data-stu-id="3aea3-132">String</span></span>       | <span data-ttu-id="3aea3-133">Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="3aea3-133">Write-only.</span></span> <span data-ttu-id="3aea3-134">Ao postar conteúdo hospedado na nova mensagem de chat, representa o tipo de conteúdo, como image/png.</span><span class="sxs-lookup"><span data-stu-id="3aea3-134">When posting new chat message hosted content, represents the type of content, such as image/png.</span></span>|

### <a name="instance-attributes"></a><span data-ttu-id="3aea3-135">Atributos de instância</span><span class="sxs-lookup"><span data-stu-id="3aea3-135">Instance attributes</span></span>

<span data-ttu-id="3aea3-136">Atributos de instância são propriedades com comportamentos especiais.</span><span class="sxs-lookup"><span data-stu-id="3aea3-136">Instance attributes are properties with special behaviors.</span></span>
<span data-ttu-id="3aea3-137">Essas propriedades são temporárias e definem o comportamento que o serviço deve executar ou fornecer valores de propriedade de curto prazo, como uma URL de download para um item que expira.</span><span class="sxs-lookup"><span data-stu-id="3aea3-137">These properties are temporary and either define behavior the service should perform or provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="3aea3-138">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3aea3-138">Property name</span></span>                     | <span data-ttu-id="3aea3-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="3aea3-139">Type</span></span>   | <span data-ttu-id="3aea3-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="3aea3-140">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="3aea3-141">@microsoft.graph.temporaryId</span><span class="sxs-lookup"><span data-stu-id="3aea3-141">@microsoft.graph.temporaryId</span></span>      | <span data-ttu-id="3aea3-142">string</span><span class="sxs-lookup"><span data-stu-id="3aea3-142">string</span></span> | <span data-ttu-id="3aea3-143">Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="3aea3-143">Write-only.</span></span> <span data-ttu-id="3aea3-144">Representa a temporaryId do conteúdo hospedado ao postar uma mensagem para se referir ao conteúdo hospedado no **recurso chatMessage** que está sendo enviado.</span><span class="sxs-lookup"><span data-stu-id="3aea3-144">Represents the temporaryId for the hosted content while posting a message to refer to the hosted content in **chatMessage** resource being sent.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3aea3-145">Relações</span><span class="sxs-lookup"><span data-stu-id="3aea3-145">Relationships</span></span>

<span data-ttu-id="3aea3-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3aea3-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3aea3-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3aea3-147">JSON representation</span></span>

<span data-ttu-id="3aea3-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3aea3-148">The following is a JSON representation of the resource.</span></span>

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


