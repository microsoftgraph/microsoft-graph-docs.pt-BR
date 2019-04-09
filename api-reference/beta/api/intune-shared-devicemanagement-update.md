---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e0dc83489ede464eb9da000acb8db4e6af13f8d2
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31518522"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="30904-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="30904-103">Update deviceManagement</span></span>

> <span data-ttu-id="30904-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="30904-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="30904-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="30904-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30904-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30904-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30904-107">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="30904-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30904-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30904-108">Prerequisites</span></span>

<span data-ttu-id="30904-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30904-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="30904-111">Observe que a permissão varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="30904-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="30904-112">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="30904-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="30904-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30904-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="30904-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30904-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="30904-115">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="30904-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="30904-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30904-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="30904-117">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="30904-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="30904-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30904-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="30904-119">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="30904-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="30904-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30904-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="30904-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="30904-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="30904-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30904-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="30904-123">&nbsp;&nbsp; **Intenção do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="30904-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="30904-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30904-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="30904-125">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="30904-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="30904-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30904-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="30904-127">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="30904-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="30904-128">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30904-128">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="30904-129">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="30904-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="30904-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30904-130">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="30904-131">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="30904-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="30904-132">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30904-132">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="30904-133">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="30904-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="30904-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30904-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="30904-135">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="30904-135">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="30904-136">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30904-136">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="30904-137">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="30904-137">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="30904-138">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30904-138">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="30904-139">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="30904-139">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="30904-140">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="30904-140">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="30904-141">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="30904-141">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="30904-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30904-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="30904-143">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="30904-143">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="30904-144">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30904-144">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="30904-145">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="30904-145">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="30904-146">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30904-146">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="30904-147">&nbsp; &nbsp; **Proteção de Informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="30904-147">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="30904-148">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30904-148">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="30904-149">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30904-149">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30904-150">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30904-150">Not supported.</span></span>|
| <span data-ttu-id="30904-151">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30904-151">Application</span></span> | <span data-ttu-id="30904-152">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30904-152">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="30904-153">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30904-153">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="30904-154">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30904-154">Request headers</span></span>

|<span data-ttu-id="30904-155">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30904-155">Header</span></span>|<span data-ttu-id="30904-156">Valor</span><span class="sxs-lookup"><span data-stu-id="30904-156">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30904-157">Autorização</span><span class="sxs-lookup"><span data-stu-id="30904-157">Authorization</span></span>|<span data-ttu-id="30904-158">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30904-158">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30904-159">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30904-159">Accept</span></span>|<span data-ttu-id="30904-160">application/json</span><span class="sxs-lookup"><span data-stu-id="30904-160">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30904-161">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30904-161">Request body</span></span>

