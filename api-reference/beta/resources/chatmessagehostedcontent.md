---
title: tipo de recurso chatMessageHostedContent
description: Um conteúdo hospedado em uma mensagem de chat
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 39939d9d61d992e5fd77fd21360ab05e8f83dbd4
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333357"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="b3625-103">tipo de recurso chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="b3625-103">chatMessageHostedContent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3625-104">Representa o conteúdo hospedado em uma mensagem de chat, como imagens ou trechos de código.</span><span class="sxs-lookup"><span data-stu-id="b3625-104">Represents content hosted in a chat message, such as images or code snippets.</span></span>

## <a name="methods"></a><span data-ttu-id="b3625-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="b3625-105">Methods</span></span>

| <span data-ttu-id="b3625-106">Método</span><span class="sxs-lookup"><span data-stu-id="b3625-106">Method</span></span>       | <span data-ttu-id="b3625-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b3625-107">Return Type</span></span> | <span data-ttu-id="b3625-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3625-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b3625-109">Listar chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="b3625-109">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | [<span data-ttu-id="b3625-110">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="b3625-110">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="b3625-111">Recupere a lista de **chatMessageHostedContent** para uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="b3625-111">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="b3625-112">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="b3625-112">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="b3625-113">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="b3625-113">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="b3625-114">Leia as propriedades e os relacionamentos de um objeto **chatMessageHostedContent** .</span><span class="sxs-lookup"><span data-stu-id="b3625-114">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b3625-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3625-115">Properties</span></span>

| <span data-ttu-id="b3625-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3625-116">Property</span></span>     | <span data-ttu-id="b3625-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3625-117">Type</span></span>        | <span data-ttu-id="b3625-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3625-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b3625-119">id</span><span class="sxs-lookup"><span data-stu-id="b3625-119">id</span></span>|<span data-ttu-id="b3625-120">String</span><span class="sxs-lookup"><span data-stu-id="b3625-120">String</span></span>| <span data-ttu-id="b3625-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3625-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3625-122">Relações</span><span class="sxs-lookup"><span data-stu-id="b3625-122">Relationships</span></span>

<span data-ttu-id="b3625-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b3625-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3625-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3625-124">JSON representation</span></span>

<span data-ttu-id="b3625-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3625-125">The following is a JSON representation of the resource.</span></span>

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
