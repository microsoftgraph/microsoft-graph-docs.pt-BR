---
title: tipo de recurso chatMessageHostedContent
description: Um conteúdo hospedado em uma mensagem de chat
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a34e09b233a60858e23155f87808e40d080867f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507702"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="6f2b2-103">tipo de recurso chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="6f2b2-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="6f2b2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6f2b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f2b2-105">Representa o conteúdo hospedado em uma mensagem de chat, como imagens ou trechos de código.</span><span class="sxs-lookup"><span data-stu-id="6f2b2-105">Represents content hosted in a chat message, such as images or code snippets.</span></span>

## <a name="methods"></a><span data-ttu-id="6f2b2-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6f2b2-106">Methods</span></span>

| <span data-ttu-id="6f2b2-107">Método</span><span class="sxs-lookup"><span data-stu-id="6f2b2-107">Method</span></span>       | <span data-ttu-id="6f2b2-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6f2b2-108">Return Type</span></span> | <span data-ttu-id="6f2b2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f2b2-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6f2b2-110">Listar chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="6f2b2-110">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | [<span data-ttu-id="6f2b2-111">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="6f2b2-111">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="6f2b2-112">Recupere a lista de **chatMessageHostedContent** para uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="6f2b2-112">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="6f2b2-113">Obter chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="6f2b2-113">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="6f2b2-114">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="6f2b2-114">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="6f2b2-115">Leia as propriedades e os relacionamentos de um objeto **chatMessageHostedContent** .</span><span class="sxs-lookup"><span data-stu-id="6f2b2-115">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6f2b2-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f2b2-116">Properties</span></span>

| <span data-ttu-id="6f2b2-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f2b2-117">Property</span></span>     | <span data-ttu-id="6f2b2-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f2b2-118">Type</span></span>        | <span data-ttu-id="6f2b2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f2b2-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6f2b2-120">id</span><span class="sxs-lookup"><span data-stu-id="6f2b2-120">id</span></span>|<span data-ttu-id="6f2b2-121">String</span><span class="sxs-lookup"><span data-stu-id="6f2b2-121">String</span></span>| <span data-ttu-id="6f2b2-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f2b2-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f2b2-123">Relações</span><span class="sxs-lookup"><span data-stu-id="6f2b2-123">Relationships</span></span>

<span data-ttu-id="6f2b2-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6f2b2-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f2b2-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f2b2-125">JSON representation</span></span>

<span data-ttu-id="6f2b2-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f2b2-126">The following is a JSON representation of the resource.</span></span>

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
