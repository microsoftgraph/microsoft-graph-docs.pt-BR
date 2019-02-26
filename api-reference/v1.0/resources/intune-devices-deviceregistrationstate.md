---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b3bee7ab56f07dd6f27c20c771329ba84edbb19
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264131"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="2c763-103">tipo de enumeração deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="2c763-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="2c763-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c763-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c763-105">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c763-105">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="2c763-106">Membros</span><span class="sxs-lookup"><span data-stu-id="2c763-106">Members</span></span>
|<span data-ttu-id="2c763-107">Membro</span><span class="sxs-lookup"><span data-stu-id="2c763-107">Member</span></span>|<span data-ttu-id="2c763-108">Valor</span><span class="sxs-lookup"><span data-stu-id="2c763-108">Value</span></span>|<span data-ttu-id="2c763-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c763-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c763-110">Não registrado</span><span class="sxs-lookup"><span data-stu-id="2c763-110">notRegistered</span></span>|<span data-ttu-id="2c763-111">,0</span><span class="sxs-lookup"><span data-stu-id="2c763-111">0</span></span>|<span data-ttu-id="2c763-112">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="2c763-112">The device is not registered.</span></span>|
|<span data-ttu-id="2c763-113">inscreve</span><span class="sxs-lookup"><span data-stu-id="2c763-113">registered</span></span>|<span data-ttu-id="2c763-114">duas</span><span class="sxs-lookup"><span data-stu-id="2c763-114">2</span></span>|<span data-ttu-id="2c763-115">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="2c763-115">The device is registered.</span></span>|
|<span data-ttu-id="2c763-116">revogado</span><span class="sxs-lookup"><span data-stu-id="2c763-116">revoked</span></span>|<span data-ttu-id="2c763-117">3D</span><span class="sxs-lookup"><span data-stu-id="2c763-117">3</span></span>|<span data-ttu-id="2c763-118">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="2c763-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="2c763-119">keyConflict</span><span class="sxs-lookup"><span data-stu-id="2c763-119">keyConflict</span></span>|<span data-ttu-id="2c763-120">quatro</span><span class="sxs-lookup"><span data-stu-id="2c763-120">4</span></span>|<span data-ttu-id="2c763-121">O dispositivo tem um conflito de teclas.</span><span class="sxs-lookup"><span data-stu-id="2c763-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="2c763-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="2c763-122">approvalPending</span></span>|<span data-ttu-id="2c763-123">0,5</span><span class="sxs-lookup"><span data-stu-id="2c763-123">5</span></span>|<span data-ttu-id="2c763-124">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="2c763-124">The device is pending approval.</span></span>|
|<span data-ttu-id="2c763-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="2c763-125">certificateReset</span></span>|<span data-ttu-id="2c763-126">6</span><span class="sxs-lookup"><span data-stu-id="2c763-126">6</span></span>|<span data-ttu-id="2c763-127">O certificado de dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="2c763-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="2c763-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="2c763-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="2c763-129">178</span><span class="sxs-lookup"><span data-stu-id="2c763-129">7</span></span>|<span data-ttu-id="2c763-130">O dispositivo não está registrado e registro pendente.</span><span class="sxs-lookup"><span data-stu-id="2c763-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="2c763-131">unknown</span><span class="sxs-lookup"><span data-stu-id="2c763-131">unknown</span></span>|<span data-ttu-id="2c763-132">8</span><span class="sxs-lookup"><span data-stu-id="2c763-132">8</span></span>|<span data-ttu-id="2c763-133">O status do registro do dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="2c763-133">The device registration status is unknown.</span></span>|



