---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e153ac5c1bfbd09540fd55b5df23eab095e2a002
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968383"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="814c5-103">tipo de enumeração deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="814c5-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="814c5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="814c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="814c5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="814c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="814c5-106">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="814c5-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="814c5-107">Membros</span><span class="sxs-lookup"><span data-stu-id="814c5-107">Members</span></span>
|<span data-ttu-id="814c5-108">Membro</span><span class="sxs-lookup"><span data-stu-id="814c5-108">Member</span></span>|<span data-ttu-id="814c5-109">Valor</span><span class="sxs-lookup"><span data-stu-id="814c5-109">Value</span></span>|<span data-ttu-id="814c5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="814c5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="814c5-111">Não registrado</span><span class="sxs-lookup"><span data-stu-id="814c5-111">notRegistered</span></span>|<span data-ttu-id="814c5-112">,0</span><span class="sxs-lookup"><span data-stu-id="814c5-112">0</span></span>|<span data-ttu-id="814c5-113">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="814c5-113">The device is not registered.</span></span>|
|<span data-ttu-id="814c5-114">inscreve</span><span class="sxs-lookup"><span data-stu-id="814c5-114">registered</span></span>|<span data-ttu-id="814c5-115">duas</span><span class="sxs-lookup"><span data-stu-id="814c5-115">2</span></span>|<span data-ttu-id="814c5-116">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="814c5-116">The device is registered.</span></span>|
|<span data-ttu-id="814c5-117">revogado</span><span class="sxs-lookup"><span data-stu-id="814c5-117">revoked</span></span>|<span data-ttu-id="814c5-118">3D</span><span class="sxs-lookup"><span data-stu-id="814c5-118">3</span></span>|<span data-ttu-id="814c5-119">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="814c5-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="814c5-120">keyconflict</span><span class="sxs-lookup"><span data-stu-id="814c5-120">keyConflict</span></span>|<span data-ttu-id="814c5-121">quatro</span><span class="sxs-lookup"><span data-stu-id="814c5-121">4</span></span>|<span data-ttu-id="814c5-122">O dispositivo tem um conflito de teclas.</span><span class="sxs-lookup"><span data-stu-id="814c5-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="814c5-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="814c5-123">approvalPending</span></span>|<span data-ttu-id="814c5-124">0,5</span><span class="sxs-lookup"><span data-stu-id="814c5-124">5</span></span>|<span data-ttu-id="814c5-125">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="814c5-125">The device is pending approval.</span></span>|
|<span data-ttu-id="814c5-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="814c5-126">certificateReset</span></span>|<span data-ttu-id="814c5-127">6</span><span class="sxs-lookup"><span data-stu-id="814c5-127">6</span></span>|<span data-ttu-id="814c5-128">O certificado de dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="814c5-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="814c5-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="814c5-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="814c5-130">178</span><span class="sxs-lookup"><span data-stu-id="814c5-130">7</span></span>|<span data-ttu-id="814c5-131">O dispositivo não está registrado e registro pendente.</span><span class="sxs-lookup"><span data-stu-id="814c5-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="814c5-132">desconhecido</span><span class="sxs-lookup"><span data-stu-id="814c5-132">unknown</span></span>|<span data-ttu-id="814c5-133">8 </span><span class="sxs-lookup"><span data-stu-id="814c5-133">8</span></span>|<span data-ttu-id="814c5-134">O status do registro do dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="814c5-134">The device registration status is unknown.</span></span>|





