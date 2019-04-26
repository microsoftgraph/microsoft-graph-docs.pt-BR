---
title: tipo de enumeração deviceEnrollmentFailureReason
description: Categorias de falha de nível superior para registro.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 623030bccfac9e023a0d1df2dff7ea317b503485
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571832"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="75b85-103">tipo de enumeração deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="75b85-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="75b85-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75b85-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75b85-105">Categorias de falha de nível superior para registro.</span><span class="sxs-lookup"><span data-stu-id="75b85-105">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="75b85-106">Membros</span><span class="sxs-lookup"><span data-stu-id="75b85-106">Members</span></span>
|<span data-ttu-id="75b85-107">Membro</span><span class="sxs-lookup"><span data-stu-id="75b85-107">Member</span></span>|<span data-ttu-id="75b85-108">Valor</span><span class="sxs-lookup"><span data-stu-id="75b85-108">Value</span></span>|<span data-ttu-id="75b85-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="75b85-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75b85-110">desconhecido</span><span class="sxs-lookup"><span data-stu-id="75b85-110">unknown</span></span>|<span data-ttu-id="75b85-111">,0</span><span class="sxs-lookup"><span data-stu-id="75b85-111">0</span></span>|<span data-ttu-id="75b85-112">O valor padrão, motivo da falha é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="75b85-112">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="75b85-113">autentica</span><span class="sxs-lookup"><span data-stu-id="75b85-113">authentication</span></span>|<span data-ttu-id="75b85-114">1 </span><span class="sxs-lookup"><span data-stu-id="75b85-114">1</span></span>|<span data-ttu-id="75b85-115">Falha de autenticação</span><span class="sxs-lookup"><span data-stu-id="75b85-115">Authentication failed</span></span>|
|<span data-ttu-id="75b85-116">nesse</span><span class="sxs-lookup"><span data-stu-id="75b85-116">authorization</span></span>|<span data-ttu-id="75b85-117">2 </span><span class="sxs-lookup"><span data-stu-id="75b85-117">2</span></span>|<span data-ttu-id="75b85-118">A chamada foi autenticada, mas não está autorizada a se inscrever.</span><span class="sxs-lookup"><span data-stu-id="75b85-118">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="75b85-119">accountValidation</span><span class="sxs-lookup"><span data-stu-id="75b85-119">accountValidation</span></span>|<span data-ttu-id="75b85-120">3 </span><span class="sxs-lookup"><span data-stu-id="75b85-120">3</span></span>|<span data-ttu-id="75b85-121">Falha ao validar a conta para registro.</span><span class="sxs-lookup"><span data-stu-id="75b85-121">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="75b85-122">(Conta bloqueada, registro não habilitado)</span><span class="sxs-lookup"><span data-stu-id="75b85-122">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="75b85-123">userValidation</span><span class="sxs-lookup"><span data-stu-id="75b85-123">userValidation</span></span>|<span data-ttu-id="75b85-124">4 </span><span class="sxs-lookup"><span data-stu-id="75b85-124">4</span></span>|<span data-ttu-id="75b85-125">Não foi possível validar o usuário.</span><span class="sxs-lookup"><span data-stu-id="75b85-125">User could not be validated.</span></span> <span data-ttu-id="75b85-126">(O usuário não existe, licença ausente)</span><span class="sxs-lookup"><span data-stu-id="75b85-126">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="75b85-127">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="75b85-127">deviceNotSupported</span></span>|<span data-ttu-id="75b85-128">5 </span><span class="sxs-lookup"><span data-stu-id="75b85-128">5</span></span>|<span data-ttu-id="75b85-129">O dispositivo não tem suporte para gerenciamento de dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="75b85-129">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="75b85-130">inManutenção</span><span class="sxs-lookup"><span data-stu-id="75b85-130">inMaintenance</span></span>|<span data-ttu-id="75b85-131">6 </span><span class="sxs-lookup"><span data-stu-id="75b85-131">6</span></span>|<span data-ttu-id="75b85-132">A conta está em manutenção.</span><span class="sxs-lookup"><span data-stu-id="75b85-132">Account is in maintenance.</span></span>|
|<span data-ttu-id="75b85-133">badRequest</span><span class="sxs-lookup"><span data-stu-id="75b85-133">badRequest</span></span>|<span data-ttu-id="75b85-134">7 </span><span class="sxs-lookup"><span data-stu-id="75b85-134">7</span></span>|<span data-ttu-id="75b85-135">O cliente enviou uma solicitação que não é compreendida/suportada pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="75b85-135">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="75b85-136">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="75b85-136">featureNotSupported</span></span>|<span data-ttu-id="75b85-137">8 </span><span class="sxs-lookup"><span data-stu-id="75b85-137">8</span></span>|<span data-ttu-id="75b85-138">Não há suporte para os recursos usados por este registro para esta conta.</span><span class="sxs-lookup"><span data-stu-id="75b85-138">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="75b85-139">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="75b85-139">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="75b85-140">9 </span><span class="sxs-lookup"><span data-stu-id="75b85-140">9</span></span>|<span data-ttu-id="75b85-141">As restrições de registro configuradas pelo administrador bloquearam esse registro.</span><span class="sxs-lookup"><span data-stu-id="75b85-141">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="75b85-142">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="75b85-142">clientDisconnected</span></span>|<span data-ttu-id="75b85-143">10 </span><span class="sxs-lookup"><span data-stu-id="75b85-143">10</span></span>|<span data-ttu-id="75b85-144">O cliente esgotou o tempo limite ou o registro foi anulado pelo enduser.</span><span class="sxs-lookup"><span data-stu-id="75b85-144">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="75b85-145">Membrouserabandonment</span><span class="sxs-lookup"><span data-stu-id="75b85-145">userAbandonment</span></span>|<span data-ttu-id="75b85-146">11 </span><span class="sxs-lookup"><span data-stu-id="75b85-146">11</span></span>|<span data-ttu-id="75b85-147">O registro foi abandonado pelo enduser.</span><span class="sxs-lookup"><span data-stu-id="75b85-147">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="75b85-148">(Enduser Started onboard, mas não conseguiu concluí-la na forma oportuna)</span><span class="sxs-lookup"><span data-stu-id="75b85-148">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->

