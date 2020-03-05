---
title: tipo de enumeração deviceEnrollmentFailureReason
description: Categorias de falha de nível superior para registro.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3241e801eb57cc517f1ab8c3b5acb49587cf7152
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447756"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="885e1-103">tipo de enumeração deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="885e1-103">deviceEnrollmentFailureReason enum type</span></span>

<span data-ttu-id="885e1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="885e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="885e1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="885e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="885e1-106">Categorias de falha de nível superior para registro.</span><span class="sxs-lookup"><span data-stu-id="885e1-106">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="885e1-107">Membros</span><span class="sxs-lookup"><span data-stu-id="885e1-107">Members</span></span>
|<span data-ttu-id="885e1-108">Membro</span><span class="sxs-lookup"><span data-stu-id="885e1-108">Member</span></span>|<span data-ttu-id="885e1-109">Valor</span><span class="sxs-lookup"><span data-stu-id="885e1-109">Value</span></span>|<span data-ttu-id="885e1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="885e1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="885e1-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="885e1-111">unknown</span></span>|<span data-ttu-id="885e1-112">,0</span><span class="sxs-lookup"><span data-stu-id="885e1-112">0</span></span>|<span data-ttu-id="885e1-113">O valor padrão, motivo da falha é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="885e1-113">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="885e1-114">autentica</span><span class="sxs-lookup"><span data-stu-id="885e1-114">authentication</span></span>|<span data-ttu-id="885e1-115">1 </span><span class="sxs-lookup"><span data-stu-id="885e1-115">1</span></span>|<span data-ttu-id="885e1-116">Falha de autenticação</span><span class="sxs-lookup"><span data-stu-id="885e1-116">Authentication failed</span></span>|
|<span data-ttu-id="885e1-117">nesse</span><span class="sxs-lookup"><span data-stu-id="885e1-117">authorization</span></span>|<span data-ttu-id="885e1-118">2 </span><span class="sxs-lookup"><span data-stu-id="885e1-118">2</span></span>|<span data-ttu-id="885e1-119">A chamada foi autenticada, mas não está autorizada a se inscrever.</span><span class="sxs-lookup"><span data-stu-id="885e1-119">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="885e1-120">accountValidation</span><span class="sxs-lookup"><span data-stu-id="885e1-120">accountValidation</span></span>|<span data-ttu-id="885e1-121">3 </span><span class="sxs-lookup"><span data-stu-id="885e1-121">3</span></span>|<span data-ttu-id="885e1-122">Falha ao validar a conta para registro.</span><span class="sxs-lookup"><span data-stu-id="885e1-122">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="885e1-123">(Conta bloqueada, registro não habilitado)</span><span class="sxs-lookup"><span data-stu-id="885e1-123">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="885e1-124">uservalidation</span><span class="sxs-lookup"><span data-stu-id="885e1-124">userValidation</span></span>|<span data-ttu-id="885e1-125">4 </span><span class="sxs-lookup"><span data-stu-id="885e1-125">4</span></span>|<span data-ttu-id="885e1-126">Não foi possível validar o usuário.</span><span class="sxs-lookup"><span data-stu-id="885e1-126">User could not be validated.</span></span> <span data-ttu-id="885e1-127">(O usuário não existe, licença ausente)</span><span class="sxs-lookup"><span data-stu-id="885e1-127">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="885e1-128">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="885e1-128">deviceNotSupported</span></span>|<span data-ttu-id="885e1-129">5 </span><span class="sxs-lookup"><span data-stu-id="885e1-129">5</span></span>|<span data-ttu-id="885e1-130">O dispositivo não tem suporte para gerenciamento de dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="885e1-130">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="885e1-131">inmanutenção</span><span class="sxs-lookup"><span data-stu-id="885e1-131">inMaintenance</span></span>|<span data-ttu-id="885e1-132">6 </span><span class="sxs-lookup"><span data-stu-id="885e1-132">6</span></span>|<span data-ttu-id="885e1-133">A conta está em manutenção.</span><span class="sxs-lookup"><span data-stu-id="885e1-133">Account is in maintenance.</span></span>|
|<span data-ttu-id="885e1-134">badRequest</span><span class="sxs-lookup"><span data-stu-id="885e1-134">badRequest</span></span>|<span data-ttu-id="885e1-135">7 </span><span class="sxs-lookup"><span data-stu-id="885e1-135">7</span></span>|<span data-ttu-id="885e1-136">O cliente enviou uma solicitação que não é compreendida/suportada pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="885e1-136">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="885e1-137">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="885e1-137">featureNotSupported</span></span>|<span data-ttu-id="885e1-138">8 </span><span class="sxs-lookup"><span data-stu-id="885e1-138">8</span></span>|<span data-ttu-id="885e1-139">Não há suporte para os recursos usados por este registro para esta conta.</span><span class="sxs-lookup"><span data-stu-id="885e1-139">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="885e1-140">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="885e1-140">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="885e1-141">9 </span><span class="sxs-lookup"><span data-stu-id="885e1-141">9</span></span>|<span data-ttu-id="885e1-142">As restrições de registro configuradas pelo administrador bloquearam esse registro.</span><span class="sxs-lookup"><span data-stu-id="885e1-142">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="885e1-143">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="885e1-143">clientDisconnected</span></span>|<span data-ttu-id="885e1-144">10 </span><span class="sxs-lookup"><span data-stu-id="885e1-144">10</span></span>|<span data-ttu-id="885e1-145">O cliente esgotou o tempo limite ou o registro foi anulado pelo enduser.</span><span class="sxs-lookup"><span data-stu-id="885e1-145">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="885e1-146">Membrouserabandonment</span><span class="sxs-lookup"><span data-stu-id="885e1-146">userAbandonment</span></span>|<span data-ttu-id="885e1-147">11 </span><span class="sxs-lookup"><span data-stu-id="885e1-147">11</span></span>|<span data-ttu-id="885e1-148">O registro foi abandonado pelo enduser.</span><span class="sxs-lookup"><span data-stu-id="885e1-148">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="885e1-149">(Enduser Started onboard, mas não conseguiu concluí-la na forma oportuna)</span><span class="sxs-lookup"><span data-stu-id="885e1-149">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->


