---
title: tipo de enum deviceEnrollmentFailureReason
description: Categorias de falha de nível superior para o registro.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: efee4e4655d36e7575df9e0ddda508dbbcc473c5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962069"
---
# <a name="deviceenrollmentfailurereason-enum-type"></a><span data-ttu-id="e10b5-103">tipo de enum deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="e10b5-103">deviceEnrollmentFailureReason enum type</span></span>

> <span data-ttu-id="e10b5-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e10b5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e10b5-105">Categorias de falha de nível superior para o registro.</span><span class="sxs-lookup"><span data-stu-id="e10b5-105">Top level failure categories for enrollment.</span></span>
## <a name="members"></a><span data-ttu-id="e10b5-106">Membros</span><span class="sxs-lookup"><span data-stu-id="e10b5-106">Members</span></span>
|<span data-ttu-id="e10b5-107">Membro</span><span class="sxs-lookup"><span data-stu-id="e10b5-107">Member</span></span>|<span data-ttu-id="e10b5-108">Valor</span><span class="sxs-lookup"><span data-stu-id="e10b5-108">Value</span></span>|<span data-ttu-id="e10b5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e10b5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e10b5-110">unknown</span><span class="sxs-lookup"><span data-stu-id="e10b5-110">unknown</span></span>|<span data-ttu-id="e10b5-111">0</span><span class="sxs-lookup"><span data-stu-id="e10b5-111">0</span></span>|<span data-ttu-id="e10b5-112">Valor padrão, o motivo da falha é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="e10b5-112">Default value, failure reason is unknown.</span></span>|
|<span data-ttu-id="e10b5-113">autenticação</span><span class="sxs-lookup"><span data-stu-id="e10b5-113">authentication</span></span>|<span data-ttu-id="e10b5-114">1</span><span class="sxs-lookup"><span data-stu-id="e10b5-114">1</span></span>|<span data-ttu-id="e10b5-115">Falha na autenticação</span><span class="sxs-lookup"><span data-stu-id="e10b5-115">Authentication failed</span></span>|
|<span data-ttu-id="e10b5-116">autorização</span><span class="sxs-lookup"><span data-stu-id="e10b5-116">authorization</span></span>|<span data-ttu-id="e10b5-117">2</span><span class="sxs-lookup"><span data-stu-id="e10b5-117">2</span></span>|<span data-ttu-id="e10b5-118">Chamada foi autenticada, mas não autorizada a registrar.</span><span class="sxs-lookup"><span data-stu-id="e10b5-118">Call was authenticated, but not authorized to enroll.</span></span>|
|<span data-ttu-id="e10b5-119">accountValidation</span><span class="sxs-lookup"><span data-stu-id="e10b5-119">accountValidation</span></span>|<span data-ttu-id="e10b5-120">3</span><span class="sxs-lookup"><span data-stu-id="e10b5-120">3</span></span>|<span data-ttu-id="e10b5-121">Falha ao validar a conta para o registro.</span><span class="sxs-lookup"><span data-stu-id="e10b5-121">Failed to validate the account for enrollment.</span></span> <span data-ttu-id="e10b5-122">(Conta bloqueada, o registro não habilitado)</span><span class="sxs-lookup"><span data-stu-id="e10b5-122">(Account blocked, enrollment not enabled)</span></span>|
|<span data-ttu-id="e10b5-123">userValidation</span><span class="sxs-lookup"><span data-stu-id="e10b5-123">userValidation</span></span>|<span data-ttu-id="e10b5-124">4</span><span class="sxs-lookup"><span data-stu-id="e10b5-124">4</span></span>|<span data-ttu-id="e10b5-125">Usuário não pôde ser validado.</span><span class="sxs-lookup"><span data-stu-id="e10b5-125">User could not be validated.</span></span> <span data-ttu-id="e10b5-126">(Usuário não existe, licença falta)</span><span class="sxs-lookup"><span data-stu-id="e10b5-126">(User does not exist, missing license)</span></span>|
|<span data-ttu-id="e10b5-127">deviceNotSupported</span><span class="sxs-lookup"><span data-stu-id="e10b5-127">deviceNotSupported</span></span>|<span data-ttu-id="e10b5-128">5</span><span class="sxs-lookup"><span data-stu-id="e10b5-128">5</span></span>|<span data-ttu-id="e10b5-129">Não há suporte para o dispositivo para gerenciamento de dispositivos móveis.</span><span class="sxs-lookup"><span data-stu-id="e10b5-129">Device is not supported for mobile device management.</span></span>|
|<span data-ttu-id="e10b5-130">inMaintenance</span><span class="sxs-lookup"><span data-stu-id="e10b5-130">inMaintenance</span></span>|<span data-ttu-id="e10b5-131">6</span><span class="sxs-lookup"><span data-stu-id="e10b5-131">6</span></span>|<span data-ttu-id="e10b5-132">Conta está na manutenção.</span><span class="sxs-lookup"><span data-stu-id="e10b5-132">Account is in maintenance.</span></span>|
|<span data-ttu-id="e10b5-133">badRequest</span><span class="sxs-lookup"><span data-stu-id="e10b5-133">badRequest</span></span>|<span data-ttu-id="e10b5-134">7</span><span class="sxs-lookup"><span data-stu-id="e10b5-134">7</span></span>|<span data-ttu-id="e10b5-135">Cliente enviou uma solicitação que não seja compreendidos/suportados pelo serviço.</span><span class="sxs-lookup"><span data-stu-id="e10b5-135">Client sent a request that is not understood/supported by the service.</span></span>|
|<span data-ttu-id="e10b5-136">featureNotSupported</span><span class="sxs-lookup"><span data-stu-id="e10b5-136">featureNotSupported</span></span>|<span data-ttu-id="e10b5-137">8</span><span class="sxs-lookup"><span data-stu-id="e10b5-137">8</span></span>|<span data-ttu-id="e10b5-138">Os recursos usados por esta inscrição não são suportados para essa conta.</span><span class="sxs-lookup"><span data-stu-id="e10b5-138">Feature(s) used by this enrollment are not supported for this account.</span></span>|
|<span data-ttu-id="e10b5-139">enrollmentRestrictionsEnforced</span><span class="sxs-lookup"><span data-stu-id="e10b5-139">enrollmentRestrictionsEnforced</span></span>|<span data-ttu-id="e10b5-140">9</span><span class="sxs-lookup"><span data-stu-id="e10b5-140">9</span></span>|<span data-ttu-id="e10b5-141">Restrições de registro configuradas pelo administrador bloqueado este registro.</span><span class="sxs-lookup"><span data-stu-id="e10b5-141">Enrollment restrictions configured by admin blocked this enrollment.</span></span>|
|<span data-ttu-id="e10b5-142">clientDisconnected</span><span class="sxs-lookup"><span data-stu-id="e10b5-142">clientDisconnected</span></span>|<span data-ttu-id="e10b5-143">10</span><span class="sxs-lookup"><span data-stu-id="e10b5-143">10</span></span>|<span data-ttu-id="e10b5-144">Cliente esgotado ou inscrição foi anulada pelo usuário final.</span><span class="sxs-lookup"><span data-stu-id="e10b5-144">Client timed out or enrollment was aborted by enduser.</span></span>|
|<span data-ttu-id="e10b5-145">userAbandonment</span><span class="sxs-lookup"><span data-stu-id="e10b5-145">userAbandonment</span></span>|<span data-ttu-id="e10b5-146">11</span><span class="sxs-lookup"><span data-stu-id="e10b5-146">11</span></span>|<span data-ttu-id="e10b5-147">O registro foi abandonado pelo usuário final.</span><span class="sxs-lookup"><span data-stu-id="e10b5-147">Enrollment was abandoned by enduser.</span></span> <span data-ttu-id="e10b5-148">(Usuário final inclusão de Introdução, mas não conseguiu concluí-la no modo oportuno)</span><span class="sxs-lookup"><span data-stu-id="e10b5-148">(Enduser started onboarding but failed to complete it in timely manner)</span></span>|


<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Enum deviceEnrollmentFailureReason has some values specified and others unspecified."
  ],
}
-->
