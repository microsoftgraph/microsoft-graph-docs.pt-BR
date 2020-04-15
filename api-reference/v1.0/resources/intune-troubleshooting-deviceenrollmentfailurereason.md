---
title: tipo de enumeração deviceEnrollmentFailureReason
description: Categorias de falha de nível superior para registro.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fefe8adf226f99a239bd9a04331596861237c0ad
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445550"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="e95c7-103">tipo de enumeração deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="e95c7-103">deviceEnrollmentFailureReason enum type</span></span>

<span data-ttu-id="e95c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e95c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e95c7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e95c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e95c7-106">Categorias de falha de nível superior para registro.</span><span class="sxs-lookup"><span data-stu-id="e95c7-106">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="e95c7-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e95c7-107">Members</span></span>
|<span data-ttu-id="e95c7-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e95c7-108">Member</span></span>|<span data-ttu-id="e95c7-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e95c7-109">Value</span></span>|<span data-ttu-id="e95c7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e95c7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e95c7-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="e95c7-111">unknown</span></span>|<span data-ttu-id="e95c7-112">,0</span><span class="sxs-lookup"><span data-stu-id="e95c7-112">0</span></span>|<span data-ttu-id="e95c7-113">O valor padrão, motivo da falha é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="e95c7-113">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="e95c7-114">autentica</span><span class="sxs-lookup"><span data-stu-id="e95c7-114">authentication</span></span>|<span data-ttu-id="e95c7-115">1</span><span class="sxs-lookup"><span data-stu-id="e95c7-115">1</span></span>|<span data-ttu-id="e95c7-116">Falha de autenticação</span><span class="sxs-lookup"><span data-stu-id="e95c7-116">Authentication failed</span></span>|
|<span data-ttu-id="e95c7-117">nesse</span><span class="sxs-lookup"><span data-stu-id="e95c7-117">authorization</span></span>|<span data-ttu-id="e95c7-118">duas</span><span class="sxs-lookup"><span data-stu-id="e95c7-118">2</span></span>|<span data-ttu-id="e95c7-119">A chamada foi autenticada, mas não está autorizada a se inscrever.</span><span class="sxs-lookup"><span data-stu-id="e95c7-119">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="e95c7-120">accountValidation</span><span class="sxs-lookup"><span data-stu-id="e95c7-120">accountValidation</span></span>|<span data-ttu-id="e95c7-121">3D</span><span class="sxs-lookup"><span data-stu-id="e95c7-121">3</span></span>|<span data-ttu-id="e95c7-122">Falha ao validar a conta para registro.</span><span class="sxs-lookup"><span data-stu-id="e95c7-122">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="e95c7-123">(Conta bloqueada, registro não habilitado)</span><span class="sxs-lookup"><span data-stu-id="e95c7-123">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="e95c7-124">uservalidation</span><span class="sxs-lookup"><span data-stu-id="e95c7-124">userValidation</span></span>|<span data-ttu-id="e95c7-125">4 </span><span class="sxs-lookup"><span data-stu-id="e95c7-125">4</span></span>|<span data-ttu-id="e95c7-126">Não foi possível validar o usuário.</span><span class="sxs-lookup"><span data-stu-id="e95c7-126">User could not be validated.</span></span> <span data-ttu-id="e95c7-127">(O usuário não existe, licença ausente)</span><span class="sxs-lookup"><span data-stu-id="e95c7-127">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="e95c7-128">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="e95c7-128">deviceNotSupported</span></span>|<span data-ttu-id="e95c7-129">5 </span><span class="sxs-lookup"><span data-stu-id="e95c7-129">5</span></span>|<span data-ttu-id="e95c7-130">O dispositivo não tem suporte para gerenciamento de dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="e95c7-130">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="e95c7-131">inmanutenção</span><span class="sxs-lookup"><span data-stu-id="e95c7-131">inMaintenance</span></span>|<span data-ttu-id="e95c7-132">6 </span><span class="sxs-lookup"><span data-stu-id="e95c7-132">6</span></span>|<span data-ttu-id="e95c7-133">A conta está em manutenção.</span><span class="sxs-lookup"><span data-stu-id="e95c7-133">Account is in maintenance.</span></span>|
|<span data-ttu-id="e95c7-134">badRequest</span><span class="sxs-lookup"><span data-stu-id="e95c7-134">badRequest</span></span>|<span data-ttu-id="e95c7-135">7 </span><span class="sxs-lookup"><span data-stu-id="e95c7-135">7</span></span>|<span data-ttu-id="e95c7-136">O cliente enviou uma solicitação que não é compreendida/suportada pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="e95c7-136">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="e95c7-137">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="e95c7-137">featureNotSupported</span></span>|<span data-ttu-id="e95c7-138">8 </span><span class="sxs-lookup"><span data-stu-id="e95c7-138">8</span></span>|<span data-ttu-id="e95c7-139">Não há suporte para os recursos usados por este registro para esta conta.</span><span class="sxs-lookup"><span data-stu-id="e95c7-139">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="e95c7-140">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="e95c7-140">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="e95c7-141">9 </span><span class="sxs-lookup"><span data-stu-id="e95c7-141">9</span></span>|<span data-ttu-id="e95c7-142">As restrições de registro configuradas pelo administrador bloquearam esse registro.</span><span class="sxs-lookup"><span data-stu-id="e95c7-142">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="e95c7-143">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="e95c7-143">clientDisconnected</span></span>|<span data-ttu-id="e95c7-144">10 </span><span class="sxs-lookup"><span data-stu-id="e95c7-144">10</span></span>|<span data-ttu-id="e95c7-145">O cliente esgotou o tempo limite ou o registro foi anulado pelo enduser.</span><span class="sxs-lookup"><span data-stu-id="e95c7-145">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="e95c7-146">Membrouserabandonment</span><span class="sxs-lookup"><span data-stu-id="e95c7-146">userAbandonment</span></span>|<span data-ttu-id="e95c7-147">11</span><span class="sxs-lookup"><span data-stu-id="e95c7-147">11</span></span>|<span data-ttu-id="e95c7-148">O registro foi abandonado pelo enduser.</span><span class="sxs-lookup"><span data-stu-id="e95c7-148">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="e95c7-149">(Enduser Started onboard, mas não conseguiu concluí-la na forma oportuna)</span><span class="sxs-lookup"><span data-stu-id="e95c7-149">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->





