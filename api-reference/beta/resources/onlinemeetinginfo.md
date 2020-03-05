---
title: tipo de recurso onlineMeetingInfo
description: Detalhes para o participante entrar na reunião online.
localization_priority: Normal
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8ac6c42f28ed1f2adccd54fcd3bd6667f4113b7a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522246"
---
# <a name="onlinemeetinginfo-resource-type"></a><span data-ttu-id="6b996-103">tipo de recurso onlineMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="6b996-103">onlineMeetingInfo resource type</span></span>

<span data-ttu-id="6b996-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6b996-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b996-105">Detalhes para o participante entrar na reunião online.</span><span class="sxs-lookup"><span data-stu-id="6b996-105">Details for an attendee to join the meeting online.</span></span>

## <a name="properties"></a><span data-ttu-id="6b996-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b996-106">Properties</span></span>

| <span data-ttu-id="6b996-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b996-107">Property</span></span>     | <span data-ttu-id="6b996-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b996-108">Type</span></span>        | <span data-ttu-id="6b996-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b996-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6b996-110">ID</span><span class="sxs-lookup"><span data-stu-id="6b996-110">conferenceId</span></span>|<span data-ttu-id="6b996-111">String</span><span class="sxs-lookup"><span data-stu-id="6b996-111">String</span></span>| <span data-ttu-id="6b996-112">A ID da conferência.</span><span class="sxs-lookup"><span data-stu-id="6b996-112">The ID of the conference.</span></span>|
|<span data-ttu-id="6b996-113">joinUrl</span><span class="sxs-lookup"><span data-stu-id="6b996-113">joinUrl</span></span>|<span data-ttu-id="6b996-114">String</span><span class="sxs-lookup"><span data-stu-id="6b996-114">String</span></span>| <span data-ttu-id="6b996-115">O link externo que inicia a reunião online.</span><span class="sxs-lookup"><span data-stu-id="6b996-115">The external link that launches the online meeting.</span></span> <span data-ttu-id="6b996-116">Esta é uma URL que os clientes serão inicializados em um navegador e redirecionará o usuário para participar da reunião.</span><span class="sxs-lookup"><span data-stu-id="6b996-116">This is a URL that clients will launch into a browser and will redirect the user to join the meeting.</span></span>|
|<span data-ttu-id="6b996-117">telefones</span><span class="sxs-lookup"><span data-stu-id="6b996-117">phones</span></span>|<span data-ttu-id="6b996-118">Coleção [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="6b996-118">[phone](phone.md) collection</span></span>| <span data-ttu-id="6b996-119">Todos os números de telefone associados a esta conferência.</span><span class="sxs-lookup"><span data-stu-id="6b996-119">All of the phone numbers associated with this conference.</span></span>|
|<span data-ttu-id="6b996-120">quickDial</span><span class="sxs-lookup"><span data-stu-id="6b996-120">quickDial</span></span>|<span data-ttu-id="6b996-121">String</span><span class="sxs-lookup"><span data-stu-id="6b996-121">String</span></span>| <span data-ttu-id="6b996-122">O Quickdial pré-formatado para esta chamada.</span><span class="sxs-lookup"><span data-stu-id="6b996-122">The pre-formatted quickdial for this call.</span></span>|
|<span data-ttu-id="6b996-123">tollFreeNumbers</span><span class="sxs-lookup"><span data-stu-id="6b996-123">tollFreeNumbers</span></span>|<span data-ttu-id="6b996-124">String collection</span><span class="sxs-lookup"><span data-stu-id="6b996-124">String collection</span></span>| <span data-ttu-id="6b996-125">Os números de chamada gratuita que podem ser usados para ingressar na conferência.</span><span class="sxs-lookup"><span data-stu-id="6b996-125">The toll free numbers that can be used to join the conference.</span></span>|
|<span data-ttu-id="6b996-126">tollNumber</span><span class="sxs-lookup"><span data-stu-id="6b996-126">tollNumber</span></span>|<span data-ttu-id="6b996-127">String</span><span class="sxs-lookup"><span data-stu-id="6b996-127">String</span></span>| <span data-ttu-id="6b996-128">O número de chamada tarifada que pode ser usado para ingressar na conferência.</span><span class="sxs-lookup"><span data-stu-id="6b996-128">The toll number that can be used to join the conference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b996-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b996-129">JSON representation</span></span>

<span data-ttu-id="6b996-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b996-130">The following is a JSON representation of the resource.</span></span>

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
