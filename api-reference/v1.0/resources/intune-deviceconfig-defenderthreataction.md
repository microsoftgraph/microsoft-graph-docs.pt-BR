---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 71533fa6d01c9c51980881429b4dc3e443f9c766
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359674"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="10819-103">tipo de enumeração defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="10819-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="10819-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10819-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10819-105">Ação padrão do defender a ser executada em ameaças de malware detectadas.</span><span class="sxs-lookup"><span data-stu-id="10819-105">Defender’s default action to take on detected Malware threats.</span></span>

## <a name="members"></a><span data-ttu-id="10819-106">Membros</span><span class="sxs-lookup"><span data-stu-id="10819-106">Members</span></span>
|<span data-ttu-id="10819-107">Membro</span><span class="sxs-lookup"><span data-stu-id="10819-107">Member</span></span>|<span data-ttu-id="10819-108">Valor</span><span class="sxs-lookup"><span data-stu-id="10819-108">Value</span></span>|<span data-ttu-id="10819-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="10819-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10819-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="10819-110">deviceDefault</span></span>|<span data-ttu-id="10819-111">,0</span><span class="sxs-lookup"><span data-stu-id="10819-111">0</span></span>|<span data-ttu-id="10819-112">Aplicar ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="10819-112">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="10819-113">ordena</span><span class="sxs-lookup"><span data-stu-id="10819-113">clean</span></span>|<span data-ttu-id="10819-114">1</span><span class="sxs-lookup"><span data-stu-id="10819-114">1</span></span>|<span data-ttu-id="10819-115">Limpe a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="10819-115">Clean the detected threat.</span></span>|
|<span data-ttu-id="10819-116">quarentena</span><span class="sxs-lookup"><span data-stu-id="10819-116">quarantine</span></span>|<span data-ttu-id="10819-117">duas</span><span class="sxs-lookup"><span data-stu-id="10819-117">2</span></span>|<span data-ttu-id="10819-118">Colocar em quarentena a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="10819-118">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="10819-119">remover</span><span class="sxs-lookup"><span data-stu-id="10819-119">remove</span></span>|<span data-ttu-id="10819-120">3D</span><span class="sxs-lookup"><span data-stu-id="10819-120">3</span></span>|<span data-ttu-id="10819-121">Remova a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="10819-121">Remove the detected threat.</span></span>|
|<span data-ttu-id="10819-122">permitiu</span><span class="sxs-lookup"><span data-stu-id="10819-122">allow</span></span>|<span data-ttu-id="10819-123">quatro</span><span class="sxs-lookup"><span data-stu-id="10819-123">4</span></span>|<span data-ttu-id="10819-124">Permitir a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="10819-124">Allow the detected threat.</span></span>|
|<span data-ttu-id="10819-125">UserDefined</span><span class="sxs-lookup"><span data-stu-id="10819-125">userDefined</span></span>|<span data-ttu-id="10819-126">0,5</span><span class="sxs-lookup"><span data-stu-id="10819-126">5</span></span>|<span data-ttu-id="10819-127">Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="10819-127">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="10819-128">Larga</span><span class="sxs-lookup"><span data-stu-id="10819-128">block</span></span>|<span data-ttu-id="10819-129">6</span><span class="sxs-lookup"><span data-stu-id="10819-129">6</span></span>|<span data-ttu-id="10819-130">Bloquear a ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="10819-130">Block the detected threat.</span></span>|




