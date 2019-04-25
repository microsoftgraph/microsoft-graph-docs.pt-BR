---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e0dc83489ede464eb9da000acb8db4e6af13f8d2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527046"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="5c507-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="5c507-103">Update deviceManagement</span></span>

> <span data-ttu-id="5c507-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5c507-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5c507-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5c507-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c507-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c507-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c507-107">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="5c507-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c507-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5c507-108">Prerequisites</span></span>

<span data-ttu-id="5c507-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c507-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5c507-111">Observe que a permissão varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5c507-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="5c507-112">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="5c507-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="5c507-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5c507-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="5c507-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c507-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="5c507-115">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="5c507-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="5c507-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c507-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="5c507-117">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="5c507-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="5c507-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c507-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="5c507-119">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="5c507-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="5c507-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c507-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5c507-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="5c507-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="5c507-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c507-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="5c507-123">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="5c507-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="5c507-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c507-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="5c507-125">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="5c507-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="5c507-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c507-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="5c507-127">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="5c507-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="5c507-128">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c507-128">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="5c507-129">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="5c507-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="5c507-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c507-130">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5c507-131">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="5c507-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="5c507-132">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c507-132">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="5c507-133">&nbsp;&nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="5c507-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="5c507-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c507-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5c507-135">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="5c507-135">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="5c507-136">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c507-136">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5c507-137">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="5c507-137">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="5c507-138">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c507-138">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="5c507-139">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="5c507-139">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="5c507-140">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5c507-140">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="5c507-141">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="5c507-141">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="5c507-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c507-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5c507-143">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="5c507-143">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="5c507-144">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c507-144">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5c507-145">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="5c507-145">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="5c507-146">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c507-146">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="5c507-147">&nbsp;&nbsp; **Proteção de informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="5c507-147">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="5c507-148">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c507-148">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="5c507-149">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c507-149">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c507-150">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c507-150">Not supported.</span></span>|
| <span data-ttu-id="5c507-151">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c507-151">Application</span></span> | <span data-ttu-id="5c507-152">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c507-152">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c507-153">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c507-153">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="5c507-154">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c507-154">Request headers</span></span>

|<span data-ttu-id="5c507-155">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c507-155">Header</span></span>|<span data-ttu-id="5c507-156">Valor</span><span class="sxs-lookup"><span data-stu-id="5c507-156">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c507-157">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c507-157">Authorization</span></span>|<span data-ttu-id="5c507-158">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c507-158">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c507-159">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5c507-159">Accept</span></span>|<span data-ttu-id="5c507-160">application/json</span><span class="sxs-lookup"><span data-stu-id="5c507-160">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c507-161">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c507-161">Request body</span></span>

