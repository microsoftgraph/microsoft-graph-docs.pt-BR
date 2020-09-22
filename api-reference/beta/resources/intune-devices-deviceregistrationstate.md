---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 628d4c6c253349e54747d4fce836a2b4c8f4579f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081423"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="a8648-103">tipo de enumeração deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="a8648-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="a8648-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8648-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8648-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8648-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8648-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8648-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8648-107">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a8648-107">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="a8648-108">Membros</span><span class="sxs-lookup"><span data-stu-id="a8648-108">Members</span></span>
|<span data-ttu-id="a8648-109">Membro</span><span class="sxs-lookup"><span data-stu-id="a8648-109">Member</span></span>|<span data-ttu-id="a8648-110">Valor</span><span class="sxs-lookup"><span data-stu-id="a8648-110">Value</span></span>|<span data-ttu-id="a8648-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8648-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8648-112">Não registrado</span><span class="sxs-lookup"><span data-stu-id="a8648-112">notRegistered</span></span>|<span data-ttu-id="a8648-113">,0</span><span class="sxs-lookup"><span data-stu-id="a8648-113">0</span></span>|<span data-ttu-id="a8648-114">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="a8648-114">The device is not registered.</span></span>|
|<span data-ttu-id="a8648-115">inscreve</span><span class="sxs-lookup"><span data-stu-id="a8648-115">registered</span></span>|<span data-ttu-id="a8648-116">2 </span><span class="sxs-lookup"><span data-stu-id="a8648-116">2</span></span>|<span data-ttu-id="a8648-117">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="a8648-117">The device is registered.</span></span>|
|<span data-ttu-id="a8648-118">revogado</span><span class="sxs-lookup"><span data-stu-id="a8648-118">revoked</span></span>|<span data-ttu-id="a8648-119">3D</span><span class="sxs-lookup"><span data-stu-id="a8648-119">3</span></span>|<span data-ttu-id="a8648-120">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="a8648-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="a8648-121">keyconflict</span><span class="sxs-lookup"><span data-stu-id="a8648-121">keyConflict</span></span>|<span data-ttu-id="a8648-122">4 </span><span class="sxs-lookup"><span data-stu-id="a8648-122">4</span></span>|<span data-ttu-id="a8648-123">O dispositivo tem um conflito de teclas.</span><span class="sxs-lookup"><span data-stu-id="a8648-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="a8648-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="a8648-124">approvalPending</span></span>|<span data-ttu-id="a8648-125">5 </span><span class="sxs-lookup"><span data-stu-id="a8648-125">5</span></span>|<span data-ttu-id="a8648-126">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="a8648-126">The device is pending approval.</span></span>|
|<span data-ttu-id="a8648-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="a8648-127">certificateReset</span></span>|<span data-ttu-id="a8648-128">6 </span><span class="sxs-lookup"><span data-stu-id="a8648-128">6</span></span>|<span data-ttu-id="a8648-129">O certificado de dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="a8648-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="a8648-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="a8648-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="a8648-131">7 </span><span class="sxs-lookup"><span data-stu-id="a8648-131">7</span></span>|<span data-ttu-id="a8648-132">O dispositivo não está registrado e registro pendente.</span><span class="sxs-lookup"><span data-stu-id="a8648-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="a8648-133">desconhecido</span><span class="sxs-lookup"><span data-stu-id="a8648-133">unknown</span></span>|<span data-ttu-id="a8648-134">8 </span><span class="sxs-lookup"><span data-stu-id="a8648-134">8</span></span>|<span data-ttu-id="a8648-135">O status do registro do dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="a8648-135">The device registration status is unknown.</span></span>|






