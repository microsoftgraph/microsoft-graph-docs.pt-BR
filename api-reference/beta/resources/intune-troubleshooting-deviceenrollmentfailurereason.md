---
title: tipo de enumeração deviceEnrollmentFailureReason
description: Categorias de falha de nível superior para registro.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4d975f554c426bf8050b5603b0b4fb1d2297f8b2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255375"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="0a890-103">tipo de enumeração deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="0a890-103">deviceEnrollmentFailureReason enum type</span></span>

<span data-ttu-id="0a890-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a890-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a890-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0a890-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a890-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a890-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a890-107">Categorias de falha de nível superior para registro.</span><span class="sxs-lookup"><span data-stu-id="0a890-107">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="0a890-108">Membros</span><span class="sxs-lookup"><span data-stu-id="0a890-108">Members</span></span>
|<span data-ttu-id="0a890-109">Membro</span><span class="sxs-lookup"><span data-stu-id="0a890-109">Member</span></span>|<span data-ttu-id="0a890-110">Valor</span><span class="sxs-lookup"><span data-stu-id="0a890-110">Value</span></span>|<span data-ttu-id="0a890-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a890-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a890-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="0a890-112">unknown</span></span>|<span data-ttu-id="0a890-113">,0</span><span class="sxs-lookup"><span data-stu-id="0a890-113">0</span></span>|<span data-ttu-id="0a890-114">O valor padrão, motivo da falha é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="0a890-114">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="0a890-115">autentica</span><span class="sxs-lookup"><span data-stu-id="0a890-115">authentication</span></span>|<span data-ttu-id="0a890-116">1</span><span class="sxs-lookup"><span data-stu-id="0a890-116">1</span></span>|<span data-ttu-id="0a890-117">Falha de autenticação</span><span class="sxs-lookup"><span data-stu-id="0a890-117">Authentication failed</span></span>|
|<span data-ttu-id="0a890-118">nesse</span><span class="sxs-lookup"><span data-stu-id="0a890-118">authorization</span></span>|<span data-ttu-id="0a890-119">duas</span><span class="sxs-lookup"><span data-stu-id="0a890-119">2</span></span>|<span data-ttu-id="0a890-120">A chamada foi autenticada, mas não está autorizada a se inscrever.</span><span class="sxs-lookup"><span data-stu-id="0a890-120">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="0a890-121">accountValidation</span><span class="sxs-lookup"><span data-stu-id="0a890-121">accountValidation</span></span>|<span data-ttu-id="0a890-122">3D</span><span class="sxs-lookup"><span data-stu-id="0a890-122">3</span></span>|<span data-ttu-id="0a890-123">Falha ao validar a conta para registro.</span><span class="sxs-lookup"><span data-stu-id="0a890-123">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="0a890-124">(Conta bloqueada, registro não habilitado)</span><span class="sxs-lookup"><span data-stu-id="0a890-124">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="0a890-125">uservalidation</span><span class="sxs-lookup"><span data-stu-id="0a890-125">userValidation</span></span>|<span data-ttu-id="0a890-126">4 </span><span class="sxs-lookup"><span data-stu-id="0a890-126">4</span></span>|<span data-ttu-id="0a890-127">Não foi possível validar o usuário.</span><span class="sxs-lookup"><span data-stu-id="0a890-127">User could not be validated.</span></span> <span data-ttu-id="0a890-128">(O usuário não existe, licença ausente)</span><span class="sxs-lookup"><span data-stu-id="0a890-128">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="0a890-129">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="0a890-129">deviceNotSupported</span></span>|<span data-ttu-id="0a890-130">5 </span><span class="sxs-lookup"><span data-stu-id="0a890-130">5</span></span>|<span data-ttu-id="0a890-131">O dispositivo não tem suporte para gerenciamento de dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="0a890-131">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="0a890-132">inmanutenção</span><span class="sxs-lookup"><span data-stu-id="0a890-132">inMaintenance</span></span>|<span data-ttu-id="0a890-133">6 </span><span class="sxs-lookup"><span data-stu-id="0a890-133">6</span></span>|<span data-ttu-id="0a890-134">A conta está em manutenção.</span><span class="sxs-lookup"><span data-stu-id="0a890-134">Account is in maintenance.</span></span>|
|<span data-ttu-id="0a890-135">badRequest</span><span class="sxs-lookup"><span data-stu-id="0a890-135">badRequest</span></span>|<span data-ttu-id="0a890-136">7 </span><span class="sxs-lookup"><span data-stu-id="0a890-136">7</span></span>|<span data-ttu-id="0a890-137">O cliente enviou uma solicitação que não é compreendida/suportada pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="0a890-137">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="0a890-138">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="0a890-138">featureNotSupported</span></span>|<span data-ttu-id="0a890-139">8 </span><span class="sxs-lookup"><span data-stu-id="0a890-139">8</span></span>|<span data-ttu-id="0a890-140">Não há suporte para os recursos usados por este registro para esta conta.</span><span class="sxs-lookup"><span data-stu-id="0a890-140">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="0a890-141">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="0a890-141">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="0a890-142">9 </span><span class="sxs-lookup"><span data-stu-id="0a890-142">9</span></span>|<span data-ttu-id="0a890-143">As restrições de registro configuradas pelo administrador bloquearam esse registro.</span><span class="sxs-lookup"><span data-stu-id="0a890-143">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="0a890-144">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="0a890-144">clientDisconnected</span></span>|<span data-ttu-id="0a890-145">10 </span><span class="sxs-lookup"><span data-stu-id="0a890-145">10</span></span>|<span data-ttu-id="0a890-146">O cliente esgotou o tempo limite ou o registro foi anulado pelo enduser.</span><span class="sxs-lookup"><span data-stu-id="0a890-146">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="0a890-147">Membrouserabandonment</span><span class="sxs-lookup"><span data-stu-id="0a890-147">userAbandonment</span></span>|<span data-ttu-id="0a890-148">11 </span><span class="sxs-lookup"><span data-stu-id="0a890-148">11</span></span>|<span data-ttu-id="0a890-149">O registro foi abandonado pelo enduser.</span><span class="sxs-lookup"><span data-stu-id="0a890-149">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="0a890-150">(Enduser Started onboard, mas não conseguiu concluí-la na forma oportuna)</span><span class="sxs-lookup"><span data-stu-id="0a890-150">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|




