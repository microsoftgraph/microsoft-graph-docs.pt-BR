---
title: tipo de recurso onlineMeetingInfo
description: Detalhes de um participante para ingressar na reunião online.
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7ed8543be8b1d22c797d0033dcd0d41ba6308888
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939387"
---
# <a name="onlinemeetinginfo-resource-type"></a><span data-ttu-id="59cf1-103">tipo de recurso onlineMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="59cf1-103">onlineMeetingInfo resource type</span></span>

<span data-ttu-id="59cf1-104">Detalhes de um participante para ingressar na reunião online.</span><span class="sxs-lookup"><span data-stu-id="59cf1-104">Details for an attendee to join the meeting online.</span></span>

## <a name="properties"></a><span data-ttu-id="59cf1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="59cf1-105">Properties</span></span>

| <span data-ttu-id="59cf1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59cf1-106">Property</span></span>     | <span data-ttu-id="59cf1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="59cf1-107">Type</span></span>        | <span data-ttu-id="59cf1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="59cf1-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="59cf1-109">ID</span><span class="sxs-lookup"><span data-stu-id="59cf1-109">conferenceId</span></span>|<span data-ttu-id="59cf1-110">String</span><span class="sxs-lookup"><span data-stu-id="59cf1-110">String</span></span>| <span data-ttu-id="59cf1-111">A ID da conferência.</span><span class="sxs-lookup"><span data-stu-id="59cf1-111">The ID of the conference.</span></span>|
|<span data-ttu-id="59cf1-112">joinUrl</span><span class="sxs-lookup"><span data-stu-id="59cf1-112">joinUrl</span></span>|<span data-ttu-id="59cf1-113">String</span><span class="sxs-lookup"><span data-stu-id="59cf1-113">String</span></span>| <span data-ttu-id="59cf1-114">O link externo que inicia a reunião online.</span><span class="sxs-lookup"><span data-stu-id="59cf1-114">The external link that launches the online meeting.</span></span> <span data-ttu-id="59cf1-115">Esta é uma URL que os clientes serão inicializados em um navegador e redirecionará o usuário para participar da reunião.</span><span class="sxs-lookup"><span data-stu-id="59cf1-115">This is a URL that clients will launch into a browser and will redirect the user to join the meeting.</span></span>|
|<span data-ttu-id="59cf1-116">telefones</span><span class="sxs-lookup"><span data-stu-id="59cf1-116">phones</span></span>|<span data-ttu-id="59cf1-117">Coleção [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="59cf1-117">[phone](phone.md) collection</span></span>| <span data-ttu-id="59cf1-118">Todos os números de telefone associados a esta conferência.</span><span class="sxs-lookup"><span data-stu-id="59cf1-118">All of the phone numbers associated with this conference.</span></span>|
|<span data-ttu-id="59cf1-119">quickDial</span><span class="sxs-lookup"><span data-stu-id="59cf1-119">quickDial</span></span>|<span data-ttu-id="59cf1-120">String</span><span class="sxs-lookup"><span data-stu-id="59cf1-120">String</span></span>| <span data-ttu-id="59cf1-121">O Quickdial pré-formatado para esta chamada.</span><span class="sxs-lookup"><span data-stu-id="59cf1-121">The pre-formatted quickdial for this call.</span></span>|
|<span data-ttu-id="59cf1-122">tollFreeNumbers</span><span class="sxs-lookup"><span data-stu-id="59cf1-122">tollFreeNumbers</span></span>|<span data-ttu-id="59cf1-123">String collection</span><span class="sxs-lookup"><span data-stu-id="59cf1-123">String collection</span></span>| <span data-ttu-id="59cf1-124">Os números de chamada gratuita que podem ser usados para ingressar na conferência.</span><span class="sxs-lookup"><span data-stu-id="59cf1-124">The toll free numbers that can be used to join the conference.</span></span>|
|<span data-ttu-id="59cf1-125">tollNumber</span><span class="sxs-lookup"><span data-stu-id="59cf1-125">tollNumber</span></span>|<span data-ttu-id="59cf1-126">String</span><span class="sxs-lookup"><span data-stu-id="59cf1-126">String</span></span>| <span data-ttu-id="59cf1-127">O número de chamada tarifada que pode ser usado para ingressar na conferência.</span><span class="sxs-lookup"><span data-stu-id="59cf1-127">The toll number that can be used to join the conference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="59cf1-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="59cf1-128">JSON representation</span></span>

<span data-ttu-id="59cf1-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="59cf1-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onlineMeetingInfo"
}-->

```json
{
  "conferenceId": "String",
  "joinUrl": "String",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "quickDial": "String",
  "tollFreeNumbers": ["String"],
  "tollNumber": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->s
