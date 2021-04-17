---
title: Tipo de recurso teamworkHostedContent
description: Representa conteúdo rich hospedado pelo Microsoft Teams
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: da0b157bab78867bd3309b4529afe8ef734f0144
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882310"
---
# <a name="teamworkhostedcontent-resource-type"></a><span data-ttu-id="54b9b-103">Tipo de recurso teamworkHostedContent</span><span class="sxs-lookup"><span data-stu-id="54b9b-103">teamworkHostedContent resource type</span></span>

<span data-ttu-id="54b9b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54b9b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54b9b-105">Representa conteúdo rico como imagens e trechos de código no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="54b9b-105">Represents rich content like images and code snippets in Microsoft Teams.</span></span> <span data-ttu-id="54b9b-106">Para conteúdo rico em [mensagens de canal e chat,](chatMessage.md)consulte [chatMessageHostedContent](chatMessageHostedContent.md).</span><span class="sxs-lookup"><span data-stu-id="54b9b-106">For rich content in [channel and chat messages](chatMessage.md), see [chatMessageHostedContent](chatMessageHostedContent.md).</span></span>

## <a name="methods"></a><span data-ttu-id="54b9b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="54b9b-107">Methods</span></span>

| <span data-ttu-id="54b9b-108">Método</span><span class="sxs-lookup"><span data-stu-id="54b9b-108">Method</span></span>                                            | <span data-ttu-id="54b9b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="54b9b-109">Return Type</span></span>                                       | <span data-ttu-id="54b9b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="54b9b-110">Description</span></span>                                                    | 
| :------------------------------------------------ | :------------------------------------------------ | :------------------------------------------------------------- |
| [<span data-ttu-id="54b9b-111">Obter bytes de ícone de aplicativo</span><span class="sxs-lookup"><span data-stu-id="54b9b-111">Get app icon bytes</span></span>](../api/teamsappicon-get.md)     | [<span data-ttu-id="54b9b-112">teamworkHostedContent</span><span class="sxs-lookup"><span data-stu-id="54b9b-112">teamworkHostedContent</span></span>](teamworkhostedcontent.md)                   | <span data-ttu-id="54b9b-113">Obter os bytes do conteúdo hospedado com o backing de um ícone de aplicativo do Teams.</span><span class="sxs-lookup"><span data-stu-id="54b9b-113">Get the bytes of the hosted content backing a Teams app icon.</span></span> |

## <a name="properties"></a><span data-ttu-id="54b9b-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54b9b-114">Properties</span></span>
|<span data-ttu-id="54b9b-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54b9b-115">Property</span></span>|<span data-ttu-id="54b9b-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="54b9b-116">Type</span></span>|<span data-ttu-id="54b9b-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="54b9b-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54b9b-118">contentBytes</span><span class="sxs-lookup"><span data-stu-id="54b9b-118">contentBytes</span></span>|<span data-ttu-id="54b9b-119">Binária</span><span class="sxs-lookup"><span data-stu-id="54b9b-119">Binary</span></span>|<span data-ttu-id="54b9b-120">Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="54b9b-120">Write only.</span></span> <span data-ttu-id="54b9b-121">Bytes para o conteúdo hospedado (como imagens).</span><span class="sxs-lookup"><span data-stu-id="54b9b-121">Bytes for the hosted content (such as images).</span></span>|
|<span data-ttu-id="54b9b-122">contentType</span><span class="sxs-lookup"><span data-stu-id="54b9b-122">contentType</span></span>|<span data-ttu-id="54b9b-123">String</span><span class="sxs-lookup"><span data-stu-id="54b9b-123">String</span></span>|<span data-ttu-id="54b9b-124">Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="54b9b-124">Write only.</span></span> <span data-ttu-id="54b9b-125">Tipo de conteúdo, como image/png, image/jpg.</span><span class="sxs-lookup"><span data-stu-id="54b9b-125">Content type, such as image/png, image/jpg.</span></span>|
|<span data-ttu-id="54b9b-126">id</span><span class="sxs-lookup"><span data-stu-id="54b9b-126">id</span></span>|<span data-ttu-id="54b9b-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54b9b-127">String</span></span>|<span data-ttu-id="54b9b-128">ID do conteúdo hospedado.</span><span class="sxs-lookup"><span data-stu-id="54b9b-128">ID of the hosted content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54b9b-129">Relações</span><span class="sxs-lookup"><span data-stu-id="54b9b-129">Relationships</span></span>
<span data-ttu-id="54b9b-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="54b9b-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="54b9b-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54b9b-131">JSON representation</span></span>
<span data-ttu-id="54b9b-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="54b9b-132">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkHostedContent",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkHostedContent",
  "id": "String (identifier)",
  "contentBytes": "Binary",
  "contentType": "String"
}
```

