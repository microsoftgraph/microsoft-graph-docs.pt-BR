---
title: Tipo de número deviceEnrollmentFailureReason
description: Categorias de falha de nível superior para registro.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9ee798d2cd9c21038cff177320b3a3ae37d05f2e
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732217"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="6097f-103">Tipo de número deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="6097f-103">deviceEnrollmentFailureReason enum type</span></span>

<span data-ttu-id="6097f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6097f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6097f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6097f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6097f-106">Categorias de falha de nível superior para registro.</span><span class="sxs-lookup"><span data-stu-id="6097f-106">Top level failure categories for enrollment.</span></span>

## <a name="members"></a><span data-ttu-id="6097f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="6097f-107">Members</span></span>
|<span data-ttu-id="6097f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="6097f-108">Member</span></span>|<span data-ttu-id="6097f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="6097f-109">Value</span></span>|<span data-ttu-id="6097f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6097f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6097f-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="6097f-111">unknown</span></span>|<span data-ttu-id="6097f-112">0</span><span class="sxs-lookup"><span data-stu-id="6097f-112">0</span></span>|<span data-ttu-id="6097f-113">Valor padrão, motivo da falha é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="6097f-113">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="6097f-114">authentication</span><span class="sxs-lookup"><span data-stu-id="6097f-114">authentication</span></span>|<span data-ttu-id="6097f-115">1</span><span class="sxs-lookup"><span data-stu-id="6097f-115">1</span></span>|<span data-ttu-id="6097f-116">Falha na autenticação</span><span class="sxs-lookup"><span data-stu-id="6097f-116">Authentication failed</span></span>|
|<span data-ttu-id="6097f-117">authorization</span><span class="sxs-lookup"><span data-stu-id="6097f-117">authorization</span></span>|<span data-ttu-id="6097f-118">2</span><span class="sxs-lookup"><span data-stu-id="6097f-118">2</span></span>|<span data-ttu-id="6097f-119">A chamada foi autenticada, mas não autorizada a se inscrever.</span><span class="sxs-lookup"><span data-stu-id="6097f-119">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="6097f-120">accountValidation</span><span class="sxs-lookup"><span data-stu-id="6097f-120">accountValidation</span></span>|<span data-ttu-id="6097f-121">3</span><span class="sxs-lookup"><span data-stu-id="6097f-121">3</span></span>|<span data-ttu-id="6097f-122">Falha ao validar a conta para registro.</span><span class="sxs-lookup"><span data-stu-id="6097f-122">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="6097f-123">(Conta bloqueada, registro não habilitado)</span><span class="sxs-lookup"><span data-stu-id="6097f-123">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="6097f-124">userValidation</span><span class="sxs-lookup"><span data-stu-id="6097f-124">userValidation</span></span>|<span data-ttu-id="6097f-125">4 </span><span class="sxs-lookup"><span data-stu-id="6097f-125">4</span></span>|<span data-ttu-id="6097f-126">O usuário não pôde ser validado.</span><span class="sxs-lookup"><span data-stu-id="6097f-126">User could not be validated.</span></span> <span data-ttu-id="6097f-127">(O usuário não existe, licença ausente)</span><span class="sxs-lookup"><span data-stu-id="6097f-127">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="6097f-128">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="6097f-128">deviceNotSupported</span></span>|<span data-ttu-id="6097f-129">5 </span><span class="sxs-lookup"><span data-stu-id="6097f-129">5</span></span>|<span data-ttu-id="6097f-130">Não há suporte para o gerenciamento de dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="6097f-130">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="6097f-131">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="6097f-131">inMaintenance</span></span>|<span data-ttu-id="6097f-132">6 </span><span class="sxs-lookup"><span data-stu-id="6097f-132">6</span></span>|<span data-ttu-id="6097f-133">A conta está em manutenção.</span><span class="sxs-lookup"><span data-stu-id="6097f-133">Account is in maintenance.</span></span>|
|<span data-ttu-id="6097f-134">badRequest</span><span class="sxs-lookup"><span data-stu-id="6097f-134">badRequest</span></span>|<span data-ttu-id="6097f-135">7 </span><span class="sxs-lookup"><span data-stu-id="6097f-135">7</span></span>|<span data-ttu-id="6097f-136">O cliente enviou uma solicitação que não é compreendida/suportada pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="6097f-136">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="6097f-137">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="6097f-137">featureNotSupported</span></span>|<span data-ttu-id="6097f-138">8 </span><span class="sxs-lookup"><span data-stu-id="6097f-138">8</span></span>|<span data-ttu-id="6097f-139">Os recursos usados por esse registro não são suportados para essa conta.</span><span class="sxs-lookup"><span data-stu-id="6097f-139">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="6097f-140">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="6097f-140">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="6097f-141">9 </span><span class="sxs-lookup"><span data-stu-id="6097f-141">9</span></span>|<span data-ttu-id="6097f-142">As restrições de registro configuradas pelo administrador bloquearam esse registro.</span><span class="sxs-lookup"><span data-stu-id="6097f-142">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="6097f-143">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="6097f-143">clientDisconnected</span></span>|<span data-ttu-id="6097f-144">10 </span><span class="sxs-lookup"><span data-stu-id="6097f-144">10</span></span>|<span data-ttu-id="6097f-145">O tempo de término do cliente ou o registro foi abortado pelo usuário final.</span><span class="sxs-lookup"><span data-stu-id="6097f-145">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="6097f-146">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="6097f-146">userAbandonment</span></span>|<span data-ttu-id="6097f-147">11</span><span class="sxs-lookup"><span data-stu-id="6097f-147">11</span></span>|<span data-ttu-id="6097f-148">O registro foi abandonado pelo usuário final.</span><span class="sxs-lookup"><span data-stu-id="6097f-148">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="6097f-149">(O Usuário final começou a integração, mas falhou ao concluí-lo em tempo hábil)</span><span class="sxs-lookup"><span data-stu-id="6097f-149">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->







