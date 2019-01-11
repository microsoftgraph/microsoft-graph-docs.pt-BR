---
title: tipo de enum windowsDeviceHealthState
description: Estado de proteção de ponto de extremidade do computador
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 91869502d0d61c25c6eb8dd67ba4e8e32d28fbb2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885922"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="716d8-103">tipo de enum windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="716d8-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="716d8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="716d8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="716d8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="716d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="716d8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="716d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="716d8-107">Estado de proteção de ponto de extremidade do computador</span><span class="sxs-lookup"><span data-stu-id="716d8-107">Computer endpoint protection state</span></span>
## <a name="members"></a><span data-ttu-id="716d8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="716d8-108">Members</span></span>
|<span data-ttu-id="716d8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="716d8-109">Member</span></span>|<span data-ttu-id="716d8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="716d8-110">Value</span></span>|<span data-ttu-id="716d8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="716d8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="716d8-112">clean</span><span class="sxs-lookup"><span data-stu-id="716d8-112">clean</span></span>|<span data-ttu-id="716d8-113">0</span><span class="sxs-lookup"><span data-stu-id="716d8-113">0</span></span>|<span data-ttu-id="716d8-114">Computador é limpa e nenhuma ação é necessária</span><span class="sxs-lookup"><span data-stu-id="716d8-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="716d8-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="716d8-115">fullScanPending</span></span>|<span data-ttu-id="716d8-116">1</span><span class="sxs-lookup"><span data-stu-id="716d8-116">1</span></span>|<span data-ttu-id="716d8-117">Computador está pendente estado de verificação completa</span><span class="sxs-lookup"><span data-stu-id="716d8-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="716d8-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="716d8-118">rebootPending</span></span>|<span data-ttu-id="716d8-119">2</span><span class="sxs-lookup"><span data-stu-id="716d8-119">2</span></span>|<span data-ttu-id="716d8-120">Computador está pendente estado de reinicialização</span><span class="sxs-lookup"><span data-stu-id="716d8-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="716d8-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="716d8-121">manualStepsPending</span></span>|<span data-ttu-id="716d8-122">4</span><span class="sxs-lookup"><span data-stu-id="716d8-122">4</span></span>|<span data-ttu-id="716d8-123">Computador está pendente estado etapas manuais</span><span class="sxs-lookup"><span data-stu-id="716d8-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="716d8-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="716d8-124">offlineScanPending</span></span>|<span data-ttu-id="716d8-125">8</span><span class="sxs-lookup"><span data-stu-id="716d8-125">8</span></span>|<span data-ttu-id="716d8-126">Computador está pendente estado de verificação offline</span><span class="sxs-lookup"><span data-stu-id="716d8-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="716d8-127">crítico</span><span class="sxs-lookup"><span data-stu-id="716d8-127">critical</span></span>|<span data-ttu-id="716d8-128">16</span><span class="sxs-lookup"><span data-stu-id="716d8-128">16</span></span>|<span data-ttu-id="716d8-129">Computador estiver em estado de falha grave</span><span class="sxs-lookup"><span data-stu-id="716d8-129">Computer is in critical failure state</span></span>|





