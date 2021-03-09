---
title: Tipo de recurso teamworkHostedContent
description: Representa conteúdo rich hospedado pelo Microsoft Teams
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 93b3b4fc817c1fe3aa3973a112b9cf887c825b6e
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578847"
---
# <a name="teamworkhostedcontent-resource-type"></a><span data-ttu-id="aa3ed-103">Tipo de recurso teamworkHostedContent</span><span class="sxs-lookup"><span data-stu-id="aa3ed-103">teamworkHostedContent resource type</span></span>

<span data-ttu-id="aa3ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa3ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa3ed-105">Representa conteúdo rico como imagens e trechos de código no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="aa3ed-105">Represents rich content like images and code snippets in Microsoft Teams.</span></span> <span data-ttu-id="aa3ed-106">Para conteúdo rico em [mensagens de canal e chat,](chatMessage.md)consulte [chatMessageHostedContent](chatMessageHostedContent.md).</span><span class="sxs-lookup"><span data-stu-id="aa3ed-106">For rich content in [channel and chat messages](chatMessage.md), see [chatMessageHostedContent](chatMessageHostedContent.md).</span></span>

## <a name="properties"></a><span data-ttu-id="aa3ed-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aa3ed-107">Properties</span></span>
|<span data-ttu-id="aa3ed-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa3ed-108">Property</span></span>|<span data-ttu-id="aa3ed-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa3ed-109">Type</span></span>|<span data-ttu-id="aa3ed-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa3ed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa3ed-111">contentBytes</span><span class="sxs-lookup"><span data-stu-id="aa3ed-111">contentBytes</span></span>|<span data-ttu-id="aa3ed-112">Binária</span><span class="sxs-lookup"><span data-stu-id="aa3ed-112">Binary</span></span>|<span data-ttu-id="aa3ed-113">Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="aa3ed-113">Write only.</span></span> <span data-ttu-id="aa3ed-114">Bytes para o conteúdo hospedado (como imagens).</span><span class="sxs-lookup"><span data-stu-id="aa3ed-114">Bytes for the hosted content (such as images).</span></span>|
|<span data-ttu-id="aa3ed-115">contentType</span><span class="sxs-lookup"><span data-stu-id="aa3ed-115">contentType</span></span>|<span data-ttu-id="aa3ed-116">String</span><span class="sxs-lookup"><span data-stu-id="aa3ed-116">String</span></span>|<span data-ttu-id="aa3ed-117">Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="aa3ed-117">Write only.</span></span> <span data-ttu-id="aa3ed-118">Tipo de conteúdo, como image/png, image/jpg.</span><span class="sxs-lookup"><span data-stu-id="aa3ed-118">Content type, such as image/png, image/jpg.</span></span>|
|<span data-ttu-id="aa3ed-119">id</span><span class="sxs-lookup"><span data-stu-id="aa3ed-119">id</span></span>|<span data-ttu-id="aa3ed-120">String</span><span class="sxs-lookup"><span data-stu-id="aa3ed-120">String</span></span>|<span data-ttu-id="aa3ed-121">ID do conteúdo hospedado.</span><span class="sxs-lookup"><span data-stu-id="aa3ed-121">ID of the hosted content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa3ed-122">Relações</span><span class="sxs-lookup"><span data-stu-id="aa3ed-122">Relationships</span></span>
<span data-ttu-id="aa3ed-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aa3ed-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa3ed-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aa3ed-124">JSON representation</span></span>
<span data-ttu-id="aa3ed-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aa3ed-125">The following is a JSON representation of the resource.</span></span>
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

