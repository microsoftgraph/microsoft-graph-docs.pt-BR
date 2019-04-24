---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b777452b627208d8e2dd726815f321075e5745ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522381"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="a9e71-103">tipo de enumeração deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="a9e71-103">deviceRegistrationState enum type</span></span>

> <span data-ttu-id="a9e71-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9e71-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9e71-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9e71-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9e71-106">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a9e71-106">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="a9e71-107">Membros</span><span class="sxs-lookup"><span data-stu-id="a9e71-107">Members</span></span>
|<span data-ttu-id="a9e71-108">Membro</span><span class="sxs-lookup"><span data-stu-id="a9e71-108">Member</span></span>|<span data-ttu-id="a9e71-109">Valor</span><span class="sxs-lookup"><span data-stu-id="a9e71-109">Value</span></span>|<span data-ttu-id="a9e71-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9e71-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9e71-111">Não registrado</span><span class="sxs-lookup"><span data-stu-id="a9e71-111">notRegistered</span></span>|<span data-ttu-id="a9e71-112">,0</span><span class="sxs-lookup"><span data-stu-id="a9e71-112">0</span></span>|<span data-ttu-id="a9e71-113">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="a9e71-113">The device is not registered.</span></span>|
|<span data-ttu-id="a9e71-114">inscreve</span><span class="sxs-lookup"><span data-stu-id="a9e71-114">registered</span></span>|<span data-ttu-id="a9e71-115">2 </span><span class="sxs-lookup"><span data-stu-id="a9e71-115">2</span></span>|<span data-ttu-id="a9e71-116">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="a9e71-116">The device is registered.</span></span>|
|<span data-ttu-id="a9e71-117">revogado</span><span class="sxs-lookup"><span data-stu-id="a9e71-117">revoked</span></span>|<span data-ttu-id="a9e71-118">3 </span><span class="sxs-lookup"><span data-stu-id="a9e71-118">3</span></span>|<span data-ttu-id="a9e71-119">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="a9e71-119">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="a9e71-120">keyConflict</span><span class="sxs-lookup"><span data-stu-id="a9e71-120">keyConflict</span></span>|<span data-ttu-id="a9e71-121">4 </span><span class="sxs-lookup"><span data-stu-id="a9e71-121">4</span></span>|<span data-ttu-id="a9e71-122">O dispositivo tem um conflito de teclas.</span><span class="sxs-lookup"><span data-stu-id="a9e71-122">The device has a key conflict.</span></span>|
|<span data-ttu-id="a9e71-123">approvalPending</span><span class="sxs-lookup"><span data-stu-id="a9e71-123">approvalPending</span></span>|<span data-ttu-id="a9e71-124">5 </span><span class="sxs-lookup"><span data-stu-id="a9e71-124">5</span></span>|<span data-ttu-id="a9e71-125">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="a9e71-125">The device is pending approval.</span></span>|
|<span data-ttu-id="a9e71-126">certificateReset</span><span class="sxs-lookup"><span data-stu-id="a9e71-126">certificateReset</span></span>|<span data-ttu-id="a9e71-127">6 </span><span class="sxs-lookup"><span data-stu-id="a9e71-127">6</span></span>|<span data-ttu-id="a9e71-128">O certificado de dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="a9e71-128">The device certificate has been reset.</span></span>|
|<span data-ttu-id="a9e71-129">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="a9e71-129">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="a9e71-130">7 </span><span class="sxs-lookup"><span data-stu-id="a9e71-130">7</span></span>|<span data-ttu-id="a9e71-131">O dispositivo não está registrado e registro pendente.</span><span class="sxs-lookup"><span data-stu-id="a9e71-131">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="a9e71-132">desconhecido</span><span class="sxs-lookup"><span data-stu-id="a9e71-132">unknown</span></span>|<span data-ttu-id="a9e71-133">8 </span><span class="sxs-lookup"><span data-stu-id="a9e71-133">8</span></span>|<span data-ttu-id="a9e71-134">O status do registro do dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="a9e71-134">The device registration status is unknown.</span></span>|





