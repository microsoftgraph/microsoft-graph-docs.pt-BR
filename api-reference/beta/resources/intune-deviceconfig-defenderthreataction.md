---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fda734d6d582f8b838e0dca26ae57c118f3438b0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526829"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="a539f-103">tipo de enumeração defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="a539f-103">defenderThreatAction enum type</span></span>

<span data-ttu-id="a539f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a539f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a539f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a539f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a539f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a539f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a539f-107">Ação padrão do defender a ser executada em ameaças de malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="a539f-107">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="a539f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a539f-108">Members</span></span>
|<span data-ttu-id="a539f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a539f-109">Member</span></span>|<span data-ttu-id="a539f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a539f-110">Value</span></span>|<span data-ttu-id="a539f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a539f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a539f-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a539f-112">deviceDefault</span></span>|<span data-ttu-id="a539f-113">,0</span><span class="sxs-lookup"><span data-stu-id="a539f-113">0</span></span>|<span data-ttu-id="a539f-114">Aplicar ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="a539f-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="a539f-115">ordena</span><span class="sxs-lookup"><span data-stu-id="a539f-115">clean</span></span>|<span data-ttu-id="a539f-116">1 </span><span class="sxs-lookup"><span data-stu-id="a539f-116">1</span></span>|<span data-ttu-id="a539f-117">Limpe a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="a539f-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="a539f-118">quarentena</span><span class="sxs-lookup"><span data-stu-id="a539f-118">quarantine</span></span>|<span data-ttu-id="a539f-119">2 </span><span class="sxs-lookup"><span data-stu-id="a539f-119">2</span></span>|<span data-ttu-id="a539f-120">Colocar em quarentena a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="a539f-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="a539f-121">remover</span><span class="sxs-lookup"><span data-stu-id="a539f-121">remove</span></span>|<span data-ttu-id="a539f-122">3 </span><span class="sxs-lookup"><span data-stu-id="a539f-122">3</span></span>|<span data-ttu-id="a539f-123">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="a539f-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="a539f-124">permitiu</span><span class="sxs-lookup"><span data-stu-id="a539f-124">allow</span></span>|<span data-ttu-id="a539f-125">4 </span><span class="sxs-lookup"><span data-stu-id="a539f-125">4</span></span>|<span data-ttu-id="a539f-126">Permitir a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="a539f-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="a539f-127">UserDefined</span><span class="sxs-lookup"><span data-stu-id="a539f-127">userDefined</span></span>|<span data-ttu-id="a539f-128">5 </span><span class="sxs-lookup"><span data-stu-id="a539f-128">5</span></span>|<span data-ttu-id="a539f-129">Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="a539f-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="a539f-130">Larga</span><span class="sxs-lookup"><span data-stu-id="a539f-130">block</span></span>|<span data-ttu-id="a539f-131">6 </span><span class="sxs-lookup"><span data-stu-id="a539f-131">6</span></span>|<span data-ttu-id="a539f-132">Bloquear a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="a539f-132">Block the detected threat.</span></span>|



