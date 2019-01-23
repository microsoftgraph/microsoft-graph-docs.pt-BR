---
title: tipo de enum windowsDeviceHealthState
description: Estado de proteção de ponto de extremidade do computador
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2d971de9b20780bb51a19c3417384a0ca0563452
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416346"
---
# <a name="windowsdevicehealthstate-enum-type"></a><span data-ttu-id="17537-103">tipo de enum windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="17537-103">windowsDeviceHealthState enum type</span></span>

> <span data-ttu-id="17537-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="17537-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="17537-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="17537-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17537-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="17537-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17537-107">Estado de proteção de ponto de extremidade do computador</span><span class="sxs-lookup"><span data-stu-id="17537-107">Computer endpoint protection state</span></span>

## <a name="members"></a><span data-ttu-id="17537-108">Membros</span><span class="sxs-lookup"><span data-stu-id="17537-108">Members</span></span>
|<span data-ttu-id="17537-109">Membro</span><span class="sxs-lookup"><span data-stu-id="17537-109">Member</span></span>|<span data-ttu-id="17537-110">Valor</span><span class="sxs-lookup"><span data-stu-id="17537-110">Value</span></span>|<span data-ttu-id="17537-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="17537-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17537-112">clean</span><span class="sxs-lookup"><span data-stu-id="17537-112">clean</span></span>|<span data-ttu-id="17537-113">0</span><span class="sxs-lookup"><span data-stu-id="17537-113">0</span></span>|<span data-ttu-id="17537-114">Computador é limpa e nenhuma ação é necessária</span><span class="sxs-lookup"><span data-stu-id="17537-114">Computer is clean and no action is required</span></span>|
|<span data-ttu-id="17537-115">fullScanPending</span><span class="sxs-lookup"><span data-stu-id="17537-115">fullScanPending</span></span>|<span data-ttu-id="17537-116">1</span><span class="sxs-lookup"><span data-stu-id="17537-116">1</span></span>|<span data-ttu-id="17537-117">Computador está pendente estado de verificação completa</span><span class="sxs-lookup"><span data-stu-id="17537-117">Computer is in pending full scan state</span></span>|
|<span data-ttu-id="17537-118">rebootPending</span><span class="sxs-lookup"><span data-stu-id="17537-118">rebootPending</span></span>|<span data-ttu-id="17537-119">2</span><span class="sxs-lookup"><span data-stu-id="17537-119">2</span></span>|<span data-ttu-id="17537-120">Computador está pendente estado de reinicialização</span><span class="sxs-lookup"><span data-stu-id="17537-120">Computer is in pending reboot state</span></span>|
|<span data-ttu-id="17537-121">manualStepsPending</span><span class="sxs-lookup"><span data-stu-id="17537-121">manualStepsPending</span></span>|<span data-ttu-id="17537-122">4</span><span class="sxs-lookup"><span data-stu-id="17537-122">4</span></span>|<span data-ttu-id="17537-123">Computador está pendente estado etapas manuais</span><span class="sxs-lookup"><span data-stu-id="17537-123">Computer is in pending manual steps state</span></span>|
|<span data-ttu-id="17537-124">offlineScanPending</span><span class="sxs-lookup"><span data-stu-id="17537-124">offlineScanPending</span></span>|<span data-ttu-id="17537-125">8</span><span class="sxs-lookup"><span data-stu-id="17537-125">8</span></span>|<span data-ttu-id="17537-126">Computador está pendente estado de verificação offline</span><span class="sxs-lookup"><span data-stu-id="17537-126">Computer is in pending offline scan state</span></span>|
|<span data-ttu-id="17537-127">crítico</span><span class="sxs-lookup"><span data-stu-id="17537-127">critical</span></span>|<span data-ttu-id="17537-128">16</span><span class="sxs-lookup"><span data-stu-id="17537-128">16</span></span>|<span data-ttu-id="17537-129">Computador estiver em estado de falha grave</span><span class="sxs-lookup"><span data-stu-id="17537-129">Computer is in critical failure state</span></span>|




