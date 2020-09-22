---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 678db76ca3218515306e847abf38c8dcac9d3b20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091149"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="95e2d-103">tipo de enumeração deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="95e2d-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="95e2d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95e2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95e2d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95e2d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95e2d-106">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95e2d-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="95e2d-107">Membros</span><span class="sxs-lookup"><span data-stu-id="95e2d-107">Members</span></span>
|<span data-ttu-id="95e2d-108">Membro</span><span class="sxs-lookup"><span data-stu-id="95e2d-108">Member</span></span>|<span data-ttu-id="95e2d-109">Valor</span><span class="sxs-lookup"><span data-stu-id="95e2d-109">Value</span></span>|<span data-ttu-id="95e2d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="95e2d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95e2d-111">Não registrado</span><span class="sxs-lookup"><span data-stu-id="95e2d-111">notRegistered</span></span>|<span data-ttu-id="95e2d-112">,0</span><span class="sxs-lookup"><span data-stu-id="95e2d-112">0</span></span>|<span data-ttu-id="95e2d-113">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="95e2d-113">The device is not registered.</span></span>|
|<span data-ttu-id="95e2d-114">inscreve</span><span class="sxs-lookup"><span data-stu-id="95e2d-114">registered</span></span>|<span data-ttu-id="95e2d-115">2 </span><span class="sxs-lookup"><span data-stu-id="95e2d-115">2</span></span>|<span data-ttu-id="95e2d-116">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="95e2d-116">The device is registered.</span></span>|
|<span data-ttu-id="95e2d-117">revogado</span><span class="sxs-lookup"><span data-stu-id="95e2d-117">revoked</span></span>|<span data-ttu-id="95e2d-118">3D</span><span class="sxs-lookup"><span data-stu-id="95e2d-118">3</span></span>|<span data-ttu-id="95e2d-119">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="95e2d-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="95e2d-120">keyconflict</span><span class="sxs-lookup"><span data-stu-id="95e2d-120">keyConflict</span></span>|<span data-ttu-id="95e2d-121">4 </span><span class="sxs-lookup"><span data-stu-id="95e2d-121">4</span></span>|<span data-ttu-id="95e2d-122">O dispositivo tem um conflito de teclas.</span><span class="sxs-lookup"><span data-stu-id="95e2d-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="95e2d-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="95e2d-123">approvalPending</span></span>|<span data-ttu-id="95e2d-124">5 </span><span class="sxs-lookup"><span data-stu-id="95e2d-124">5</span></span>|<span data-ttu-id="95e2d-125">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="95e2d-125">The device is pending approval.</span></span>|
|<span data-ttu-id="95e2d-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="95e2d-126">certificateReset</span></span>|<span data-ttu-id="95e2d-127">6 </span><span class="sxs-lookup"><span data-stu-id="95e2d-127">6</span></span>|<span data-ttu-id="95e2d-128">O certificado de dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="95e2d-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="95e2d-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="95e2d-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="95e2d-130">7 </span><span class="sxs-lookup"><span data-stu-id="95e2d-130">7</span></span>|<span data-ttu-id="95e2d-131">O dispositivo não está registrado e registro pendente.</span><span class="sxs-lookup"><span data-stu-id="95e2d-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="95e2d-132">desconhecido</span><span class="sxs-lookup"><span data-stu-id="95e2d-132">unknown</span></span>|<span data-ttu-id="95e2d-133">8 </span><span class="sxs-lookup"><span data-stu-id="95e2d-133">8</span></span>|<span data-ttu-id="95e2d-134">O status do registro do dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="95e2d-134">The device registration status is unknown.</span></span>|









