---
title: tipo de enumeração deviceEnrollmentFailureReason
description: Categorias de falha de nível superior para registro.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7a0721495a8eb217007c0ee1f18942009614696d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010312"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="e4e1b-103">tipo de enumeração deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="e4e1b-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="e4e1b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4e1b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4e1b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4e1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4e1b-106">Categorias de falha de nível superior para registro.</span><span class="sxs-lookup"><span data-stu-id="e4e1b-106">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="e4e1b-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e4e1b-107">Members</span></span>
|<span data-ttu-id="e4e1b-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e4e1b-108">Member</span></span>|<span data-ttu-id="e4e1b-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e4e1b-109">Value</span></span>|<span data-ttu-id="e4e1b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4e1b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4e1b-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="e4e1b-111">unknown</span></span>|<span data-ttu-id="e4e1b-112">,0</span><span class="sxs-lookup"><span data-stu-id="e4e1b-112">0</span></span>|<span data-ttu-id="e4e1b-113">O valor padrão, motivo da falha é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="e4e1b-113">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="e4e1b-114">autentica</span><span class="sxs-lookup"><span data-stu-id="e4e1b-114">authentication</span></span>|<span data-ttu-id="e4e1b-115">1</span><span class="sxs-lookup"><span data-stu-id="e4e1b-115">1</span></span>|<span data-ttu-id="e4e1b-116">Falha de autenticação</span><span class="sxs-lookup"><span data-stu-id="e4e1b-116">Authentication failed</span></span>|
|<span data-ttu-id="e4e1b-117">nesse</span><span class="sxs-lookup"><span data-stu-id="e4e1b-117">authorization</span></span>|<span data-ttu-id="e4e1b-118">duas</span><span class="sxs-lookup"><span data-stu-id="e4e1b-118">2</span></span>|<span data-ttu-id="e4e1b-119">A chamada foi autenticada, mas não está autorizada a se inscrever.</span><span class="sxs-lookup"><span data-stu-id="e4e1b-119">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="e4e1b-120">accountValidation</span><span class="sxs-lookup"><span data-stu-id="e4e1b-120">accountValidation</span></span>|<span data-ttu-id="e4e1b-121">3D</span><span class="sxs-lookup"><span data-stu-id="e4e1b-121">3</span></span>|<span data-ttu-id="e4e1b-122">Falha ao validar a conta para registro.</span><span class="sxs-lookup"><span data-stu-id="e4e1b-122">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="e4e1b-123">(Conta bloqueada, registro não habilitado)</span><span class="sxs-lookup"><span data-stu-id="e4e1b-123">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="e4e1b-124">uservalidation</span><span class="sxs-lookup"><span data-stu-id="e4e1b-124">userValidation</span></span>|<span data-ttu-id="e4e1b-125">quatro</span><span class="sxs-lookup"><span data-stu-id="e4e1b-125">4</span></span>|<span data-ttu-id="e4e1b-126">Não foi possível validar o usuário.</span><span class="sxs-lookup"><span data-stu-id="e4e1b-126">User could not be validated.</span></span> <span data-ttu-id="e4e1b-127">(O usuário não existe, licença ausente)</span><span class="sxs-lookup"><span data-stu-id="e4e1b-127">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="e4e1b-128">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="e4e1b-128">deviceNotSupported</span></span>|<span data-ttu-id="e4e1b-129">0,5</span><span class="sxs-lookup"><span data-stu-id="e4e1b-129">5</span></span>|<span data-ttu-id="e4e1b-130">O dispositivo não tem suporte para gerenciamento de dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="e4e1b-130">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="e4e1b-131">inmanutenção</span><span class="sxs-lookup"><span data-stu-id="e4e1b-131">inMaintenance</span></span>|<span data-ttu-id="e4e1b-132">6</span><span class="sxs-lookup"><span data-stu-id="e4e1b-132">6</span></span>|<span data-ttu-id="e4e1b-133">A conta está em manutenção.</span><span class="sxs-lookup"><span data-stu-id="e4e1b-133">Account is in maintenance.</span></span>|
|<span data-ttu-id="e4e1b-134">badRequest</span><span class="sxs-lookup"><span data-stu-id="e4e1b-134">badRequest</span></span>|<span data-ttu-id="e4e1b-135">178</span><span class="sxs-lookup"><span data-stu-id="e4e1b-135">7</span></span>|<span data-ttu-id="e4e1b-136">O cliente enviou uma solicitação que não é compreendida/suportada pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="e4e1b-136">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="e4e1b-137">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="e4e1b-137">featureNotSupported</span></span>|<span data-ttu-id="e4e1b-138">8 </span><span class="sxs-lookup"><span data-stu-id="e4e1b-138">8</span></span>|<span data-ttu-id="e4e1b-139">Não há suporte para os recursos usados por este registro para esta conta.</span><span class="sxs-lookup"><span data-stu-id="e4e1b-139">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="e4e1b-140">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="e4e1b-140">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="e4e1b-141">9 </span><span class="sxs-lookup"><span data-stu-id="e4e1b-141">9</span></span>|<span data-ttu-id="e4e1b-142">As restrições de registro configuradas pelo administrador bloquearam esse registro.</span><span class="sxs-lookup"><span data-stu-id="e4e1b-142">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="e4e1b-143">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="e4e1b-143">clientDisconnected</span></span>|<span data-ttu-id="e4e1b-144">10 </span><span class="sxs-lookup"><span data-stu-id="e4e1b-144">10</span></span>|<span data-ttu-id="e4e1b-145">O cliente esgotou o tempo limite ou o registro foi anulado pelo enduser.</span><span class="sxs-lookup"><span data-stu-id="e4e1b-145">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="e4e1b-146">Membrouserabandonment</span><span class="sxs-lookup"><span data-stu-id="e4e1b-146">userAbandonment</span></span>|<span data-ttu-id="e4e1b-147">11</span><span class="sxs-lookup"><span data-stu-id="e4e1b-147">11</span></span>|<span data-ttu-id="e4e1b-148">O registro foi abandonado pelo enduser.</span><span class="sxs-lookup"><span data-stu-id="e4e1b-148">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="e4e1b-149">(Enduser Started onboard, mas não conseguiu concluí-la na forma oportuna)</span><span class="sxs-lookup"><span data-stu-id="e4e1b-149">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|





