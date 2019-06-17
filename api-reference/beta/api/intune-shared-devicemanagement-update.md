---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a77605170d7df943b0d1a96fc2fe864b9d46e4f7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989690"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="8743a-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="8743a-103">Update deviceManagement</span></span>

> <span data-ttu-id="8743a-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8743a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8743a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8743a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8743a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8743a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8743a-107">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="8743a-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8743a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8743a-108">Prerequisites</span></span>

<span data-ttu-id="8743a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8743a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8743a-111">Observe que a permissão varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="8743a-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="8743a-112">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="8743a-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="8743a-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8743a-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="8743a-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8743a-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="8743a-115">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="8743a-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="8743a-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="8743a-117">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="8743a-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="8743a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="8743a-119">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="8743a-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="8743a-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="8743a-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="8743a-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8743a-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="8743a-123">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="8743a-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="8743a-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="8743a-125">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="8743a-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8743a-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="8743a-127">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="8743a-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="8743a-128">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-128">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="8743a-129">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="8743a-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="8743a-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-130">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="8743a-131">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="8743a-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="8743a-132">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-132">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="8743a-133">&nbsp;&nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="8743a-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="8743a-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="8743a-135">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="8743a-135">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="8743a-136">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-136">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="8743a-137">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="8743a-137">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="8743a-138">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-138">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="8743a-139">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="8743a-139">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="8743a-140">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-140">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="8743a-141">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="8743a-141">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="8743a-142">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8743a-142">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="8743a-143">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="8743a-143">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="8743a-144">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-144">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="8743a-145">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="8743a-145">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="8743a-146">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-146">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="8743a-147">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="8743a-147">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="8743a-148">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-148">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="8743a-149">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="8743a-149">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="8743a-150">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8743a-150">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="8743a-151">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8743a-151">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8743a-152">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8743a-152">Not supported.</span></span>|
| <span data-ttu-id="8743a-153">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8743a-153">Application</span></span> | <span data-ttu-id="8743a-154">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8743a-154">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8743a-155">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8743a-155">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="8743a-156">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8743a-156">Request headers</span></span>

|<span data-ttu-id="8743a-157">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8743a-157">Header</span></span>|<span data-ttu-id="8743a-158">Valor</span><span class="sxs-lookup"><span data-stu-id="8743a-158">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8743a-159">Autorização</span><span class="sxs-lookup"><span data-stu-id="8743a-159">Authorization</span></span>|<span data-ttu-id="8743a-160">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8743a-160">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8743a-161">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8743a-161">Accept</span></span>|<span data-ttu-id="8743a-162">application/json</span><span class="sxs-lookup"><span data-stu-id="8743a-162">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8743a-163">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8743a-163">Request body</span></span>

