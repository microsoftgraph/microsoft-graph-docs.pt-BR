---
title: tipo de recurso lobbyBypassSettings
description: Especifica quais participantes podem ignorar o lobby da reunião.
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3723f6593547b75c60a82b8436995c931d64e436
ms.sourcegitcommit: 7dcae492d8b4707d068adca3a74732e25a8198e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/10/2020
ms.locfileid: "47423678"
---
# <a name="lobbybypasssettings-resource-type"></a><span data-ttu-id="1c3b4-103">tipo de recurso lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="1c3b4-103">lobbyBypassSettings resource type</span></span>

<span data-ttu-id="1c3b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c3b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c3b4-105">Especifica quais participantes podem ignorar o lobby da reunião.</span><span class="sxs-lookup"><span data-stu-id="1c3b4-105">Specifies which participants can bypass the meeting lobby.</span></span>

## <a name="properties"></a><span data-ttu-id="1c3b4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1c3b4-106">Properties</span></span>

| <span data-ttu-id="1c3b4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c3b4-107">Property</span></span>              | <span data-ttu-id="1c3b4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c3b4-108">Type</span></span>    | <span data-ttu-id="1c3b4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c3b4-109">Description</span></span>                                                         | 
| --------------------- | ------- | ------------------------------------------------------------------- | 
| <span data-ttu-id="1c3b4-110">scope</span><span class="sxs-lookup"><span data-stu-id="1c3b4-110">scope</span></span>                 | <span data-ttu-id="1c3b4-111">lobbyBypassScope</span><span class="sxs-lookup"><span data-stu-id="1c3b4-111">lobbyBypassScope</span></span>  | <span data-ttu-id="1c3b4-112">Especifica o tipo de participantes que são automaticamente admitidos em uma reunião, ignorando o lobby.</span><span class="sxs-lookup"><span data-stu-id="1c3b4-112">Specifies the type of participants that are automatically admitted into a meeting, bypassing the lobby.</span></span> <span data-ttu-id="1c3b4-113">Os valores possíveis estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="1c3b4-113">Possible values are listed in the following table.</span></span> <span data-ttu-id="1c3b4-114">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1c3b4-114">Optional.</span></span>|
| <span data-ttu-id="1c3b4-115">isDialInBypassEnabled</span><span class="sxs-lookup"><span data-stu-id="1c3b4-115">isDialInBypassEnabled</span></span> | <span data-ttu-id="1c3b4-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c3b4-116">Boolean</span></span> | <span data-ttu-id="1c3b4-117">Especifica se você deseja ou não permitir que chamadores de discagem ignorem o lobby.</span><span class="sxs-lookup"><span data-stu-id="1c3b4-117">Specifies whether or not to always let dial-in callers bypass the lobby.</span></span> <span data-ttu-id="1c3b4-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1c3b4-118">Optional.</span></span> | 

### <a name="lobbybypassscope-values"></a><span data-ttu-id="1c3b4-119">valores de lobbyBypassScope</span><span class="sxs-lookup"><span data-stu-id="1c3b4-119">lobbyBypassScope values</span></span>

| <span data-ttu-id="1c3b4-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1c3b4-120">Value</span></span>                    | <span data-ttu-id="1c3b4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c3b4-121">Description</span></span>                                                                                                                                              |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1c3b4-122">organizer</span><span class="sxs-lookup"><span data-stu-id="1c3b4-122">organizer</span></span>                | <span data-ttu-id="1c3b4-123">Somente o organizador é admitido na reunião, ignorando o lobby.</span><span class="sxs-lookup"><span data-stu-id="1c3b4-123">Only the organizer is admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="1c3b4-124">Todos os outros participantes são colocados na sala de reunião.</span><span class="sxs-lookup"><span data-stu-id="1c3b4-124">All other participants are placed in the meeting lobby.</span></span>                                                                                                         |
| <span data-ttu-id="1c3b4-125">organization</span><span class="sxs-lookup"><span data-stu-id="1c3b4-125">organization</span></span>             | <span data-ttu-id="1c3b4-126">Somente os participantes da mesma empresa são admitidos na reunião, ignorando o lobby.</span><span class="sxs-lookup"><span data-stu-id="1c3b4-126">Only the participants from the same company are admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="1c3b4-127">Todos os outros participantes são colocados na sala de reunião.</span><span class="sxs-lookup"><span data-stu-id="1c3b4-127">All other participants are placed in the meeting lobby.</span></span>                                                                              |
| <span data-ttu-id="1c3b4-128">organizationAndFederated</span><span class="sxs-lookup"><span data-stu-id="1c3b4-128">organizationAndFederated</span></span> | <span data-ttu-id="1c3b4-129">Somente os participantes da mesma empresa ou organização confiável são admitidos na reunião, ignorando o lobby.</span><span class="sxs-lookup"><span data-stu-id="1c3b4-129">Only the participants from the same company or trusted organization are admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="1c3b4-130">Todos os outros participantes são colocados na sala de reunião.</span><span class="sxs-lookup"><span data-stu-id="1c3b4-130">All other participants are placed in the meeting lobby.</span></span> |
| <span data-ttu-id="1c3b4-131">têm</span><span class="sxs-lookup"><span data-stu-id="1c3b4-131">everyone</span></span>                 | <span data-ttu-id="1c3b4-132">Todos são admitidos na reunião.</span><span class="sxs-lookup"><span data-stu-id="1c3b4-132">Everyone is admitted into the meeting.</span></span> <span data-ttu-id="1c3b4-133">Nenhum participante é colocado na sala de reunião.</span><span class="sxs-lookup"><span data-stu-id="1c3b4-133">No participants are placed in the meeting lobby.</span></span>                                                                                                                   |
| <span data-ttu-id="1c3b4-134">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="1c3b4-134">unknownFutureValue</span></span>       | <span data-ttu-id="1c3b4-135">Valor de futuro desconhecido.</span><span class="sxs-lookup"><span data-stu-id="1c3b4-135">Unknow future value.</span></span>                                                                                                                                     |

## <a name="json-representation"></a><span data-ttu-id="1c3b4-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1c3b4-136">JSON representation</span></span>

<span data-ttu-id="1c3b4-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1c3b4-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.lobbyBypassSettings"
}-->
```json
{
  "scope": "organizer | organization | organizationAndFederated | everyone | unknownFutureValue",
  "isDialInBypassEnabled": "Boolean",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "lobbyBypassSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
