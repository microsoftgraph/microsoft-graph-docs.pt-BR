---
title: tipo de enum windowsDeviceHealthState
description: Estado de proteção de ponto de extremidade do computador
author: tfitzmac
ms.openlocfilehash: b794f8121132e396459f9198c644084690fe95b4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326324"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="9bcbc-103">tipo de enum windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="9bcbc-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="9bcbc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9bcbc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bcbc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9bcbc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9bcbc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9bcbc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9bcbc-107">Estado de proteção de ponto de extremidade do computador</span><span class="sxs-lookup"><span data-stu-id="9bcbc-107">Computer endpoint protection state</span></span>
## <a name="members"></a><span data-ttu-id="9bcbc-108">Membros</span><span class="sxs-lookup"><span data-stu-id="9bcbc-108">Members</span></span>
|<span data-ttu-id="9bcbc-109">Membro</span><span class="sxs-lookup"><span data-stu-id="9bcbc-109">Member</span></span>|<span data-ttu-id="9bcbc-110">Valor</span><span class="sxs-lookup"><span data-stu-id="9bcbc-110">Value</span></span>|<span data-ttu-id="9bcbc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bcbc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bcbc-112">clean</span><span class="sxs-lookup"><span data-stu-id="9bcbc-112">clean</span></span>|<span data-ttu-id="9bcbc-113">0</span><span class="sxs-lookup"><span data-stu-id="9bcbc-113">0</span></span>|<span data-ttu-id="9bcbc-114">Computador é limpa e nenhuma ação é necessária</span><span class="sxs-lookup"><span data-stu-id="9bcbc-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="9bcbc-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="9bcbc-115">fullScanPending</span></span>|<span data-ttu-id="9bcbc-116">1</span><span class="sxs-lookup"><span data-stu-id="9bcbc-116">1</span></span>|<span data-ttu-id="9bcbc-117">Computador está pendente estado de verificação completa</span><span class="sxs-lookup"><span data-stu-id="9bcbc-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="9bcbc-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="9bcbc-118">rebootPending</span></span>|<span data-ttu-id="9bcbc-119">2</span><span class="sxs-lookup"><span data-stu-id="9bcbc-119">2</span></span>|<span data-ttu-id="9bcbc-120">Computador está pendente estado de reinicialização</span><span class="sxs-lookup"><span data-stu-id="9bcbc-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="9bcbc-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="9bcbc-121">manualStepsPending</span></span>|<span data-ttu-id="9bcbc-122">4</span><span class="sxs-lookup"><span data-stu-id="9bcbc-122">4</span></span>|<span data-ttu-id="9bcbc-123">Computador está pendente estado etapas manuais</span><span class="sxs-lookup"><span data-stu-id="9bcbc-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="9bcbc-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="9bcbc-124">offlineScanPending</span></span>|<span data-ttu-id="9bcbc-125">8</span><span class="sxs-lookup"><span data-stu-id="9bcbc-125">8</span></span>|<span data-ttu-id="9bcbc-126">Computador está pendente estado de verificação offline</span><span class="sxs-lookup"><span data-stu-id="9bcbc-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="9bcbc-127">crítico</span><span class="sxs-lookup"><span data-stu-id="9bcbc-127">critical</span></span>|<span data-ttu-id="9bcbc-128">16</span><span class="sxs-lookup"><span data-stu-id="9bcbc-128">16</span></span>|<span data-ttu-id="9bcbc-129">Computador estiver em estado de falha grave</span><span class="sxs-lookup"><span data-stu-id="9bcbc-129">Computer is in critical failure state</span></span>|





