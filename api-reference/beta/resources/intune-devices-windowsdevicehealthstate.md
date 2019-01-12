---
title: tipo de enum windowsDeviceHealthState
description: Estado de proteção de ponto de extremidade do computador
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 628450b33a219e8408d5c5887c6902b78ae02bd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923940"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="38e1e-103">tipo de enum windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="38e1e-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="38e1e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="38e1e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38e1e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="38e1e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38e1e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="38e1e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38e1e-107">Estado de proteção de ponto de extremidade do computador</span><span class="sxs-lookup"><span data-stu-id="38e1e-107">Computer endpoint protection state</span></span>
## <a name="members"></a><span data-ttu-id="38e1e-108">Membros</span><span class="sxs-lookup"><span data-stu-id="38e1e-108">Members</span></span>
|<span data-ttu-id="38e1e-109">Membro</span><span class="sxs-lookup"><span data-stu-id="38e1e-109">Member</span></span>|<span data-ttu-id="38e1e-110">Valor</span><span class="sxs-lookup"><span data-stu-id="38e1e-110">Value</span></span>|<span data-ttu-id="38e1e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="38e1e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38e1e-112">clean</span><span class="sxs-lookup"><span data-stu-id="38e1e-112">clean</span></span>|<span data-ttu-id="38e1e-113">0</span><span class="sxs-lookup"><span data-stu-id="38e1e-113">0</span></span>|<span data-ttu-id="38e1e-114">Computador é limpa e nenhuma ação é necessária</span><span class="sxs-lookup"><span data-stu-id="38e1e-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="38e1e-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="38e1e-115">fullScanPending</span></span>|<span data-ttu-id="38e1e-116">1</span><span class="sxs-lookup"><span data-stu-id="38e1e-116">1</span></span>|<span data-ttu-id="38e1e-117">Computador está pendente estado de verificação completa</span><span class="sxs-lookup"><span data-stu-id="38e1e-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="38e1e-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="38e1e-118">rebootPending</span></span>|<span data-ttu-id="38e1e-119">2</span><span class="sxs-lookup"><span data-stu-id="38e1e-119">2</span></span>|<span data-ttu-id="38e1e-120">Computador está pendente estado de reinicialização</span><span class="sxs-lookup"><span data-stu-id="38e1e-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="38e1e-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="38e1e-121">manualStepsPending</span></span>|<span data-ttu-id="38e1e-122">4</span><span class="sxs-lookup"><span data-stu-id="38e1e-122">4</span></span>|<span data-ttu-id="38e1e-123">Computador está pendente estado etapas manuais</span><span class="sxs-lookup"><span data-stu-id="38e1e-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="38e1e-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="38e1e-124">offlineScanPending</span></span>|<span data-ttu-id="38e1e-125">8</span><span class="sxs-lookup"><span data-stu-id="38e1e-125">8</span></span>|<span data-ttu-id="38e1e-126">Computador está pendente estado de verificação offline</span><span class="sxs-lookup"><span data-stu-id="38e1e-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="38e1e-127">crítico</span><span class="sxs-lookup"><span data-stu-id="38e1e-127">critical</span></span>|<span data-ttu-id="38e1e-128">16</span><span class="sxs-lookup"><span data-stu-id="38e1e-128">16</span></span>|<span data-ttu-id="38e1e-129">Computador estiver em estado de falha grave</span><span class="sxs-lookup"><span data-stu-id="38e1e-129">Computer is in critical failure state</span></span>|





