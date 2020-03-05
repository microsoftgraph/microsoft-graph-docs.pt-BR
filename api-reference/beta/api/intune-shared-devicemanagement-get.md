---
title: Acessar deviceManagement
description: Leia as propriedades e as relações do objeto deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9a14fd14f5b020eb45327f49c8b63bdd4dc2c1db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458627"
---
# <a name="get-devicemanagement"></a><span data-ttu-id="b99f7-103">Acessar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="b99f7-103">Get deviceManagement</span></span>

<span data-ttu-id="b99f7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b99f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b99f7-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b99f7-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b99f7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b99f7-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b99f7-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b99f7-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b99f7-108">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="b99f7-108">Read properties and relationships of the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b99f7-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b99f7-109">Prerequisites</span></span>

<span data-ttu-id="b99f7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b99f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b99f7-112">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="b99f7-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="b99f7-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b99f7-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="b99f7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b99f7-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="b99f7-115">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="b99f7-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="b99f7-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b99f7-117">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="b99f7-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="b99f7-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="b99f7-119">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="b99f7-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="b99f7-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b99f7-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b99f7-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b99f7-123">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b99f7-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="b99f7-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="b99f7-125">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b99f7-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b99f7-126">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-126">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="b99f7-127">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="b99f7-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="b99f7-128">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-128">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b99f7-129">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="b99f7-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="b99f7-130">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-130">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-131">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="b99f7-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="b99f7-132">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-132">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b99f7-133">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="b99f7-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="b99f7-134">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-134">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-135">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="b99f7-135">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="b99f7-136">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-136">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-137">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="b99f7-137">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b99f7-138">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-138">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-139">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="b99f7-139">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b99f7-140">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-140">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-141">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="b99f7-141">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="b99f7-142">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-142">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="b99f7-143">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="b99f7-143">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="b99f7-144">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-144">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b99f7-145">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="b99f7-145">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="b99f7-146">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-146">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-147">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="b99f7-147">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="b99f7-148">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-148">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-149">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="b99f7-149">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="b99f7-150">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-150">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-151">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="b99f7-151">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b99f7-152">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-152">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="b99f7-153">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="b99f7-153">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="b99f7-154">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-154">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="b99f7-155">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b99f7-155">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b99f7-156">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b99f7-156">Not supported.</span></span>|
| <span data-ttu-id="b99f7-157">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b99f7-157">Application</span></span> | |
| <span data-ttu-id="b99f7-158">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="b99f7-158">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="b99f7-159">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-159">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b99f7-160">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="b99f7-160">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="b99f7-161">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-161">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="b99f7-162">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="b99f7-162">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="b99f7-163">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-163">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-164">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b99f7-164">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b99f7-165">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-165">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b99f7-166">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b99f7-166">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="b99f7-167">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-167">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="b99f7-168">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b99f7-168">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b99f7-169">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-169">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="b99f7-170">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="b99f7-170">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="b99f7-171">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-171">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b99f7-172">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="b99f7-172">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="b99f7-173">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-173">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-174">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="b99f7-174">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="b99f7-175">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-175">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b99f7-176">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="b99f7-176">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="b99f7-177">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-177">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-178">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="b99f7-178">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="b99f7-179">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-179">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-180">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="b99f7-180">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="b99f7-181">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-181">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-182">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="b99f7-182">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="b99f7-183">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-183">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-184">&nbsp;&nbsp; **RBAC**</span><span class="sxs-lookup"><span data-stu-id="b99f7-184">&nbsp; &nbsp; **RBAC**</span></span> | <span data-ttu-id="b99f7-185">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-185">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="b99f7-186">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="b99f7-186">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="b99f7-187">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-187">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="b99f7-188">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="b99f7-188">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="b99f7-189">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-189">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-190">&nbsp;&nbsp; **Atualização de software**</span><span class="sxs-lookup"><span data-stu-id="b99f7-190">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="b99f7-191">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-191">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-192">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="b99f7-192">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="b99f7-193">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-193">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="b99f7-194">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="b99f7-194">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b99f7-195">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-195">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="b99f7-196">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="b99f7-196">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="b99f7-197">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b99f7-197">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b99f7-198">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b99f7-198">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b99f7-199">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b99f7-199">Optional query parameters</span></span>

<span data-ttu-id="b99f7-200">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b99f7-200">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b99f7-201">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b99f7-201">Request headers</span></span>
|<span data-ttu-id="b99f7-202">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b99f7-202">Header</span></span>|<span data-ttu-id="b99f7-203">Valor</span><span class="sxs-lookup"><span data-stu-id="b99f7-203">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b99f7-204">Autorização</span><span class="sxs-lookup"><span data-stu-id="b99f7-204">Authorization</span></span>|<span data-ttu-id="b99f7-205">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b99f7-205">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b99f7-206">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b99f7-206">Accept</span></span>|<span data-ttu-id="b99f7-207">application/json</span><span class="sxs-lookup"><span data-stu-id="b99f7-207">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b99f7-208">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b99f7-208">Request body</span></span>

<span data-ttu-id="b99f7-209">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b99f7-209">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b99f7-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="b99f7-210">Response</span></span>

<span data-ttu-id="b99f7-211">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b99f7-211">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b99f7-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b99f7-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="b99f7-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b99f7-213">Request</span></span>

<span data-ttu-id="b99f7-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b99f7-214">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```

### <a name="response"></a><span data-ttu-id="b99f7-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="b99f7-215">Response</span></span>

<span data-ttu-id="b99f7-216">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b99f7-216">Here are example of the response.</span></span> 

<span data-ttu-id="b99f7-217">Observação: os objetos de resposta mostrados aqui podem ser truncados por brevidade.</span><span class="sxs-lookup"><span data-stu-id="b99f7-217">Note: The response objects shown here may be truncated for brevity.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b"
  }
}
```

<span data-ttu-id="b99f7-218">As propriedades apropriadas para o fluxo de trabalho são retornadas.</span><span class="sxs-lookup"><span data-stu-id="b99f7-218">Properties appropriate for the workflow are returned.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b",
    "subscriptionState": "active",
    "subscriptions": "intune",
    "adminConsent": {
      "@odata.type": "microsoft.graph.adminConsent",
      "shareAPNSData": "granted"
    },
    "deviceProtectionOverview": {
      "@odata.type": "microsoft.graph.deviceProtectionOverview",
      "totalReportedDeviceCount": 8,
      "inactiveThreatAgentDeviceCount": 14,
      "unknownStateThreatAgentDeviceCount": 2,
      "pendingSignatureUpdateDeviceCount": 1,
      "cleanDeviceCount": 0,
      "pendingFullScanDeviceCount": 10,
      "pendingRestartDeviceCount": 9,
      "pendingManualStepsDeviceCount": 13,
      "pendingOfflineScanDeviceCount": 13,
      "criticalFailuresDeviceCount": 11
    },
    "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
  }
}
```











