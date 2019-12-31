---
title: tipo de recurso onlineMeetingInfo
description: Detalhes para o participante entrar na reunião online.
localization_priority: Normal
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 52bfe4fd46443c826838153cc2a40ea57712182b
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913153"
---
# <a name="onlinemeetinginfo-resource-type"></a><span data-ttu-id="7a57b-103">tipo de recurso onlineMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="7a57b-103">onlineMeetingInfo resource type</span></span>

<span data-ttu-id="7a57b-104">Detalhes para o participante entrar na reunião online.</span><span class="sxs-lookup"><span data-stu-id="7a57b-104">Details for an attendee to join the meeting online.</span></span>

## <a name="properties"></a><span data-ttu-id="7a57b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a57b-105">Properties</span></span>

| <span data-ttu-id="7a57b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a57b-106">Property</span></span>     | <span data-ttu-id="7a57b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a57b-107">Type</span></span>        | <span data-ttu-id="7a57b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a57b-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7a57b-109">ID</span><span class="sxs-lookup"><span data-stu-id="7a57b-109">conferenceId</span></span>|<span data-ttu-id="7a57b-110">String</span><span class="sxs-lookup"><span data-stu-id="7a57b-110">String</span></span>| <span data-ttu-id="7a57b-111">A ID da conferência.</span><span class="sxs-lookup"><span data-stu-id="7a57b-111">The ID of the conference.</span></span>|
|<span data-ttu-id="7a57b-112">joinUrl</span><span class="sxs-lookup"><span data-stu-id="7a57b-112">joinUrl</span></span>|<span data-ttu-id="7a57b-113">String</span><span class="sxs-lookup"><span data-stu-id="7a57b-113">String</span></span>| <span data-ttu-id="7a57b-114">O link externo que inicia a reunião online.</span><span class="sxs-lookup"><span data-stu-id="7a57b-114">The external link that launches the online meeting.</span></span> <span data-ttu-id="7a57b-115">Esta é uma URL que os clientes serão inicializados em um navegador e redirecionará o usuário para participar da reunião.</span><span class="sxs-lookup"><span data-stu-id="7a57b-115">This is a URL that clients will launch into a browser and will redirect the user to join the meeting.</span></span>|
|<span data-ttu-id="7a57b-116">telefones</span><span class="sxs-lookup"><span data-stu-id="7a57b-116">phones</span></span>|<span data-ttu-id="7a57b-117">Coleção [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="7a57b-117">[phone](phone.md) collection</span></span>| <span data-ttu-id="7a57b-118">Todos os números de telefone associados a esta conferência.</span><span class="sxs-lookup"><span data-stu-id="7a57b-118">All of the phone numbers associated with this conference.</span></span>|
|<span data-ttu-id="7a57b-119">quickDial</span><span class="sxs-lookup"><span data-stu-id="7a57b-119">quickDial</span></span>|<span data-ttu-id="7a57b-120">String</span><span class="sxs-lookup"><span data-stu-id="7a57b-120">String</span></span>| <span data-ttu-id="7a57b-121">O Quickdial pré-formatado para esta chamada.</span><span class="sxs-lookup"><span data-stu-id="7a57b-121">The pre-formatted quickdial for this call.</span></span>|
|<span data-ttu-id="7a57b-122">tollFreeNumbers</span><span class="sxs-lookup"><span data-stu-id="7a57b-122">tollFreeNumbers</span></span>|<span data-ttu-id="7a57b-123">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a57b-123">String collection</span></span>| <span data-ttu-id="7a57b-124">Os números de chamada gratuita que podem ser usados para ingressar na conferência.</span><span class="sxs-lookup"><span data-stu-id="7a57b-124">The toll free numbers that can be used to join the conference.</span></span>|
|<span data-ttu-id="7a57b-125">tollNumber</span><span class="sxs-lookup"><span data-stu-id="7a57b-125">tollNumber</span></span>|<span data-ttu-id="7a57b-126">String</span><span class="sxs-lookup"><span data-stu-id="7a57b-126">String</span></span>| <span data-ttu-id="7a57b-127">O número de chamada tarifada que pode ser usado para ingressar na conferência.</span><span class="sxs-lookup"><span data-stu-id="7a57b-127">The toll number that can be used to join the conference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a57b-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a57b-128">JSON representation</span></span>

<span data-ttu-id="7a57b-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a57b-129">The following is a JSON representation of the resource.</span></span>

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