<span data-ttu-id="5c507-162">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="5c507-162">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="5c507-163">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="5c507-163">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="5c507-164">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c507-164">Property</span></span>|<span data-ttu-id="5c507-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c507-165">Type</span></span>|<span data-ttu-id="5c507-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c507-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c507-167">id</span><span class="sxs-lookup"><span data-stu-id="5c507-167">id</span></span>|<span data-ttu-id="5c507-168">String</span><span class="sxs-lookup"><span data-stu-id="5c507-168">String</span></span>|<span data-ttu-id="5c507-169">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c507-169">Unique identifier for the device.</span></span>|
|<span data-ttu-id="5c507-170">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="5c507-170">**Device configuration**</span></span>|
|<span data-ttu-id="5c507-171">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="5c507-171">intuneAccountId</span></span>|<span data-ttu-id="5c507-172">GUID</span><span class="sxs-lookup"><span data-stu-id="5c507-172">GUID</span></span>|<span data-ttu-id="5c507-173">ID da conta do Intune para determinado locatário</span><span class="sxs-lookup"><span data-stu-id="5c507-173">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="5c507-174">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="5c507-174">legacyPcManangementEnabled</span></span>|<span data-ttu-id="5c507-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="5c507-175">Boolean</span></span>|<span data-ttu-id="5c507-176">A propriedade para habilitar o gerenciamento de computador herdado não MDM gerenciado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="5c507-176">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="5c507-177">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5c507-177">This property is read-only.</span></span>|
|<span data-ttu-id="5c507-178">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="5c507-178">maximumDepTokens</span></span>|<span data-ttu-id="5c507-179">Int32</span><span class="sxs-lookup"><span data-stu-id="5c507-179">Int32</span></span>|<span data-ttu-id="5c507-180">Número máximo de tokens DEP permitidos por locatário.</span><span class="sxs-lookup"><span data-stu-id="5c507-180">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="5c507-181">settings</span><span class="sxs-lookup"><span data-stu-id="5c507-181">settings</span></span>|[<span data-ttu-id="5c507-182">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="5c507-182">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="5c507-183">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="5c507-183">Account level settings.</span></span>|
|<span data-ttu-id="5c507-184">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="5c507-184">**Device management**</span></span>|
|<span data-ttu-id="5c507-185">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="5c507-185">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="5c507-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c507-186">DateTimeOffset</span></span>|<span data-ttu-id="5c507-187">A data & hora em que os dados do locatário são movidos entre ScaleUnits.</span><span class="sxs-lookup"><span data-stu-id="5c507-187">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="5c507-188">adminConsent</span><span class="sxs-lookup"><span data-stu-id="5c507-188">adminConsent</span></span>|[<span data-ttu-id="5c507-189">adminConsent</span><span class="sxs-lookup"><span data-stu-id="5c507-189">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="5c507-190">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="5c507-190">Admin consent information.</span></span>|
|<span data-ttu-id="5c507-191">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="5c507-191">deviceProtectionOverview</span></span>|[<span data-ttu-id="5c507-192">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="5c507-192">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="5c507-193">Visão geral da proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5c507-193">Device protection overview.</span></span>|
|<span data-ttu-id="5c507-194">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="5c507-194">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="5c507-195">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="5c507-195">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="5c507-196">Regra de limpeza de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5c507-196">Device cleanup rule</span></span>|
|<span data-ttu-id="5c507-197">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="5c507-197">subscriptionState</span></span>|[<span data-ttu-id="5c507-198">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="5c507-198">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="5c507-199">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="5c507-199">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="5c507-200">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="5c507-200">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="5c507-201">assinaturas</span><span class="sxs-lookup"><span data-stu-id="5c507-201">subscriptions</span></span>|[<span data-ttu-id="5c507-202">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="5c507-202">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="5c507-203">Assinatura do locatário.</span><span class="sxs-lookup"><span data-stu-id="5c507-203">Tenant's Subscription.</span></span> <span data-ttu-id="5c507-204">Os possíveis valores são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="5c507-204">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="5c507-205">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="5c507-205">windowsMalwareOverview</span></span>|[<span data-ttu-id="5c507-206">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="5c507-206">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="5c507-207">Visão geral de malware para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="5c507-207">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="5c507-208">**Integração**</span><span class="sxs-lookup"><span data-stu-id="5c507-208">**Onboarding**</span></span>|
|<span data-ttu-id="5c507-209">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="5c507-209">intuneBrand</span></span>|[<span data-ttu-id="5c507-210">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="5c507-210">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="5c507-211">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="5c507-211">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="5c507-212">O suporte à propriedade do corpo da solicitação varia de acordo com o fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="5c507-212">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="5c507-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c507-213">Response</span></span>
<span data-ttu-id="5c507-214">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c507-214">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c507-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c507-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c507-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c507-216">Request</span></span>

<span data-ttu-id="5c507-217">Veja a seguir um exemplo de uma solicitação após o fluxo de trabalho de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="5c507-217">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="5c507-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c507-218">Response</span></span>

<span data-ttu-id="5c507-219">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c507-219">Here is an example of the response.</span></span> 

<span data-ttu-id="5c507-220">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="5c507-220">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5c507-221">As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.</span><span class="sxs-lookup"><span data-stu-id="5c507-221">Returned properties vary according to workflow and context.</span></span>

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



