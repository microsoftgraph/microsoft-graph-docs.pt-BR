---
title: Tipo de recurso lobbyBypassSettings
description: Especifica quais participantes podem ignorar o lobby da reunião.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c6d530765e1bc356486f0b8893c69c445c07181f
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896680"
---
# <a name="lobbybypasssettings-resource-type"></a><span data-ttu-id="c54a9-103">Tipo de recurso lobbyBypassSettings</span><span class="sxs-lookup"><span data-stu-id="c54a9-103">lobbyBypassSettings resource type</span></span>

<span data-ttu-id="c54a9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c54a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c54a9-105">Especifica quais participantes podem ignorar o lobby da reunião.</span><span class="sxs-lookup"><span data-stu-id="c54a9-105">Specifies which participants can bypass the meeting lobby.</span></span>

## <a name="properties"></a><span data-ttu-id="c54a9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c54a9-106">Properties</span></span>

| <span data-ttu-id="c54a9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c54a9-107">Property</span></span>              | <span data-ttu-id="c54a9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c54a9-108">Type</span></span>    | <span data-ttu-id="c54a9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c54a9-109">Description</span></span>                                                         | 
| --------------------- | ------- | ------------------------------------------------------------------- | 
| <span data-ttu-id="c54a9-110">scope</span><span class="sxs-lookup"><span data-stu-id="c54a9-110">scope</span></span>                 | [<span data-ttu-id="c54a9-111">lobbyBypassScope</span><span class="sxs-lookup"><span data-stu-id="c54a9-111">lobbyBypassScope</span></span>](#lobbybypassscope-values)  | <span data-ttu-id="c54a9-112">Especifica o tipo de participantes que são automaticamente admitidos em uma reunião, ignorando o lobby.</span><span class="sxs-lookup"><span data-stu-id="c54a9-112">Specifies the type of participants that are automatically admitted into a meeting, bypassing the lobby.</span></span> <span data-ttu-id="c54a9-113">Os valores possíveis são listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="c54a9-113">Possible values are listed in the following table.</span></span> <span data-ttu-id="c54a9-114">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c54a9-114">Optional.</span></span>|
| <span data-ttu-id="c54a9-115">isDialInBypassEnabled</span><span class="sxs-lookup"><span data-stu-id="c54a9-115">isDialInBypassEnabled</span></span> | <span data-ttu-id="c54a9-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="c54a9-116">Boolean</span></span> | <span data-ttu-id="c54a9-117">Especifica se os chamadores de discagem sempre podem ou não ignorar o lobby.</span><span class="sxs-lookup"><span data-stu-id="c54a9-117">Specifies whether or not to always let dial-in callers bypass the lobby.</span></span> <span data-ttu-id="c54a9-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c54a9-118">Optional.</span></span> | 

### <a name="lobbybypassscope-values"></a><span data-ttu-id="c54a9-119">valores lobbyBypassScope</span><span class="sxs-lookup"><span data-stu-id="c54a9-119">lobbyBypassScope values</span></span>

| <span data-ttu-id="c54a9-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c54a9-120">Value</span></span>                    | <span data-ttu-id="c54a9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c54a9-121">Description</span></span>                                                                                                                                              |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c54a9-122">organizer</span><span class="sxs-lookup"><span data-stu-id="c54a9-122">organizer</span></span>                | <span data-ttu-id="c54a9-123">Somente o organizador é admitido na reunião, ignorando o lobby.</span><span class="sxs-lookup"><span data-stu-id="c54a9-123">Only the organizer is admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="c54a9-124">Todos os outros participantes são colocados no lobby da reunião.</span><span class="sxs-lookup"><span data-stu-id="c54a9-124">All other participants are placed in the meeting lobby.</span></span>                                                                                                         |
| <span data-ttu-id="c54a9-125">organization</span><span class="sxs-lookup"><span data-stu-id="c54a9-125">organization</span></span>             | <span data-ttu-id="c54a9-126">Somente os participantes da mesma empresa são admitidos na reunião, ignorando o lobby.</span><span class="sxs-lookup"><span data-stu-id="c54a9-126">Only the participants from the same company are admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="c54a9-127">Todos os outros participantes são colocados no lobby da reunião.</span><span class="sxs-lookup"><span data-stu-id="c54a9-127">All other participants are placed in the meeting lobby.</span></span>                                                                              |
| <span data-ttu-id="c54a9-128">organizationAndFederated</span><span class="sxs-lookup"><span data-stu-id="c54a9-128">organizationAndFederated</span></span> | <span data-ttu-id="c54a9-129">Somente os participantes da mesma empresa ou organização confiável são admitidos na reunião, ignorando o lobby.</span><span class="sxs-lookup"><span data-stu-id="c54a9-129">Only the participants from the same company or trusted organization are admitted into the meeting, bypassing the lobby.</span></span> <span data-ttu-id="c54a9-130">Todos os outros participantes são colocados no lobby da reunião.</span><span class="sxs-lookup"><span data-stu-id="c54a9-130">All other participants are placed in the meeting lobby.</span></span> |
| <span data-ttu-id="c54a9-131">everyone</span><span class="sxs-lookup"><span data-stu-id="c54a9-131">everyone</span></span>                 | <span data-ttu-id="c54a9-132">Todos são admitidos na reunião.</span><span class="sxs-lookup"><span data-stu-id="c54a9-132">Everyone is admitted into the meeting.</span></span> <span data-ttu-id="c54a9-133">Nenhum participante é colocado no lobby da reunião.</span><span class="sxs-lookup"><span data-stu-id="c54a9-133">No participants are placed in the meeting lobby.</span></span>                                                                                                                   |
| <span data-ttu-id="c54a9-134">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="c54a9-134">unknownFutureValue</span></span>       | <span data-ttu-id="c54a9-135">Valor futuro desconhecido.</span><span class="sxs-lookup"><span data-stu-id="c54a9-135">Unknow future value.</span></span>                                                                                                                                     |

## <a name="json-representation"></a><span data-ttu-id="c54a9-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c54a9-136">JSON representation</span></span>

<span data-ttu-id="c54a9-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c54a9-137">The following is a JSON representation of the resource.</span></span>

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
