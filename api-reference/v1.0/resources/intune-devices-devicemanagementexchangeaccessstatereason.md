---
title: tipo de enumeração deviceManagementExchangeAccessStateReason
description: Motivo do estado de acesso ao Exchange do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 37ce7d40ef2f8ea6cc729b25bcfc9b66480fdf6a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091169"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a><span data-ttu-id="6bbb3-103">tipo de enumeração deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="6bbb3-103">deviceManagementExchangeAccessStateReason enum type</span></span>

<span data-ttu-id="6bbb3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bbb3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6bbb3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bbb3-106">Motivo do estado de acesso ao Exchange do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6bbb3-106">Device Exchange Access State Reason.</span></span>

## <a name="members"></a><span data-ttu-id="6bbb3-107">Membros</span><span class="sxs-lookup"><span data-stu-id="6bbb3-107">Members</span></span>
|<span data-ttu-id="6bbb3-108">Membro</span><span class="sxs-lookup"><span data-stu-id="6bbb3-108">Member</span></span>|<span data-ttu-id="6bbb3-109">Valor</span><span class="sxs-lookup"><span data-stu-id="6bbb3-109">Value</span></span>|<span data-ttu-id="6bbb3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bbb3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bbb3-111">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6bbb3-111">none</span></span>|<span data-ttu-id="6bbb3-112">,0</span><span class="sxs-lookup"><span data-stu-id="6bbb3-112">0</span></span>|<span data-ttu-id="6bbb3-113">Nenhum motivo de estado de acesso descoberto do Exchange</span><span class="sxs-lookup"><span data-stu-id="6bbb3-113">No access state reason discovered from Exchange</span></span>|
|<span data-ttu-id="6bbb3-114">desconhecido</span><span class="sxs-lookup"><span data-stu-id="6bbb3-114">unknown</span></span>|<span data-ttu-id="6bbb3-115">1 </span><span class="sxs-lookup"><span data-stu-id="6bbb3-115">1</span></span>|<span data-ttu-id="6bbb3-116">Razão do estado de acesso desconhecido</span><span class="sxs-lookup"><span data-stu-id="6bbb3-116">Unknown access state reason</span></span>|
|<span data-ttu-id="6bbb3-117">exchangeGlobalRule</span><span class="sxs-lookup"><span data-stu-id="6bbb3-117">exchangeGlobalRule</span></span>|<span data-ttu-id="6bbb3-118">2 </span><span class="sxs-lookup"><span data-stu-id="6bbb3-118">2</span></span>|<span data-ttu-id="6bbb3-119">Estado de acesso determinado pela regra global do Exchange</span><span class="sxs-lookup"><span data-stu-id="6bbb3-119">Access state determined by Exchange Global rule</span></span>|
|<span data-ttu-id="6bbb3-120">exchangeIndividualRule</span><span class="sxs-lookup"><span data-stu-id="6bbb3-120">exchangeIndividualRule</span></span>|<span data-ttu-id="6bbb3-121">3D</span><span class="sxs-lookup"><span data-stu-id="6bbb3-121">3</span></span>|<span data-ttu-id="6bbb3-122">Estado de acesso determinado pela regra individual do Exchange</span><span class="sxs-lookup"><span data-stu-id="6bbb3-122">Access state determined by Exchange Individual rule</span></span>|
|<span data-ttu-id="6bbb3-123">exchangeDeviceRule</span><span class="sxs-lookup"><span data-stu-id="6bbb3-123">exchangeDeviceRule</span></span>|<span data-ttu-id="6bbb3-124">4 </span><span class="sxs-lookup"><span data-stu-id="6bbb3-124">4</span></span>|<span data-ttu-id="6bbb3-125">Estado de acesso determinado pela regra de dispositivo do Exchange</span><span class="sxs-lookup"><span data-stu-id="6bbb3-125">Access state determined by Exchange Device rule</span></span>|
|<span data-ttu-id="6bbb3-126">exchangeUpgrade</span><span class="sxs-lookup"><span data-stu-id="6bbb3-126">exchangeUpgrade</span></span>|<span data-ttu-id="6bbb3-127">5 </span><span class="sxs-lookup"><span data-stu-id="6bbb3-127">5</span></span>|<span data-ttu-id="6bbb3-128">Estado de acesso devido à atualização do Exchange</span><span class="sxs-lookup"><span data-stu-id="6bbb3-128">Access state due to Exchange upgrade</span></span>|
|<span data-ttu-id="6bbb3-129">exchangeMailboxPolicy</span><span class="sxs-lookup"><span data-stu-id="6bbb3-129">exchangeMailboxPolicy</span></span>|<span data-ttu-id="6bbb3-130">6 </span><span class="sxs-lookup"><span data-stu-id="6bbb3-130">6</span></span>|<span data-ttu-id="6bbb3-131">Estado de acesso determinado pela política de caixa de correio do Exchange</span><span class="sxs-lookup"><span data-stu-id="6bbb3-131">Access state determined by Exchange Mailbox Policy</span></span>|
|<span data-ttu-id="6bbb3-132">outro</span><span class="sxs-lookup"><span data-stu-id="6bbb3-132">other</span></span>|<span data-ttu-id="6bbb3-133">7 </span><span class="sxs-lookup"><span data-stu-id="6bbb3-133">7</span></span>|<span data-ttu-id="6bbb3-134">Estado de acesso determinado pelo Exchange</span><span class="sxs-lookup"><span data-stu-id="6bbb3-134">Access state determined by Exchange</span></span>|
|<span data-ttu-id="6bbb3-135">com</span><span class="sxs-lookup"><span data-stu-id="6bbb3-135">compliant</span></span>|<span data-ttu-id="6bbb3-136">8 </span><span class="sxs-lookup"><span data-stu-id="6bbb3-136">8</span></span>|<span data-ttu-id="6bbb3-137">Estado de acesso concedido por desafio de conformidade</span><span class="sxs-lookup"><span data-stu-id="6bbb3-137">Access state granted by compliance challenge</span></span>|
|<span data-ttu-id="6bbb3-138">incompatível</span><span class="sxs-lookup"><span data-stu-id="6bbb3-138">notCompliant</span></span>|<span data-ttu-id="6bbb3-139">9 </span><span class="sxs-lookup"><span data-stu-id="6bbb3-139">9</span></span>|<span data-ttu-id="6bbb3-140">Estado de acesso revogado pelo desafio de conformidade</span><span class="sxs-lookup"><span data-stu-id="6bbb3-140">Access state revoked by compliance challenge</span></span>|
|<span data-ttu-id="6bbb3-141">Não registrado</span><span class="sxs-lookup"><span data-stu-id="6bbb3-141">notEnrolled</span></span>|<span data-ttu-id="6bbb3-142">10 </span><span class="sxs-lookup"><span data-stu-id="6bbb3-142">10</span></span>|<span data-ttu-id="6bbb3-143">Estado de acesso revogado pelo desafio de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="6bbb3-143">Access state revoked by management challenge</span></span>|
|<span data-ttu-id="6bbb3-144">unknownLocation</span><span class="sxs-lookup"><span data-stu-id="6bbb3-144">unknownLocation</span></span>|<span data-ttu-id="6bbb3-145">12 </span><span class="sxs-lookup"><span data-stu-id="6bbb3-145">12</span></span>|<span data-ttu-id="6bbb3-146">Estado de acesso devido à localização desconhecida</span><span class="sxs-lookup"><span data-stu-id="6bbb3-146">Access state due to unknown location</span></span>|
|<span data-ttu-id="6bbb3-147">mfaRequired</span><span class="sxs-lookup"><span data-stu-id="6bbb3-147">mfaRequired</span></span>|<span data-ttu-id="6bbb3-148">13 </span><span class="sxs-lookup"><span data-stu-id="6bbb3-148">13</span></span>|<span data-ttu-id="6bbb3-149">Estado de acesso devido ao desafio da MFA</span><span class="sxs-lookup"><span data-stu-id="6bbb3-149">Access state due to MFA challenge</span></span>|
|<span data-ttu-id="6bbb3-150">azureADBlockDueToAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="6bbb3-150">azureADBlockDueToAccessPolicy</span></span>|<span data-ttu-id="6bbb3-151">14 </span><span class="sxs-lookup"><span data-stu-id="6bbb3-151">14</span></span>|<span data-ttu-id="6bbb3-152">Estado de acesso revogado pela política de acesso AAD</span><span class="sxs-lookup"><span data-stu-id="6bbb3-152">Access State revoked by AAD Access Policy</span></span>|
|<span data-ttu-id="6bbb3-153">compromisedPassword</span><span class="sxs-lookup"><span data-stu-id="6bbb3-153">compromisedPassword</span></span>|<span data-ttu-id="6bbb3-154">15 </span><span class="sxs-lookup"><span data-stu-id="6bbb3-154">15</span></span>|<span data-ttu-id="6bbb3-155">Estado de acesso revogado por senha comprometida</span><span class="sxs-lookup"><span data-stu-id="6bbb3-155">Access State revoked by compromised password</span></span>|
|<span data-ttu-id="6bbb3-156">deviceNotKnownWithManagedApp</span><span class="sxs-lookup"><span data-stu-id="6bbb3-156">deviceNotKnownWithManagedApp</span></span>|<span data-ttu-id="6bbb3-157">16 </span><span class="sxs-lookup"><span data-stu-id="6bbb3-157">16</span></span>|<span data-ttu-id="6bbb3-158">Estado de acesso revogado por desafio de aplicativo gerenciado</span><span class="sxs-lookup"><span data-stu-id="6bbb3-158">Access state revoked by managed application challenge</span></span>|