<span data-ttu-id="8743a-164">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="8743a-164">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="8743a-165">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="8743a-165">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="8743a-166">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8743a-166">Property</span></span>|<span data-ttu-id="8743a-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="8743a-167">Type</span></span>|<span data-ttu-id="8743a-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="8743a-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8743a-169">id</span><span class="sxs-lookup"><span data-stu-id="8743a-169">id</span></span>|<span data-ttu-id="8743a-170">String</span><span class="sxs-lookup"><span data-stu-id="8743a-170">String</span></span>|<span data-ttu-id="8743a-171">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8743a-171">Unique identifier for the device.</span></span>|
|<span data-ttu-id="8743a-172">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="8743a-172">**Device configuration**</span></span>|
|<span data-ttu-id="8743a-173">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="8743a-173">intuneAccountId</span></span>|<span data-ttu-id="8743a-174">GUID</span><span class="sxs-lookup"><span data-stu-id="8743a-174">GUID</span></span>|<span data-ttu-id="8743a-175">ID da conta do Intune para determinado locatário</span><span class="sxs-lookup"><span data-stu-id="8743a-175">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="8743a-176">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="8743a-176">legacyPcManangementEnabled</span></span>|<span data-ttu-id="8743a-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="8743a-177">Boolean</span></span>|<span data-ttu-id="8743a-178">A propriedade para habilitar o gerenciamento de computador herdado não MDM gerenciado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="8743a-178">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="8743a-179">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8743a-179">This property is read-only.</span></span>|
|<span data-ttu-id="8743a-180">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="8743a-180">maximumDepTokens</span></span>|<span data-ttu-id="8743a-181">Int32</span><span class="sxs-lookup"><span data-stu-id="8743a-181">Int32</span></span>|<span data-ttu-id="8743a-182">Número máximo de tokens DEP permitidos por locatário.</span><span class="sxs-lookup"><span data-stu-id="8743a-182">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="8743a-183">settings</span><span class="sxs-lookup"><span data-stu-id="8743a-183">settings</span></span>|[<span data-ttu-id="8743a-184">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="8743a-184">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="8743a-185">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="8743a-185">Account level settings.</span></span>|
|<span data-ttu-id="8743a-186">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="8743a-186">**Device management**</span></span>|
|<span data-ttu-id="8743a-187">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="8743a-187">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="8743a-188">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8743a-188">DateTimeOffset</span></span>|<span data-ttu-id="8743a-189">A data & hora em que os dados do locatário são movidos entre o ScaleUnits.</span><span class="sxs-lookup"><span data-stu-id="8743a-189">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="8743a-190">adminConsent</span><span class="sxs-lookup"><span data-stu-id="8743a-190">adminConsent</span></span>|[<span data-ttu-id="8743a-191">adminConsent</span><span class="sxs-lookup"><span data-stu-id="8743a-191">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="8743a-192">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="8743a-192">Admin consent information.</span></span>|
|<span data-ttu-id="8743a-193">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="8743a-193">deviceProtectionOverview</span></span>|[<span data-ttu-id="8743a-194">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="8743a-194">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="8743a-195">Visão geral da proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8743a-195">Device protection overview.</span></span>|
|<span data-ttu-id="8743a-196">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="8743a-196">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="8743a-197">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="8743a-197">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="8743a-198">Regra de limpeza de dispositivo</span><span class="sxs-lookup"><span data-stu-id="8743a-198">Device cleanup rule</span></span>|
|<span data-ttu-id="8743a-199">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="8743a-199">subscriptionState</span></span>|[<span data-ttu-id="8743a-200">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="8743a-200">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="8743a-201">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="8743a-201">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="8743a-202">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="8743a-202">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="8743a-203">assinaturas</span><span class="sxs-lookup"><span data-stu-id="8743a-203">subscriptions</span></span>|[<span data-ttu-id="8743a-204">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="8743a-204">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="8743a-205">Assinatura do locatário.</span><span class="sxs-lookup"><span data-stu-id="8743a-205">Tenant's Subscription.</span></span> <span data-ttu-id="8743a-206">Os possíveis valores são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="8743a-206">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="8743a-207">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="8743a-207">windowsMalwareOverview</span></span>|[<span data-ttu-id="8743a-208">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="8743a-208">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="8743a-209">Visão geral de malware para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="8743a-209">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="8743a-210">**Integração**</span><span class="sxs-lookup"><span data-stu-id="8743a-210">**Onboarding**</span></span>|
|<span data-ttu-id="8743a-211">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="8743a-211">intuneBrand</span></span>|[<span data-ttu-id="8743a-212">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="8743a-212">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="8743a-213">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="8743a-213">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="8743a-214">O suporte à propriedade do corpo da solicitação varia de acordo com o fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="8743a-214">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="8743a-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="8743a-215">Response</span></span>
<span data-ttu-id="8743a-216">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8743a-216">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8743a-217">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8743a-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="8743a-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8743a-218">Request</span></span>

<span data-ttu-id="8743a-219">Veja a seguir um exemplo de uma solicitação após o fluxo de trabalho de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="8743a-219">Here is an example of a request following the device management workflow:</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
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
```

### <a name="response"></a><span data-ttu-id="8743a-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="8743a-220">Response</span></span>

<span data-ttu-id="8743a-221">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8743a-221">Here is an example of the response.</span></span> 

<span data-ttu-id="8743a-222">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="8743a-222">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8743a-223">As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.</span><span class="sxs-lookup"><span data-stu-id="8743a-223">Returned properties vary according to workflow and context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
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
```



