---
title: tipo de recurso chatMessageHostedContent
description: Um conteúdo hospedado em uma mensagem de chat
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: aff1033a68f2e98b5ea5f1ca940a2be026ae18c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064266"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="0bc30-103">tipo de recurso chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="0bc30-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="0bc30-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bc30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bc30-105">Representa o conteúdo de equipes hospedados em uma mensagem de chat, como imagens ou trechos de código.</span><span class="sxs-lookup"><span data-stu-id="0bc30-105">Represents Teams content hosted in a chat message, such as images or code snippets.</span></span>
<span data-ttu-id="0bc30-106">[Anexos de arquivo](chatmessageattachment.md) não são conteúdo hospedado; Eles são armazenados no SharePoint ou no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="0bc30-106">[File attachments](chatmessageattachment.md) are not hosted content; they are stored in SharePoint or OneDrive.</span></span>

## <a name="methods"></a><span data-ttu-id="0bc30-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="0bc30-107">Methods</span></span>

| <span data-ttu-id="0bc30-108">Método</span><span class="sxs-lookup"><span data-stu-id="0bc30-108">Method</span></span>       | <span data-ttu-id="0bc30-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0bc30-109">Return Type</span></span> | <span data-ttu-id="0bc30-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bc30-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0bc30-111">Listar chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="0bc30-111">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | [<span data-ttu-id="0bc30-112">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="0bc30-112">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="0bc30-113">Recupere a lista de **chatMessageHostedContent** para uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="0bc30-113">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="0bc30-114">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="0bc30-114">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="0bc30-115">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="0bc30-115">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="0bc30-116">Leia as propriedades e os relacionamentos de um objeto **chatMessageHostedContent** .</span><span class="sxs-lookup"><span data-stu-id="0bc30-116">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0bc30-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0bc30-117">Properties</span></span>

| <span data-ttu-id="0bc30-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bc30-118">Property</span></span>     | <span data-ttu-id="0bc30-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bc30-119">Type</span></span>        | <span data-ttu-id="0bc30-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bc30-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0bc30-121">id</span><span class="sxs-lookup"><span data-stu-id="0bc30-121">id</span></span>            |<span data-ttu-id="0bc30-122">String</span><span class="sxs-lookup"><span data-stu-id="0bc30-122">String</span></span>       | <span data-ttu-id="0bc30-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0bc30-123">Read-only.</span></span> <span data-ttu-id="0bc30-124">Representa o identificador de conteúdo hospedado da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="0bc30-124">Represents the chat message hosted content identifier.</span></span>|
|<span data-ttu-id="0bc30-125">contentBytes</span><span class="sxs-lookup"><span data-stu-id="0bc30-125">contentBytes</span></span>  |<span data-ttu-id="0bc30-126">Edm.Binary</span><span class="sxs-lookup"><span data-stu-id="0bc30-126">Edm.Binary</span></span>   | <span data-ttu-id="0bc30-127">Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="0bc30-127">Write-only.</span></span> <span data-ttu-id="0bc30-128">Ao lançar o novo conteúdo hospedado da mensagem de chat, representa os bytes da carga.</span><span class="sxs-lookup"><span data-stu-id="0bc30-128">When posting new chat message hosted content, represents the bytes of the payload.</span></span> <span data-ttu-id="0bc30-129">Eles são representados como uma cadeia de caracteres base64Encoded.</span><span class="sxs-lookup"><span data-stu-id="0bc30-129">These are represented as a base64Encoded string.</span></span>|
|<span data-ttu-id="0bc30-130">contentType</span><span class="sxs-lookup"><span data-stu-id="0bc30-130">contentType</span></span>   |<span data-ttu-id="0bc30-131">String</span><span class="sxs-lookup"><span data-stu-id="0bc30-131">String</span></span>       | <span data-ttu-id="0bc30-132">Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="0bc30-132">Write-only.</span></span> <span data-ttu-id="0bc30-133">Ao lançar o novo conteúdo hospedado da mensagem de chat, representa o tipo de conteúdo, como image/png.</span><span class="sxs-lookup"><span data-stu-id="0bc30-133">When posting new chat message hosted content, represents the type of content, such as image/png.</span></span>|

### <a name="instance-attributes"></a><span data-ttu-id="0bc30-134">Atributos de instância</span><span class="sxs-lookup"><span data-stu-id="0bc30-134">Instance attributes</span></span>

<span data-ttu-id="0bc30-135">Atributos de instância são propriedades com comportamentos especiais.</span><span class="sxs-lookup"><span data-stu-id="0bc30-135">Instance attributes are properties with special behaviors.</span></span>
<span data-ttu-id="0bc30-136">Essas propriedades são temporárias e definem o comportamento que o serviço deve executar ou fornecer valores de propriedade de curto prazo, como uma URL de download para um item que expira.</span><span class="sxs-lookup"><span data-stu-id="0bc30-136">These properties are temporary and either define behavior the service should perform or provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="0bc30-137">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="0bc30-137">Property name</span></span>                     | <span data-ttu-id="0bc30-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bc30-138">Type</span></span>   | <span data-ttu-id="0bc30-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bc30-139">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="0bc30-140">@microsoft. Graph. TemporaryId</span><span class="sxs-lookup"><span data-stu-id="0bc30-140">@microsoft.graph.temporaryId</span></span>      | <span data-ttu-id="0bc30-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bc30-141">string</span></span> | <span data-ttu-id="0bc30-142">Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="0bc30-142">Write-only.</span></span> <span data-ttu-id="0bc30-143">Representa o TemporaryId do conteúdo hospedado durante a postagem de uma mensagem para fazer referência ao conteúdo hospedado no recurso **chat** que está sendo enviado.</span><span class="sxs-lookup"><span data-stu-id="0bc30-143">Represents the temporaryId for the hosted content while posting a message to refer to the hosted content in **chatMessage** resource being sent.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bc30-144">Relações</span><span class="sxs-lookup"><span data-stu-id="0bc30-144">Relationships</span></span>

<span data-ttu-id="0bc30-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0bc30-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0bc30-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0bc30-146">JSON representation</span></span>

<span data-ttu-id="0bc30-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0bc30-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "baseType": "",
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


