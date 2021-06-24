---
title: Tipo de recurso serviceUpdateMessageViewpoint
description: Representa os dados de pontos de exibição do usuário para um serviceUpdateMessage."
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c84a07691c2507a9ff74102ac6f4b1675cb382e7
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109062"
---
# <a name="serviceupdatemessageviewpoint-resource-type"></a><span data-ttu-id="397c5-103">Tipo de recurso serviceUpdateMessageViewpoint</span><span class="sxs-lookup"><span data-stu-id="397c5-103">serviceUpdateMessageViewpoint resource type</span></span>

<span data-ttu-id="397c5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="397c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="397c5-105">Representa dados de pontos de exibição do usuário para [um serviceUpdateMessage](../resources/serviceupdatemessage.md).</span><span class="sxs-lookup"><span data-stu-id="397c5-105">Represents user view points data for a [serviceUpdateMessage](../resources/serviceupdatemessage.md).</span></span>

## <a name="properties"></a><span data-ttu-id="397c5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="397c5-106">Properties</span></span>
|<span data-ttu-id="397c5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="397c5-107">Property</span></span>|<span data-ttu-id="397c5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="397c5-108">Type</span></span>|<span data-ttu-id="397c5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="397c5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="397c5-110">isArchived</span><span class="sxs-lookup"><span data-stu-id="397c5-110">isArchived</span></span>|<span data-ttu-id="397c5-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="397c5-111">Boolean</span></span>|<span data-ttu-id="397c5-112">Indica se o usuário arquivou a mensagem.</span><span class="sxs-lookup"><span data-stu-id="397c5-112">Indicates whether the user archived the message.</span></span>|
|<span data-ttu-id="397c5-113">isFavorited</span><span class="sxs-lookup"><span data-stu-id="397c5-113">isFavorited</span></span>|<span data-ttu-id="397c5-114">Booleano</span><span class="sxs-lookup"><span data-stu-id="397c5-114">Boolean</span></span>|<span data-ttu-id="397c5-115">Indica se o usuário marcou a mensagem como favorita.</span><span class="sxs-lookup"><span data-stu-id="397c5-115">Indicates whether the user marked the message as favorite.</span></span>|
|<span data-ttu-id="397c5-116">isRead</span><span class="sxs-lookup"><span data-stu-id="397c5-116">isRead</span></span>|<span data-ttu-id="397c5-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="397c5-117">Boolean</span></span>|<span data-ttu-id="397c5-118">Indica se o usuário leu a mensagem.</span><span class="sxs-lookup"><span data-stu-id="397c5-118">Indicates whether the user read the message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="397c5-119">Relações</span><span class="sxs-lookup"><span data-stu-id="397c5-119">Relationships</span></span>
<span data-ttu-id="397c5-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="397c5-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="397c5-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="397c5-121">JSON representation</span></span>
<span data-ttu-id="397c5-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="397c5-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.serviceUpdateMessageViewpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceUpdateMessageViewpoint",
  "isRead": "Boolean",
  "isArchived": "Boolean",
  "isFavorited": "Boolean"
}
```