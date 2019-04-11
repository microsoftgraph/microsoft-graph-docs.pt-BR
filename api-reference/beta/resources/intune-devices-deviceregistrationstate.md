---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b777452b627208d8e2dd726815f321075e5745ae
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794012"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="9c24f-103">tipo de enumeração deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="9c24f-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="9c24f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9c24f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c24f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c24f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c24f-106">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9c24f-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="9c24f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="9c24f-107">Members</span></span>
|<span data-ttu-id="9c24f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="9c24f-108">Member</span></span>|<span data-ttu-id="9c24f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="9c24f-109">Value</span></span>|<span data-ttu-id="9c24f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c24f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c24f-111">Não registrado</span><span class="sxs-lookup"><span data-stu-id="9c24f-111">notRegistered</span></span>|<span data-ttu-id="9c24f-112">,0</span><span class="sxs-lookup"><span data-stu-id="9c24f-112">0</span></span>|<span data-ttu-id="9c24f-113">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="9c24f-113">The device is not registered.</span></span>|
|<span data-ttu-id="9c24f-114">inscreve</span><span class="sxs-lookup"><span data-stu-id="9c24f-114">registered</span></span>|<span data-ttu-id="9c24f-115">duas</span><span class="sxs-lookup"><span data-stu-id="9c24f-115">2</span></span>|<span data-ttu-id="9c24f-116">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="9c24f-116">The device is registered.</span></span>|
|<span data-ttu-id="9c24f-117">revogado</span><span class="sxs-lookup"><span data-stu-id="9c24f-117">revoked</span></span>|<span data-ttu-id="9c24f-118">3D</span><span class="sxs-lookup"><span data-stu-id="9c24f-118">3</span></span>|<span data-ttu-id="9c24f-119">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="9c24f-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="9c24f-120">keyConflict</span><span class="sxs-lookup"><span data-stu-id="9c24f-120">keyConflict</span></span>|<span data-ttu-id="9c24f-121">quatro</span><span class="sxs-lookup"><span data-stu-id="9c24f-121">4</span></span>|<span data-ttu-id="9c24f-122">O dispositivo tem um conflito de teclas.</span><span class="sxs-lookup"><span data-stu-id="9c24f-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="9c24f-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="9c24f-123">approvalPending</span></span>|<span data-ttu-id="9c24f-124">0,5</span><span class="sxs-lookup"><span data-stu-id="9c24f-124">5</span></span>|<span data-ttu-id="9c24f-125">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="9c24f-125">The device is pending approval.</span></span>|
|<span data-ttu-id="9c24f-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="9c24f-126">certificateReset</span></span>|<span data-ttu-id="9c24f-127">6</span><span class="sxs-lookup"><span data-stu-id="9c24f-127">6</span></span>|<span data-ttu-id="9c24f-128">O certificado de dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="9c24f-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="9c24f-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="9c24f-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="9c24f-130">178</span><span class="sxs-lookup"><span data-stu-id="9c24f-130">7</span></span>|<span data-ttu-id="9c24f-131">O dispositivo não está registrado e registro pendente.</span><span class="sxs-lookup"><span data-stu-id="9c24f-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="9c24f-132">desconhecido</span><span class="sxs-lookup"><span data-stu-id="9c24f-132">unknown</span></span>|<span data-ttu-id="9c24f-133">8</span><span class="sxs-lookup"><span data-stu-id="9c24f-133">8</span></span>|<span data-ttu-id="9c24f-134">O status do registro do dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="9c24f-134">The device registration status is unknown.</span></span>|





