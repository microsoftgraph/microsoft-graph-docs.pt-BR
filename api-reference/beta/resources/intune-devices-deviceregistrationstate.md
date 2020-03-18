---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 908f38a2da8f5960eb9c5f1879b7b54374b806ed
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784130"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="360d9-103">tipo de enumeração deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="360d9-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="360d9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="360d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="360d9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="360d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="360d9-106">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="360d9-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="360d9-107">Membros</span><span class="sxs-lookup"><span data-stu-id="360d9-107">Members</span></span>
|<span data-ttu-id="360d9-108">Membro</span><span class="sxs-lookup"><span data-stu-id="360d9-108">Member</span></span>|<span data-ttu-id="360d9-109">Valor</span><span class="sxs-lookup"><span data-stu-id="360d9-109">Value</span></span>|<span data-ttu-id="360d9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="360d9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="360d9-111">Não registrado</span><span class="sxs-lookup"><span data-stu-id="360d9-111">notRegistered</span></span>|<span data-ttu-id="360d9-112">,0</span><span class="sxs-lookup"><span data-stu-id="360d9-112">0</span></span>|<span data-ttu-id="360d9-113">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="360d9-113">The device is not registered.</span></span>|
|<span data-ttu-id="360d9-114">inscreve</span><span class="sxs-lookup"><span data-stu-id="360d9-114">registered</span></span>|<span data-ttu-id="360d9-115">duas</span><span class="sxs-lookup"><span data-stu-id="360d9-115">2</span></span>|<span data-ttu-id="360d9-116">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="360d9-116">The device is registered.</span></span>|
|<span data-ttu-id="360d9-117">revogado</span><span class="sxs-lookup"><span data-stu-id="360d9-117">revoked</span></span>|<span data-ttu-id="360d9-118">3D</span><span class="sxs-lookup"><span data-stu-id="360d9-118">3</span></span>|<span data-ttu-id="360d9-119">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="360d9-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="360d9-120">keyconflict</span><span class="sxs-lookup"><span data-stu-id="360d9-120">keyConflict</span></span>|<span data-ttu-id="360d9-121">4 </span><span class="sxs-lookup"><span data-stu-id="360d9-121">4</span></span>|<span data-ttu-id="360d9-122">O dispositivo tem um conflito de teclas.</span><span class="sxs-lookup"><span data-stu-id="360d9-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="360d9-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="360d9-123">approvalPending</span></span>|<span data-ttu-id="360d9-124">5 </span><span class="sxs-lookup"><span data-stu-id="360d9-124">5</span></span>|<span data-ttu-id="360d9-125">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="360d9-125">The device is pending approval.</span></span>|
|<span data-ttu-id="360d9-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="360d9-126">certificateReset</span></span>|<span data-ttu-id="360d9-127">6 </span><span class="sxs-lookup"><span data-stu-id="360d9-127">6</span></span>|<span data-ttu-id="360d9-128">O certificado de dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="360d9-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="360d9-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="360d9-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="360d9-130">7 </span><span class="sxs-lookup"><span data-stu-id="360d9-130">7</span></span>|<span data-ttu-id="360d9-131">O dispositivo não está registrado e registro pendente.</span><span class="sxs-lookup"><span data-stu-id="360d9-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="360d9-132">desconhecido</span><span class="sxs-lookup"><span data-stu-id="360d9-132">unknown</span></span>|<span data-ttu-id="360d9-133">8 </span><span class="sxs-lookup"><span data-stu-id="360d9-133">8</span></span>|<span data-ttu-id="360d9-134">O status do registro do dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="360d9-134">The device registration status is unknown.</span></span>|



