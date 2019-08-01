---
title: tipo de enumeração deviceEnrollmentFailureReason
description: Categorias de falha de nível superior para registro.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 742c30da453a8de814dad0a70fae2be2946f1127
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036789"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="dc38f-103">tipo de enumeração deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="dc38f-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="dc38f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc38f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc38f-105">Categorias de falha de nível superior para registro.</span><span class="sxs-lookup"><span data-stu-id="dc38f-105">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="dc38f-106">Membros</span><span class="sxs-lookup"><span data-stu-id="dc38f-106">Members</span></span>
|<span data-ttu-id="dc38f-107">Membro</span><span class="sxs-lookup"><span data-stu-id="dc38f-107">Member</span></span>|<span data-ttu-id="dc38f-108">Valor</span><span class="sxs-lookup"><span data-stu-id="dc38f-108">Value</span></span>|<span data-ttu-id="dc38f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc38f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc38f-110">desconhecido</span><span class="sxs-lookup"><span data-stu-id="dc38f-110">unknown</span></span>|<span data-ttu-id="dc38f-111">,0</span><span class="sxs-lookup"><span data-stu-id="dc38f-111">0</span></span>|<span data-ttu-id="dc38f-112">O valor padrão, motivo da falha é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="dc38f-112">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="dc38f-113">autentica</span><span class="sxs-lookup"><span data-stu-id="dc38f-113">authentication</span></span>|<span data-ttu-id="dc38f-114">1</span><span class="sxs-lookup"><span data-stu-id="dc38f-114">1</span></span>|<span data-ttu-id="dc38f-115">Falha de autenticação</span><span class="sxs-lookup"><span data-stu-id="dc38f-115">Authentication failed</span></span>|
|<span data-ttu-id="dc38f-116">nesse</span><span class="sxs-lookup"><span data-stu-id="dc38f-116">authorization</span></span>|<span data-ttu-id="dc38f-117">duas</span><span class="sxs-lookup"><span data-stu-id="dc38f-117">2</span></span>|<span data-ttu-id="dc38f-118">A chamada foi autenticada, mas não está autorizada a se inscrever.</span><span class="sxs-lookup"><span data-stu-id="dc38f-118">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="dc38f-119">accountValidation</span><span class="sxs-lookup"><span data-stu-id="dc38f-119">accountValidation</span></span>|<span data-ttu-id="dc38f-120">3D</span><span class="sxs-lookup"><span data-stu-id="dc38f-120">3</span></span>|<span data-ttu-id="dc38f-121">Falha ao validar a conta para registro.</span><span class="sxs-lookup"><span data-stu-id="dc38f-121">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="dc38f-122">(Conta bloqueada, registro não habilitado)</span><span class="sxs-lookup"><span data-stu-id="dc38f-122">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="dc38f-123">uservalidation</span><span class="sxs-lookup"><span data-stu-id="dc38f-123">userValidation</span></span>|<span data-ttu-id="dc38f-124">quatro</span><span class="sxs-lookup"><span data-stu-id="dc38f-124">4</span></span>|<span data-ttu-id="dc38f-125">Não foi possível validar o usuário.</span><span class="sxs-lookup"><span data-stu-id="dc38f-125">User could not be validated.</span></span> <span data-ttu-id="dc38f-126">(O usuário não existe, licença ausente)</span><span class="sxs-lookup"><span data-stu-id="dc38f-126">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="dc38f-127">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="dc38f-127">deviceNotSupported</span></span>|<span data-ttu-id="dc38f-128">0,5</span><span class="sxs-lookup"><span data-stu-id="dc38f-128">5</span></span>|<span data-ttu-id="dc38f-129">O dispositivo não tem suporte para gerenciamento de dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="dc38f-129">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="dc38f-130">inmanutenção</span><span class="sxs-lookup"><span data-stu-id="dc38f-130">inMaintenance</span></span>|<span data-ttu-id="dc38f-131">6</span><span class="sxs-lookup"><span data-stu-id="dc38f-131">6</span></span>|<span data-ttu-id="dc38f-132">A conta está em manutenção.</span><span class="sxs-lookup"><span data-stu-id="dc38f-132">Account is in maintenance.</span></span>|
|<span data-ttu-id="dc38f-133">badRequest</span><span class="sxs-lookup"><span data-stu-id="dc38f-133">badRequest</span></span>|<span data-ttu-id="dc38f-134">178</span><span class="sxs-lookup"><span data-stu-id="dc38f-134">7</span></span>|<span data-ttu-id="dc38f-135">O cliente enviou uma solicitação que não é compreendida/suportada pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="dc38f-135">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="dc38f-136">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="dc38f-136">featureNotSupported</span></span>|<span data-ttu-id="dc38f-137">8 </span><span class="sxs-lookup"><span data-stu-id="dc38f-137">8</span></span>|<span data-ttu-id="dc38f-138">Não há suporte para os recursos usados por este registro para esta conta.</span><span class="sxs-lookup"><span data-stu-id="dc38f-138">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="dc38f-139">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="dc38f-139">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="dc38f-140">9 </span><span class="sxs-lookup"><span data-stu-id="dc38f-140">9</span></span>|<span data-ttu-id="dc38f-141">As restrições de registro configuradas pelo administrador bloquearam esse registro.</span><span class="sxs-lookup"><span data-stu-id="dc38f-141">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="dc38f-142">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="dc38f-142">clientDisconnected</span></span>|<span data-ttu-id="dc38f-143">10 </span><span class="sxs-lookup"><span data-stu-id="dc38f-143">10</span></span>|<span data-ttu-id="dc38f-144">O cliente esgotou o tempo limite ou o registro foi anulado pelo enduser.</span><span class="sxs-lookup"><span data-stu-id="dc38f-144">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="dc38f-145">Membrouserabandonment</span><span class="sxs-lookup"><span data-stu-id="dc38f-145">userAbandonment</span></span>|<span data-ttu-id="dc38f-146">11</span><span class="sxs-lookup"><span data-stu-id="dc38f-146">11</span></span>|<span data-ttu-id="dc38f-147">O registro foi abandonado pelo enduser.</span><span class="sxs-lookup"><span data-stu-id="dc38f-147">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="dc38f-148">(Enduser Started onboard, mas não conseguiu concluí-la na forma oportuna)</span><span class="sxs-lookup"><span data-stu-id="dc38f-148">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->