<span data-ttu-id="30904-162">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="30904-162">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="30904-163">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="30904-163">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="30904-164">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30904-164">Property</span></span>|<span data-ttu-id="30904-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="30904-165">Type</span></span>|<span data-ttu-id="30904-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="30904-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30904-167">id</span><span class="sxs-lookup"><span data-stu-id="30904-167">id</span></span>|<span data-ttu-id="30904-168">String</span><span class="sxs-lookup"><span data-stu-id="30904-168">String</span></span>|<span data-ttu-id="30904-169">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="30904-169">Unique identifier for the device.</span></span>|
|**<span data-ttu-id="30904-170">Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="30904-170">Device configuration</span></span>**|
|<span data-ttu-id="30904-171">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="30904-171">intuneAccountId</span></span>|<span data-ttu-id="30904-172">GUID</span><span class="sxs-lookup"><span data-stu-id="30904-172">GUID</span></span>|<span data-ttu-id="30904-173">ID da conta do Intune para determinado locatário</span><span class="sxs-lookup"><span data-stu-id="30904-173">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="30904-174">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="30904-174">legacyPcManangementEnabled</span></span>|<span data-ttu-id="30904-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="30904-175">Boolean</span></span>|<span data-ttu-id="30904-176">A propriedade para habilitar o gerenciamento de computador herdado não MDM gerenciado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="30904-176">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="30904-177">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="30904-177">This property is read-only.</span></span>|
|<span data-ttu-id="30904-178">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="30904-178">maximumDepTokens</span></span>|<span data-ttu-id="30904-179">Int32</span><span class="sxs-lookup"><span data-stu-id="30904-179">Int32</span></span>|<span data-ttu-id="30904-180">Número máximo de tokens DEP permitidos por locatário.</span><span class="sxs-lookup"><span data-stu-id="30904-180">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="30904-181">settings</span><span class="sxs-lookup"><span data-stu-id="30904-181">settings</span></span>|[<span data-ttu-id="30904-182">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="30904-182">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="30904-183">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="30904-183">Account level settings.</span></span>|
|**<span data-ttu-id="30904-184">Gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="30904-184">Device management</span></span>**|
|<span data-ttu-id="30904-185">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="30904-185">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="30904-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30904-186">DateTimeOffset</span></span>|<span data-ttu-id="30904-187">A data & hora em que os dados do locatário são movidos entre ScaleUnits.</span><span class="sxs-lookup"><span data-stu-id="30904-187">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="30904-188">adminConsent</span><span class="sxs-lookup"><span data-stu-id="30904-188">adminConsent</span></span>|[<span data-ttu-id="30904-189">adminConsent</span><span class="sxs-lookup"><span data-stu-id="30904-189">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="30904-190">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="30904-190">Admin consent information.</span></span>|
|<span data-ttu-id="30904-191">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="30904-191">deviceProtectionOverview</span></span>|[<span data-ttu-id="30904-192">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="30904-192">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="30904-193">Visão geral da proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="30904-193">Device protection overview.</span></span>|
|<span data-ttu-id="30904-194">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="30904-194">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="30904-195">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="30904-195">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="30904-196">Regra de limpeza de dispositivo</span><span class="sxs-lookup"><span data-stu-id="30904-196">Device cleanup rule</span></span>|
|<span data-ttu-id="30904-197">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="30904-197">subscriptionState</span></span>|[<span data-ttu-id="30904-198">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="30904-198">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="30904-199">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="30904-199">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="30904-200">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="30904-200">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="30904-201">assinaturas</span><span class="sxs-lookup"><span data-stu-id="30904-201">subscriptions</span></span>|[<span data-ttu-id="30904-202">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="30904-202">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="30904-203">Assinatura do locatário.</span><span class="sxs-lookup"><span data-stu-id="30904-203">Tenant's Subscription.</span></span> <span data-ttu-id="30904-204">Os valores possíveis são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="30904-204">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="30904-205">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="30904-205">windowsMalwareOverview</span></span>|[<span data-ttu-id="30904-206">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="30904-206">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="30904-207">Visão geral de malware para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="30904-207">Malware overview for windows devices.</span></span>|
|**<span data-ttu-id="30904-208">Integração</span><span class="sxs-lookup"><span data-stu-id="30904-208">Onboarding</span></span>**|
|<span data-ttu-id="30904-209">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="30904-209">intuneBrand</span></span>|[<span data-ttu-id="30904-210">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="30904-210">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="30904-211">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="30904-211">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="30904-212">O suporte à propriedade do corpo da solicitação varia de acordo com o fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="30904-212">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="30904-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="30904-213">Response</span></span>
<span data-ttu-id="30904-214">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30904-214">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30904-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30904-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="30904-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30904-216">Request</span></span>

<span data-ttu-id="30904-217">Veja a seguir um exemplo de uma solicitação após o fluxo de trabalho de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="30904-217">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="30904-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="30904-218">Response</span></span>

<span data-ttu-id="30904-219">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30904-219">Here is an example of the response.</span></span> 

<span data-ttu-id="30904-220">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="30904-220">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="30904-221">As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.</span><span class="sxs-lookup"><span data-stu-id="30904-221">Returned properties vary according to workflow and context.</span></span>

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



