---
title: tipo de enumeração deviceManagementExchangeAccessStateReason
description: Motivo do estado de acesso ao Exchange do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0b2e45192ee953ca38e3738c87ee3c0714d0dfdd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060150"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="d346a-103">tipo de enumeração deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="d346a-103">deviceManagementExchangeAccessStateReason enum type</span></span>

<span data-ttu-id="d346a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d346a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d346a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d346a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d346a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d346a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d346a-107">Motivo do estado de acesso ao Exchange do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d346a-107">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="d346a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="d346a-108">Members</span></span>
|<span data-ttu-id="d346a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="d346a-109">Member</span></span>|<span data-ttu-id="d346a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="d346a-110">Value</span></span>|<span data-ttu-id="d346a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d346a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d346a-112">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d346a-112">none</span></span>|<span data-ttu-id="d346a-113">,0</span><span class="sxs-lookup"><span data-stu-id="d346a-113">0</span></span>|<span data-ttu-id="d346a-114">Nenhum motivo de estado de acesso descoberto do Exchange</span><span class="sxs-lookup"><span data-stu-id="d346a-114">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="d346a-115">desconhecido</span><span class="sxs-lookup"><span data-stu-id="d346a-115">unknown</span></span>|<span data-ttu-id="d346a-116">1 </span><span class="sxs-lookup"><span data-stu-id="d346a-116">1</span></span>|<span data-ttu-id="d346a-117">Razão do estado de acesso desconhecido</span><span class="sxs-lookup"><span data-stu-id="d346a-117">Unknown access state reason</span></span>|
|<span data-ttu-id="d346a-118">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="d346a-118">exchangeGlobalRule</span></span>|<span data-ttu-id="d346a-119">2 </span><span class="sxs-lookup"><span data-stu-id="d346a-119">2</span></span>|<span data-ttu-id="d346a-120">Estado de acesso determinado pela regra global do Exchange</span><span class="sxs-lookup"><span data-stu-id="d346a-120">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="d346a-121">exchangeIndividualRule</span><span class="sxs-lookup"><span data-stu-id="d346a-121">exchangeIndividualRule</span></span>|<span data-ttu-id="d346a-122">3 </span><span class="sxs-lookup"><span data-stu-id="d346a-122">3</span></span>|<span data-ttu-id="d346a-123">Estado de acesso determinado pela regra individual do Exchange</span><span class="sxs-lookup"><span data-stu-id="d346a-123">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="d346a-124">exchangeDeviceRule</span><span class="sxs-lookup"><span data-stu-id="d346a-124">exchangeDeviceRule</span></span>|<span data-ttu-id="d346a-125">4 </span><span class="sxs-lookup"><span data-stu-id="d346a-125">4</span></span>|<span data-ttu-id="d346a-126">Estado de acesso determinado pela regra de dispositivo do Exchange</span><span class="sxs-lookup"><span data-stu-id="d346a-126">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="d346a-127">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="d346a-127">exchangeUpgrade</span></span>|<span data-ttu-id="d346a-128">5 </span><span class="sxs-lookup"><span data-stu-id="d346a-128">5</span></span>|<span data-ttu-id="d346a-129">Estado de acesso devido à atualização do Exchange</span><span class="sxs-lookup"><span data-stu-id="d346a-129">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="d346a-130">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="d346a-130">exchangeMailboxPolicy</span></span>|<span data-ttu-id="d346a-131">6 </span><span class="sxs-lookup"><span data-stu-id="d346a-131">6</span></span>|<span data-ttu-id="d346a-132">Estado de acesso determinado pela política de caixa de correio do Exchange</span><span class="sxs-lookup"><span data-stu-id="d346a-132">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="d346a-133">outro</span><span class="sxs-lookup"><span data-stu-id="d346a-133">other</span></span>|<span data-ttu-id="d346a-134">7 </span><span class="sxs-lookup"><span data-stu-id="d346a-134">7</span></span>|<span data-ttu-id="d346a-135">Estado de acesso determinado pelo Exchange</span><span class="sxs-lookup"><span data-stu-id="d346a-135">Access state determined by Exchange</span></span>|
|<span data-ttu-id="d346a-136">com</span><span class="sxs-lookup"><span data-stu-id="d346a-136">compliant</span></span>|<span data-ttu-id="d346a-137">8 </span><span class="sxs-lookup"><span data-stu-id="d346a-137">8</span></span>|<span data-ttu-id="d346a-138">Estado de acesso concedido por desafio de conformidade</span><span class="sxs-lookup"><span data-stu-id="d346a-138">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="d346a-139">incompatível</span><span class="sxs-lookup"><span data-stu-id="d346a-139">notCompliant</span></span>|<span data-ttu-id="d346a-140">9 </span><span class="sxs-lookup"><span data-stu-id="d346a-140">9</span></span>|<span data-ttu-id="d346a-141">Estado de acesso revogado pelo desafio de conformidade</span><span class="sxs-lookup"><span data-stu-id="d346a-141">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="d346a-142">Não registrado</span><span class="sxs-lookup"><span data-stu-id="d346a-142">notEnrolled</span></span>|<span data-ttu-id="d346a-143">10 </span><span class="sxs-lookup"><span data-stu-id="d346a-143">10</span></span>|<span data-ttu-id="d346a-144">Estado de acesso revogado pelo desafio de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="d346a-144">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="d346a-145">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="d346a-145">unknownLocation</span></span>|<span data-ttu-id="d346a-146">12 </span><span class="sxs-lookup"><span data-stu-id="d346a-146">12</span></span>|<span data-ttu-id="d346a-147">Estado de acesso devido à localização desconhecida</span><span class="sxs-lookup"><span data-stu-id="d346a-147">Access state due to unknown location</span></span>|
|<span data-ttu-id="d346a-148">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="d346a-148">mfaRequired</span></span>|<span data-ttu-id="d346a-149">13 </span><span class="sxs-lookup"><span data-stu-id="d346a-149">13</span></span>|<span data-ttu-id="d346a-150">Estado de acesso devido ao desafio da MFA</span><span class="sxs-lookup"><span data-stu-id="d346a-150">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="d346a-151">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="d346a-151">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="d346a-152">14 </span><span class="sxs-lookup"><span data-stu-id="d346a-152">14</span></span>|<span data-ttu-id="d346a-153">Estado de acesso revogado pela política de acesso AAD</span><span class="sxs-lookup"><span data-stu-id="d346a-153">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="d346a-154">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="d346a-154">compromisedPassword</span></span>|<span data-ttu-id="d346a-155">15 </span><span class="sxs-lookup"><span data-stu-id="d346a-155">15</span></span>|<span data-ttu-id="d346a-156">Estado de acesso revogado por senha comprometida</span><span class="sxs-lookup"><span data-stu-id="d346a-156">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="d346a-157">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="d346a-157">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="d346a-158">16 </span><span class="sxs-lookup"><span data-stu-id="d346a-158">16</span></span>|<span data-ttu-id="d346a-159">Estado de acesso revogado por desafio de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="d346a-159">Access state revoked by managed application challenge</span></span>|






