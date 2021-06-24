---
title: Tipo de recurso serviceHealthIssuePost
description: Representa uma postagem histórica em um problema de saúde do serviço.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 910236d2059f951169bea314a0b38ae2516b1918
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107768"
---
# <a name="servicehealthissuepost-resource-type"></a><span data-ttu-id="f87eb-103">Tipo de recurso serviceHealthIssuePost</span><span class="sxs-lookup"><span data-stu-id="f87eb-103">serviceHealthIssuePost resource type</span></span>

<span data-ttu-id="f87eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f87eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f87eb-105">Representa uma postagem histórica em um [problema de saúde do serviço.](../resources/servicehealthissue.md)</span><span class="sxs-lookup"><span data-stu-id="f87eb-105">Represents a historical post in a [service health issue](../resources/servicehealthissue.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f87eb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f87eb-106">Properties</span></span>
|<span data-ttu-id="f87eb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f87eb-107">Property</span></span>|<span data-ttu-id="f87eb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f87eb-108">Type</span></span>|<span data-ttu-id="f87eb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f87eb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f87eb-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f87eb-110">createdDateTime</span></span>|<span data-ttu-id="f87eb-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f87eb-111">DateTimeOffset</span></span>|<span data-ttu-id="f87eb-112">O horário publicado da postagem.</span><span class="sxs-lookup"><span data-stu-id="f87eb-112">The published time of the post.</span></span>|
|<span data-ttu-id="f87eb-113">description</span><span class="sxs-lookup"><span data-stu-id="f87eb-113">description</span></span>|[<span data-ttu-id="f87eb-114">itemBody</span><span class="sxs-lookup"><span data-stu-id="f87eb-114">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="f87eb-115">O conteúdo da postagem de problema do serviço.</span><span class="sxs-lookup"><span data-stu-id="f87eb-115">The content of the service issue post.</span></span>|
|<span data-ttu-id="f87eb-116">postType</span><span class="sxs-lookup"><span data-stu-id="f87eb-116">postType</span></span>|<span data-ttu-id="f87eb-117">postType</span><span class="sxs-lookup"><span data-stu-id="f87eb-117">postType</span></span>|<span data-ttu-id="f87eb-118">O tipo de postagem da postagem histórica do problema do serviço.</span><span class="sxs-lookup"><span data-stu-id="f87eb-118">The post type of the service issue historical post.</span></span> <span data-ttu-id="f87eb-119">Os valores possíveis são: `regular`, `quick`, `strategic`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f87eb-119">Possible values are: `regular`, `quick`, `strategic`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f87eb-120">Relações</span><span class="sxs-lookup"><span data-stu-id="f87eb-120">Relationships</span></span>
<span data-ttu-id="f87eb-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f87eb-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f87eb-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f87eb-122">JSON representation</span></span>
<span data-ttu-id="f87eb-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f87eb-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.serviceHealthIssuePost"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealthIssuePost",
  "createdDateTime": "String (timestamp)",
  "postType": "String",
  "description": {
    "@odata.type": "microsoft.graph.itemBody"
  }
}
```

