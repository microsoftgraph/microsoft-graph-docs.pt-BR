---
title: tipo de recurso chatMessageHostedContent
description: Um conteúdo hospedado em uma mensagem de chat
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 421ed3b1c439a7ae550100a113c651ab3e0a34b9
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791066"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="df694-103">tipo de recurso chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="df694-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="df694-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df694-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df694-105">Representa o conteúdo de equipes hospedados em uma mensagem de chat, como imagens ou trechos de código.</span><span class="sxs-lookup"><span data-stu-id="df694-105">Represents Teams content hosted in a chat message, such as images or code snippets.</span></span>
<span data-ttu-id="df694-106">[Anexos de arquivo](chatmessageattachment.md) não são conteúdo hospedado, eles são armazenados no SharePoint ou no onedrive.</span><span class="sxs-lookup"><span data-stu-id="df694-106">[File attachments](chatmessageattachment.md) are not hosted content, they are stored in SharePoint or OneDrive.</span></span>

## <a name="methods"></a><span data-ttu-id="df694-107">Methods</span><span class="sxs-lookup"><span data-stu-id="df694-107">Methods</span></span>

| <span data-ttu-id="df694-108">Método</span><span class="sxs-lookup"><span data-stu-id="df694-108">Method</span></span>       | <span data-ttu-id="df694-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="df694-109">Return Type</span></span> | <span data-ttu-id="df694-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="df694-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="df694-111">Listar chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="df694-111">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | [<span data-ttu-id="df694-112">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="df694-112">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="df694-113">Recupere a lista de **chatMessageHostedContent** para uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="df694-113">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="df694-114">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="df694-114">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="df694-115">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="df694-115">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="df694-116">Leia as propriedades e os relacionamentos de um objeto **chatMessageHostedContent** .</span><span class="sxs-lookup"><span data-stu-id="df694-116">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="df694-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df694-117">Properties</span></span>

| <span data-ttu-id="df694-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df694-118">Property</span></span>     | <span data-ttu-id="df694-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="df694-119">Type</span></span>        | <span data-ttu-id="df694-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="df694-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df694-121">id</span><span class="sxs-lookup"><span data-stu-id="df694-121">id</span></span>|<span data-ttu-id="df694-122">String</span><span class="sxs-lookup"><span data-stu-id="df694-122">String</span></span>| <span data-ttu-id="df694-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df694-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df694-124">Relações</span><span class="sxs-lookup"><span data-stu-id="df694-124">Relationships</span></span>

<span data-ttu-id="df694-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df694-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="df694-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df694-126">JSON representation</span></span>

<span data-ttu-id="df694-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df694-127">The following is a JSON representation of the resource.</span></span>

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
  "id": "String (identifier)"
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
