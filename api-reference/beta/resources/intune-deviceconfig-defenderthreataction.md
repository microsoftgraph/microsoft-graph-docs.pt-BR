---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 215b243a6e63ee44163a4127cd3724b37995cdb6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979736"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="33294-103">tipo de enumeração defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="33294-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="33294-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="33294-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33294-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="33294-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33294-106">Ação padrão do defender a ser executada em ameaças de malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="33294-106">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="33294-107">Membros</span><span class="sxs-lookup"><span data-stu-id="33294-107">Members</span></span>
|<span data-ttu-id="33294-108">Membro</span><span class="sxs-lookup"><span data-stu-id="33294-108">Member</span></span>|<span data-ttu-id="33294-109">Valor</span><span class="sxs-lookup"><span data-stu-id="33294-109">Value</span></span>|<span data-ttu-id="33294-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="33294-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33294-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="33294-111">deviceDefault</span></span>|<span data-ttu-id="33294-112">,0</span><span class="sxs-lookup"><span data-stu-id="33294-112">0</span></span>|<span data-ttu-id="33294-113">Aplicar ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="33294-113">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="33294-114">ordena</span><span class="sxs-lookup"><span data-stu-id="33294-114">clean</span></span>|<span data-ttu-id="33294-115">1</span><span class="sxs-lookup"><span data-stu-id="33294-115">1</span></span>|<span data-ttu-id="33294-116">Limpe a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="33294-116">Clean the detected threat.</span></span>|
|<span data-ttu-id="33294-117">quarentena</span><span class="sxs-lookup"><span data-stu-id="33294-117">quarantine</span></span>|<span data-ttu-id="33294-118">duas</span><span class="sxs-lookup"><span data-stu-id="33294-118">2</span></span>|<span data-ttu-id="33294-119">Colocar em quarentena a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="33294-119">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="33294-120">remover</span><span class="sxs-lookup"><span data-stu-id="33294-120">remove</span></span>|<span data-ttu-id="33294-121">3D</span><span class="sxs-lookup"><span data-stu-id="33294-121">3</span></span>|<span data-ttu-id="33294-122">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="33294-122">Remove the detected threat.</span></span>|
|<span data-ttu-id="33294-123">permitiu</span><span class="sxs-lookup"><span data-stu-id="33294-123">allow</span></span>|<span data-ttu-id="33294-124">quatro</span><span class="sxs-lookup"><span data-stu-id="33294-124">4</span></span>|<span data-ttu-id="33294-125">Permitir a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="33294-125">Allow the detected threat.</span></span>|
|<span data-ttu-id="33294-126">UserDefined</span><span class="sxs-lookup"><span data-stu-id="33294-126">userDefined</span></span>|<span data-ttu-id="33294-127">0,5</span><span class="sxs-lookup"><span data-stu-id="33294-127">5</span></span>|<span data-ttu-id="33294-128">Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="33294-128">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="33294-129">Larga</span><span class="sxs-lookup"><span data-stu-id="33294-129">block</span></span>|<span data-ttu-id="33294-130">6</span><span class="sxs-lookup"><span data-stu-id="33294-130">6</span></span>|<span data-ttu-id="33294-131">Bloquear a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="33294-131">Block the detected threat.</span></span>|





