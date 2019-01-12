---
title: tipo de enum defenderThreatAction
description: Ação de padrão do Defender assuma detectadas ameaças de Malware.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: fb54523f2817da328854e57a6672045e46ceb266
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938080"
---
# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="dac2e-103">tipo de enum defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="dac2e-103">defenderThreatAction enum type</span></span>

> <span data-ttu-id="dac2e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dac2e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dac2e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dac2e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dac2e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dac2e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dac2e-107">Ação de padrão do Defender assuma detectadas ameaças de Malware.</span><span class="sxs-lookup"><span data-stu-id="dac2e-107">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="dac2e-108">Membros</span><span class="sxs-lookup"><span data-stu-id="dac2e-108">Members</span></span>
|<span data-ttu-id="dac2e-109">Membro</span><span class="sxs-lookup"><span data-stu-id="dac2e-109">Member</span></span>|<span data-ttu-id="dac2e-110">Valor</span><span class="sxs-lookup"><span data-stu-id="dac2e-110">Value</span></span>|<span data-ttu-id="dac2e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dac2e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dac2e-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="dac2e-112">deviceDefault</span></span>|<span data-ttu-id="dac2e-113">0</span><span class="sxs-lookup"><span data-stu-id="dac2e-113">0</span></span>|<span data-ttu-id="dac2e-114">Aplica a ação com base na definição de atualização.</span><span class="sxs-lookup"><span data-stu-id="dac2e-114">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="dac2e-115">clean</span><span class="sxs-lookup"><span data-stu-id="dac2e-115">clean</span></span>|<span data-ttu-id="dac2e-116">1</span><span class="sxs-lookup"><span data-stu-id="dac2e-116">1</span></span>|<span data-ttu-id="dac2e-117">Limpe ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="dac2e-117">Clean the detected threat.</span></span>|
|<span data-ttu-id="dac2e-118">quarentena</span><span class="sxs-lookup"><span data-stu-id="dac2e-118">quarantine</span></span>|<span data-ttu-id="dac2e-119">2</span><span class="sxs-lookup"><span data-stu-id="dac2e-119">2</span></span>|<span data-ttu-id="dac2e-120">Quarentena ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="dac2e-120">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="dac2e-121">remover</span><span class="sxs-lookup"><span data-stu-id="dac2e-121">remove</span></span>|<span data-ttu-id="dac2e-122">3</span><span class="sxs-lookup"><span data-stu-id="dac2e-122">3</span></span>|<span data-ttu-id="dac2e-123">Remova ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="dac2e-123">Remove the detected threat.</span></span>|
|<span data-ttu-id="dac2e-124">permitir</span><span class="sxs-lookup"><span data-stu-id="dac2e-124">allow</span></span>|<span data-ttu-id="dac2e-125">4</span><span class="sxs-lookup"><span data-stu-id="dac2e-125">4</span></span>|<span data-ttu-id="dac2e-126">Permitir ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="dac2e-126">Allow the detected threat.</span></span>|
|<span data-ttu-id="dac2e-127">userDefined</span><span class="sxs-lookup"><span data-stu-id="dac2e-127">userDefined</span></span>|<span data-ttu-id="dac2e-128">5</span><span class="sxs-lookup"><span data-stu-id="dac2e-128">5</span></span>|<span data-ttu-id="dac2e-129">Permitir que o usuário determinar a ação a ser executada com ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="dac2e-129">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="dac2e-130">bloquear</span><span class="sxs-lookup"><span data-stu-id="dac2e-130">block</span></span>|<span data-ttu-id="dac2e-131">6</span><span class="sxs-lookup"><span data-stu-id="dac2e-131">6</span></span>|<span data-ttu-id="dac2e-132">Bloquear ameaça detectada.</span><span class="sxs-lookup"><span data-stu-id="dac2e-132">Block the detected threat.</span></span>|





