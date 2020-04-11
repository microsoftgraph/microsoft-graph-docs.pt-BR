---
title: tipo de recurso onlineMeetingInfo
description: Detalhes para o participante entrar na reunião online.
localization_priority: Normal
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 063f2f43f98d9f2d75822f712c4e17755bc290f7
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229448"
---
# <a name="onlinemeetinginfo-resource-type"></a><span data-ttu-id="3a737-103">tipo de recurso onlineMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="3a737-103">onlineMeetingInfo resource type</span></span>

<span data-ttu-id="3a737-104">Detalhes para o participante entrar na reunião online.</span><span class="sxs-lookup"><span data-stu-id="3a737-104">Details for an attendee to join the meeting online.</span></span>

## <a name="properties"></a><span data-ttu-id="3a737-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a737-105">Properties</span></span>

| <span data-ttu-id="3a737-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a737-106">Property</span></span>     | <span data-ttu-id="3a737-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a737-107">Type</span></span>        | <span data-ttu-id="3a737-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a737-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3a737-109">ID</span><span class="sxs-lookup"><span data-stu-id="3a737-109">conferenceId</span></span>|<span data-ttu-id="3a737-110">String</span><span class="sxs-lookup"><span data-stu-id="3a737-110">String</span></span>| <span data-ttu-id="3a737-111">A ID da conferência.</span><span class="sxs-lookup"><span data-stu-id="3a737-111">The ID of the conference.</span></span>|
|<span data-ttu-id="3a737-112">joinUrl</span><span class="sxs-lookup"><span data-stu-id="3a737-112">joinUrl</span></span>|<span data-ttu-id="3a737-113">String</span><span class="sxs-lookup"><span data-stu-id="3a737-113">String</span></span>| <span data-ttu-id="3a737-114">O link externo que inicia a reunião online.</span><span class="sxs-lookup"><span data-stu-id="3a737-114">The external link that launches the online meeting.</span></span> <span data-ttu-id="3a737-115">Esta é uma URL que os clientes serão inicializados em um navegador e redirecionará o usuário para participar da reunião.</span><span class="sxs-lookup"><span data-stu-id="3a737-115">This is a URL that clients will launch into a browser and will redirect the user to join the meeting.</span></span>|
|<span data-ttu-id="3a737-116">telefones</span><span class="sxs-lookup"><span data-stu-id="3a737-116">phones</span></span>|<span data-ttu-id="3a737-117">Coleção [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="3a737-117">[phone](phone.md) collection</span></span>| <span data-ttu-id="3a737-118">Todos os números de telefone associados a esta conferência.</span><span class="sxs-lookup"><span data-stu-id="3a737-118">All of the phone numbers associated with this conference.</span></span>|
|<span data-ttu-id="3a737-119">quickDial</span><span class="sxs-lookup"><span data-stu-id="3a737-119">quickDial</span></span>|<span data-ttu-id="3a737-120">String</span><span class="sxs-lookup"><span data-stu-id="3a737-120">String</span></span>| <span data-ttu-id="3a737-121">O Quickdial pré-formatado para esta chamada.</span><span class="sxs-lookup"><span data-stu-id="3a737-121">The pre-formatted quickdial for this call.</span></span>|
|<span data-ttu-id="3a737-122">tollFreeNumbers</span><span class="sxs-lookup"><span data-stu-id="3a737-122">tollFreeNumbers</span></span>|<span data-ttu-id="3a737-123">String collection</span><span class="sxs-lookup"><span data-stu-id="3a737-123">String collection</span></span>| <span data-ttu-id="3a737-124">Os números de chamada gratuita que podem ser usados para ingressar na conferência.</span><span class="sxs-lookup"><span data-stu-id="3a737-124">The toll free numbers that can be used to join the conference.</span></span>|
|<span data-ttu-id="3a737-125">tollNumber</span><span class="sxs-lookup"><span data-stu-id="3a737-125">tollNumber</span></span>|<span data-ttu-id="3a737-126">String</span><span class="sxs-lookup"><span data-stu-id="3a737-126">String</span></span>| <span data-ttu-id="3a737-127">O número de chamada tarifada que pode ser usado para ingressar na conferência.</span><span class="sxs-lookup"><span data-stu-id="3a737-127">The toll number that can be used to join the conference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3a737-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a737-128">JSON representation</span></span>

<span data-ttu-id="3a737-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a737-129">The following is a JSON representation of the resource.</span></span>

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
}-->
