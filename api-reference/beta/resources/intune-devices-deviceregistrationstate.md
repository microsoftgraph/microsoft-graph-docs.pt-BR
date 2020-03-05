---
title: tipo de enumeração deviceRegistrationState
description: Status do registro do dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f999e393caab410ea3f7565ade25d189193cfc40
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525023"
---
# <a name="deviceregistrationstate-enum-type"></a><span data-ttu-id="71a8b-103">tipo de enumeração deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="71a8b-103">deviceRegistrationState enum type</span></span>

<span data-ttu-id="71a8b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="71a8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71a8b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71a8b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71a8b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71a8b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71a8b-107">Status do registro do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="71a8b-107">Device registration status.</span></span>

## <a name="members"></a><span data-ttu-id="71a8b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="71a8b-108">Members</span></span>
|<span data-ttu-id="71a8b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="71a8b-109">Member</span></span>|<span data-ttu-id="71a8b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="71a8b-110">Value</span></span>|<span data-ttu-id="71a8b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="71a8b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71a8b-112">Não registrado</span><span class="sxs-lookup"><span data-stu-id="71a8b-112">notRegistered</span></span>|<span data-ttu-id="71a8b-113">,0</span><span class="sxs-lookup"><span data-stu-id="71a8b-113">0</span></span>|<span data-ttu-id="71a8b-114">O dispositivo não está registrado.</span><span class="sxs-lookup"><span data-stu-id="71a8b-114">The device is not registered.</span></span>|
|<span data-ttu-id="71a8b-115">inscreve</span><span class="sxs-lookup"><span data-stu-id="71a8b-115">registered</span></span>|<span data-ttu-id="71a8b-116">2 </span><span class="sxs-lookup"><span data-stu-id="71a8b-116">2</span></span>|<span data-ttu-id="71a8b-117">O dispositivo está registrado.</span><span class="sxs-lookup"><span data-stu-id="71a8b-117">The device is registered.</span></span>|
|<span data-ttu-id="71a8b-118">revogado</span><span class="sxs-lookup"><span data-stu-id="71a8b-118">revoked</span></span>|<span data-ttu-id="71a8b-119">3 </span><span class="sxs-lookup"><span data-stu-id="71a8b-119">3</span></span>|<span data-ttu-id="71a8b-120">O dispositivo foi bloqueado, apagado ou desativado.</span><span class="sxs-lookup"><span data-stu-id="71a8b-120">The device has been blocked, wiped or retired.</span></span>|
|<span data-ttu-id="71a8b-121">keyconflict</span><span class="sxs-lookup"><span data-stu-id="71a8b-121">keyConflict</span></span>|<span data-ttu-id="71a8b-122">4 </span><span class="sxs-lookup"><span data-stu-id="71a8b-122">4</span></span>|<span data-ttu-id="71a8b-123">O dispositivo tem um conflito de teclas.</span><span class="sxs-lookup"><span data-stu-id="71a8b-123">The device has a key conflict.</span></span>|
|<span data-ttu-id="71a8b-124">approvalPending</span><span class="sxs-lookup"><span data-stu-id="71a8b-124">approvalPending</span></span>|<span data-ttu-id="71a8b-125">5 </span><span class="sxs-lookup"><span data-stu-id="71a8b-125">5</span></span>|<span data-ttu-id="71a8b-126">O dispositivo está aguardando aprovação.</span><span class="sxs-lookup"><span data-stu-id="71a8b-126">The device is pending approval.</span></span>|
|<span data-ttu-id="71a8b-127">certificateReset</span><span class="sxs-lookup"><span data-stu-id="71a8b-127">certificateReset</span></span>|<span data-ttu-id="71a8b-128">6 </span><span class="sxs-lookup"><span data-stu-id="71a8b-128">6</span></span>|<span data-ttu-id="71a8b-129">O certificado de dispositivo foi redefinido.</span><span class="sxs-lookup"><span data-stu-id="71a8b-129">The device certificate has been reset.</span></span>|
|<span data-ttu-id="71a8b-130">notRegisteredPendingEnrollment</span><span class="sxs-lookup"><span data-stu-id="71a8b-130">notRegisteredPendingEnrollment</span></span>|<span data-ttu-id="71a8b-131">7 </span><span class="sxs-lookup"><span data-stu-id="71a8b-131">7</span></span>|<span data-ttu-id="71a8b-132">O dispositivo não está registrado e registro pendente.</span><span class="sxs-lookup"><span data-stu-id="71a8b-132">The device is not registered and pending enrollment.</span></span>|
|<span data-ttu-id="71a8b-133">desconhecido</span><span class="sxs-lookup"><span data-stu-id="71a8b-133">unknown</span></span>|<span data-ttu-id="71a8b-134">8 </span><span class="sxs-lookup"><span data-stu-id="71a8b-134">8</span></span>|<span data-ttu-id="71a8b-135">O status do registro do dispositivo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="71a8b-135">The device registration status is unknown.</span></span>|



