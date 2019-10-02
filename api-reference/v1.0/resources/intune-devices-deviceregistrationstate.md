---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2543f1a7d874a8443424fa1161187e7ccd771f7b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356916"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="0c60a-103">tipo de enumeração deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="0c60a-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="0c60a-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c60a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c60a-105">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c60a-105">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="0c60a-106">Membros</span><span class="sxs-lookup"><span data-stu-id="0c60a-106">Members</span></span>
|<span data-ttu-id="0c60a-107">Membro</span><span class="sxs-lookup"><span data-stu-id="0c60a-107">Member</span></span>|<span data-ttu-id="0c60a-108">Valor</span><span class="sxs-lookup"><span data-stu-id="0c60a-108">Value</span></span>|<span data-ttu-id="0c60a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c60a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c60a-110">Não registrado</span><span class="sxs-lookup"><span data-stu-id="0c60a-110">notRegistered</span></span>|<span data-ttu-id="0c60a-111">,0</span><span class="sxs-lookup"><span data-stu-id="0c60a-111">0</span></span>|<span data-ttu-id="0c60a-112">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="0c60a-112">The device is not registered.</span></span>|
|<span data-ttu-id="0c60a-113">inscreve</span><span class="sxs-lookup"><span data-stu-id="0c60a-113">registered</span></span>|<span data-ttu-id="0c60a-114">duas</span><span class="sxs-lookup"><span data-stu-id="0c60a-114">2</span></span>|<span data-ttu-id="0c60a-115">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="0c60a-115">The device is registered.</span></span>|
|<span data-ttu-id="0c60a-116">revogado</span><span class="sxs-lookup"><span data-stu-id="0c60a-116">revoked</span></span>|<span data-ttu-id="0c60a-117">3D</span><span class="sxs-lookup"><span data-stu-id="0c60a-117">3</span></span>|<span data-ttu-id="0c60a-118">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="0c60a-118">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="0c60a-119">keyconflict</span><span class="sxs-lookup"><span data-stu-id="0c60a-119">keyConflict</span></span>|<span data-ttu-id="0c60a-120">quatro</span><span class="sxs-lookup"><span data-stu-id="0c60a-120">4</span></span>|<span data-ttu-id="0c60a-121">O dispositivo tem um conflito de teclas.</span><span class="sxs-lookup"><span data-stu-id="0c60a-121">The device has a key conflict.</span></span>|
|<span data-ttu-id="0c60a-122">approvalPending</span><span class="sxs-lookup"><span data-stu-id="0c60a-122">approvalPending</span></span>|<span data-ttu-id="0c60a-123">0,5</span><span class="sxs-lookup"><span data-stu-id="0c60a-123">5</span></span>|<span data-ttu-id="0c60a-124">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="0c60a-124">The device is pending approval.</span></span>|
|<span data-ttu-id="0c60a-125">certificateReset</span><span class="sxs-lookup"><span data-stu-id="0c60a-125">certificateReset</span></span>|<span data-ttu-id="0c60a-126">6</span><span class="sxs-lookup"><span data-stu-id="0c60a-126">6</span></span>|<span data-ttu-id="0c60a-127">O certificado de dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="0c60a-127">The device certificate has been reset.</span></span>|
|<span data-ttu-id="0c60a-128">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="0c60a-128">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="0c60a-129">178</span><span class="sxs-lookup"><span data-stu-id="0c60a-129">7</span></span>|<span data-ttu-id="0c60a-130">O dispositivo não está registrado e registro pendente.</span><span class="sxs-lookup"><span data-stu-id="0c60a-130">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="0c60a-131">desconhecido</span><span class="sxs-lookup"><span data-stu-id="0c60a-131">unknown</span></span>|<span data-ttu-id="0c60a-132">8 </span><span class="sxs-lookup"><span data-stu-id="0c60a-132">8</span></span>|<span data-ttu-id="0c60a-133">O status do registro do dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="0c60a-133">The device registration status is unknown.</span></span>|




