---
title: Tipo de recurso chatMessageHostedContent
description: Um conteúdo hospedado em uma mensagem de chat
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c2434253ef303123ac7d64695cdbbc6172d7989c
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50626227"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="281bf-103">Tipo de recurso chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="281bf-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="281bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="281bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="281bf-105">Representa o conteúdo do Teams hospedado em uma mensagem de chat, como imagens ou trechos de código.</span><span class="sxs-lookup"><span data-stu-id="281bf-105">Represents Teams content hosted in a chat message, such as images or code snippets.</span></span>
<span data-ttu-id="281bf-106">[Anexos de arquivo](chatmessageattachment.md) não são conteúdo hospedado; eles são armazenados no SharePoint ou no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="281bf-106">[File attachments](chatmessageattachment.md) are not hosted content; they are stored in SharePoint or OneDrive.</span></span>

## <a name="methods"></a><span data-ttu-id="281bf-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="281bf-107">Methods</span></span>

| <span data-ttu-id="281bf-108">Método</span><span class="sxs-lookup"><span data-stu-id="281bf-108">Method</span></span>       | <span data-ttu-id="281bf-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="281bf-109">Return Type</span></span> | <span data-ttu-id="281bf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="281bf-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="281bf-111">Listar chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="281bf-111">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | <span data-ttu-id="281bf-112">[coleção chatMessageHostedContent](chatmessagehostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="281bf-112">[chatMessageHostedContent](chatmessagehostedcontent.md) collection</span></span> | <span data-ttu-id="281bf-113">Recupere a lista de **chatMessageHostedContent** para uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="281bf-113">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="281bf-114">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="281bf-114">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="281bf-115">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="281bf-115">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="281bf-116">Leia as propriedades e as relações de um **objeto chatMessageHostedContent.**</span><span class="sxs-lookup"><span data-stu-id="281bf-116">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="281bf-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="281bf-117">Properties</span></span>

<span data-ttu-id="281bf-118">chatMessageHostedContent deriva do trabalho em [equipeHostedContent](teamworkhostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="281bf-118">chatMessageHostedContent derives from [teamworkHostedContent](teamworkhostedcontent.md)</span></span>

| <span data-ttu-id="281bf-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="281bf-119">Property</span></span>     | <span data-ttu-id="281bf-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="281bf-120">Type</span></span>        | <span data-ttu-id="281bf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="281bf-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="281bf-122">id</span><span class="sxs-lookup"><span data-stu-id="281bf-122">id</span></span>            |<span data-ttu-id="281bf-123">String</span><span class="sxs-lookup"><span data-stu-id="281bf-123">String</span></span>       | <span data-ttu-id="281bf-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="281bf-124">Read-only.</span></span> <span data-ttu-id="281bf-125">Representa o identificador de conteúdo hospedado da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="281bf-125">Represents the chat message hosted content identifier.</span></span>|
|<span data-ttu-id="281bf-126">contentBytes</span><span class="sxs-lookup"><span data-stu-id="281bf-126">contentBytes</span></span>  |<span data-ttu-id="281bf-127">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="281bf-127">Edm.Binary</span></span>   | <span data-ttu-id="281bf-128">Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="281bf-128">Write-only.</span></span> <span data-ttu-id="281bf-129">Ao postar o conteúdo hospedado da nova mensagem de chat, representa os bytes da carga.</span><span class="sxs-lookup"><span data-stu-id="281bf-129">When posting new chat message hosted content, represents the bytes of the payload.</span></span> <span data-ttu-id="281bf-130">Eles são representados como uma cadeia de caracteres base64Encoded.</span><span class="sxs-lookup"><span data-stu-id="281bf-130">These are represented as a base64Encoded string.</span></span>|
|<span data-ttu-id="281bf-131">contentType</span><span class="sxs-lookup"><span data-stu-id="281bf-131">contentType</span></span>   |<span data-ttu-id="281bf-132">String</span><span class="sxs-lookup"><span data-stu-id="281bf-132">String</span></span>       | <span data-ttu-id="281bf-133">Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="281bf-133">Write-only.</span></span> <span data-ttu-id="281bf-134">Ao postar conteúdo hospedado na nova mensagem de chat, representa o tipo de conteúdo, como image/png.</span><span class="sxs-lookup"><span data-stu-id="281bf-134">When posting new chat message hosted content, represents the type of content, such as image/png.</span></span>|

### <a name="instance-attributes"></a><span data-ttu-id="281bf-135">Atributos de instância</span><span class="sxs-lookup"><span data-stu-id="281bf-135">Instance attributes</span></span>

<span data-ttu-id="281bf-136">Atributos de instância são propriedades com comportamentos especiais.</span><span class="sxs-lookup"><span data-stu-id="281bf-136">Instance attributes are properties with special behaviors.</span></span>
<span data-ttu-id="281bf-137">Essas propriedades são temporárias e definem o comportamento que o serviço deve executar ou fornecer valores de propriedade de curto prazo, como uma URL de download para um item que expira.</span><span class="sxs-lookup"><span data-stu-id="281bf-137">These properties are temporary and either define behavior the service should perform or provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="281bf-138">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="281bf-138">Property name</span></span>                     | <span data-ttu-id="281bf-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="281bf-139">Type</span></span>   | <span data-ttu-id="281bf-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="281bf-140">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="281bf-141">@microsoft.graph.temporaryId</span><span class="sxs-lookup"><span data-stu-id="281bf-141">@microsoft.graph.temporaryId</span></span>      | <span data-ttu-id="281bf-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="281bf-142">string</span></span> | <span data-ttu-id="281bf-143">Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="281bf-143">Write-only.</span></span> <span data-ttu-id="281bf-144">Representa a temporaryId do conteúdo hospedado ao postar uma mensagem para se referir ao conteúdo hospedado no **recurso chatMessage** que está sendo enviado.</span><span class="sxs-lookup"><span data-stu-id="281bf-144">Represents the temporaryId for the hosted content while posting a message to refer to the hosted content in **chatMessage** resource being sent.</span></span>|

## <a name="relationships"></a><span data-ttu-id="281bf-145">Relações</span><span class="sxs-lookup"><span data-stu-id="281bf-145">Relationships</span></span>

<span data-ttu-id="281bf-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="281bf-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="281bf-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="281bf-147">JSON representation</span></span>

<span data-ttu-id="281bf-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="281bf-148">The following is a JSON representation of the resource.</span></span>

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


