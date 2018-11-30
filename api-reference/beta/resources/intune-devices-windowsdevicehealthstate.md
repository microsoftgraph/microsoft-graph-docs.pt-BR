---
title: tipo de enum windowsDeviceHealthState
description: Estado de proteção de ponto de extremidade do computador
ms.openlocfilehash: 601531dd71ee0d44e9f5ebc89eb018ba5e0f2675
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033006"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="c2a81-103">tipo de enum windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="c2a81-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="c2a81-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c2a81-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2a81-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c2a81-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2a81-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c2a81-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2a81-107">Estado de proteção de ponto de extremidade do computador</span><span class="sxs-lookup"><span data-stu-id="c2a81-107">Computer endpoint protection state</span></span>
## <a name="members"></a><span data-ttu-id="c2a81-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c2a81-108">Members</span></span>
|<span data-ttu-id="c2a81-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c2a81-109">Member</span></span>|<span data-ttu-id="c2a81-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c2a81-110">Value</span></span>|<span data-ttu-id="c2a81-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2a81-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2a81-112">clean</span><span class="sxs-lookup"><span data-stu-id="c2a81-112">clean</span></span>|<span data-ttu-id="c2a81-113">0</span><span class="sxs-lookup"><span data-stu-id="c2a81-113">0</span></span>|<span data-ttu-id="c2a81-114">Computador é limpa e nenhuma ação é necessária</span><span class="sxs-lookup"><span data-stu-id="c2a81-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="c2a81-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="c2a81-115">fullScanPending</span></span>|<span data-ttu-id="c2a81-116">1</span><span class="sxs-lookup"><span data-stu-id="c2a81-116">1</span></span>|<span data-ttu-id="c2a81-117">Computador está pendente estado de verificação completa</span><span class="sxs-lookup"><span data-stu-id="c2a81-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="c2a81-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="c2a81-118">rebootPending</span></span>|<span data-ttu-id="c2a81-119">2</span><span class="sxs-lookup"><span data-stu-id="c2a81-119">2</span></span>|<span data-ttu-id="c2a81-120">Computador está pendente estado de reinicialização</span><span class="sxs-lookup"><span data-stu-id="c2a81-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="c2a81-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="c2a81-121">manualStepsPending</span></span>|<span data-ttu-id="c2a81-122">4</span><span class="sxs-lookup"><span data-stu-id="c2a81-122">4</span></span>|<span data-ttu-id="c2a81-123">Computador está pendente estado etapas manuais</span><span class="sxs-lookup"><span data-stu-id="c2a81-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="c2a81-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="c2a81-124">offlineScanPending</span></span>|<span data-ttu-id="c2a81-125">8</span><span class="sxs-lookup"><span data-stu-id="c2a81-125">8</span></span>|<span data-ttu-id="c2a81-126">Computador está pendente estado de verificação offline</span><span class="sxs-lookup"><span data-stu-id="c2a81-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="c2a81-127">crítico</span><span class="sxs-lookup"><span data-stu-id="c2a81-127">critical</span></span>|<span data-ttu-id="c2a81-128">16</span><span class="sxs-lookup"><span data-stu-id="c2a81-128">16</span></span>|<span data-ttu-id="c2a81-129">Computador estiver em estado de falha grave</span><span class="sxs-lookup"><span data-stu-id="c2a81-129">Computer is in critical failure state</span></span>|





