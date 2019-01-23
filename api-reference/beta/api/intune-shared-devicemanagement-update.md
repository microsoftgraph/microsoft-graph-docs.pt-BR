---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f4ef1c7eb4711afd2aa29071f160f440dceefba3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415772"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="629e7-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="629e7-103">Update deviceManagement</span></span>

> <span data-ttu-id="629e7-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="629e7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="629e7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="629e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="629e7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="629e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="629e7-107">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="629e7-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="629e7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="629e7-108">Prerequisites</span></span>

<span data-ttu-id="629e7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="629e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="629e7-111">Observe que a permissão varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="629e7-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="629e7-112">Permissão&nbsp;tipo&nbsp;(por&nbsp;fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="629e7-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="629e7-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="629e7-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="629e7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="629e7-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="629e7-115">&nbsp;&nbsp; **Android para o trabalho**</span><span class="sxs-lookup"><span data-stu-id="629e7-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="629e7-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e7-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="629e7-117">&nbsp;&nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="629e7-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="629e7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e7-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="629e7-119">&nbsp;&nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="629e7-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="629e7-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e7-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="629e7-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="629e7-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="629e7-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e7-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="629e7-123">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="629e7-123">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="629e7-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e7-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="629e7-125">&nbsp;&nbsp; **SIM eletrônico**</span><span class="sxs-lookup"><span data-stu-id="629e7-125">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="629e7-126">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e7-126">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="629e7-127">&nbsp; &nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="629e7-127">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="629e7-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e7-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="629e7-129">&nbsp;&nbsp; **Fencing**</span><span class="sxs-lookup"><span data-stu-id="629e7-129">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="629e7-130">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e7-130">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="629e7-131">&nbsp; &nbsp; **Notification**</span><span class="sxs-lookup"><span data-stu-id="629e7-131">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="629e7-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e7-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="629e7-133">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="629e7-133">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="629e7-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e7-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="629e7-135">&nbsp;&nbsp; **O controle de acesso baseado em função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="629e7-135">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="629e7-136">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e7-136">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="629e7-137">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="629e7-137">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="629e7-138">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="629e7-138">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="629e7-139">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="629e7-139">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="629e7-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e7-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="629e7-141">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="629e7-141">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="629e7-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e7-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="629e7-143">&nbsp;&nbsp; **a solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="629e7-143">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="629e7-144">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e7-144">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="629e7-145">&nbsp;&nbsp; **Proteção de informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="629e7-145">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="629e7-146">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="629e7-146">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="629e7-147">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="629e7-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="629e7-148">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="629e7-148">Not supported.</span></span>|
| <span data-ttu-id="629e7-149">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="629e7-149">Application</span></span> | <span data-ttu-id="629e7-150">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="629e7-150">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="629e7-151">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="629e7-151">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="629e7-152">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="629e7-152">Request headers</span></span>

|<span data-ttu-id="629e7-153">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="629e7-153">Header</span></span>|<span data-ttu-id="629e7-154">Valor</span><span class="sxs-lookup"><span data-stu-id="629e7-154">Value</span></span>|
|:---|:---|
|<span data-ttu-id="629e7-155">Autorização</span><span class="sxs-lookup"><span data-stu-id="629e7-155">Authorization</span></span>|<span data-ttu-id="629e7-156">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="629e7-156">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="629e7-157">Aceitar</span><span class="sxs-lookup"><span data-stu-id="629e7-157">Accept</span></span>|<span data-ttu-id="629e7-158">application/json</span><span class="sxs-lookup"><span data-stu-id="629e7-158">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="629e7-159">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="629e7-159">Request body</span></span>

<span data-ttu-id="629e7-160">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="629e7-160">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="629e7-161">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="629e7-161">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="629e7-162">Propriedade</span><span class="sxs-lookup"><span data-stu-id="629e7-162">Property</span></span>|<span data-ttu-id="629e7-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="629e7-163">Type</span></span>|<span data-ttu-id="629e7-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="629e7-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="629e7-165">id</span><span class="sxs-lookup"><span data-stu-id="629e7-165">id</span></span>|<span data-ttu-id="629e7-166">String</span><span class="sxs-lookup"><span data-stu-id="629e7-166">String</span></span>|<span data-ttu-id="629e7-167">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="629e7-167">Unique identifier for the device.</span></span>|
|<span data-ttu-id="629e7-168">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="629e7-168">**Device configuration**</span></span>|
|<span data-ttu-id="629e7-169">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="629e7-169">intuneAccountId</span></span>|<span data-ttu-id="629e7-170">GUID</span><span class="sxs-lookup"><span data-stu-id="629e7-170">GUID</span></span>|<span data-ttu-id="629e7-171">ID da conta Intune para dado locatário</span><span class="sxs-lookup"><span data-stu-id="629e7-171">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="629e7-172">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="629e7-172">legacyPcManangementEnabled</span></span>|<span data-ttu-id="629e7-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="629e7-173">Boolean</span></span>|<span data-ttu-id="629e7-174">A propriedade habilitem Non-MDM gerenciados herdado gerenciamento de PC para essa conta.</span><span class="sxs-lookup"><span data-stu-id="629e7-174">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="629e7-175">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="629e7-175">This property is read-only.</span></span>|
|<span data-ttu-id="629e7-176">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="629e7-176">maximumDepTokens</span></span>|<span data-ttu-id="629e7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="629e7-177">Int32</span></span>|<span data-ttu-id="629e7-178">Número máximo de tokens DEP permitido por locatário.</span><span class="sxs-lookup"><span data-stu-id="629e7-178">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="629e7-179">configurações</span><span class="sxs-lookup"><span data-stu-id="629e7-179">settings</span></span>|[<span data-ttu-id="629e7-180">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="629e7-180">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="629e7-181">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="629e7-181">Account level settings.</span></span>|
|<span data-ttu-id="629e7-182">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="629e7-182">**Device management**</span></span>|
|<span data-ttu-id="629e7-183">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="629e7-183">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="629e7-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="629e7-184">DateTimeOffset</span></span>|<span data-ttu-id="629e7-185">A data hora & ao mover os dados de inquilinos entre scaleunits.</span><span class="sxs-lookup"><span data-stu-id="629e7-185">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="629e7-186">adminConsent</span><span class="sxs-lookup"><span data-stu-id="629e7-186">adminConsent</span></span>|[<span data-ttu-id="629e7-187">adminConsent</span><span class="sxs-lookup"><span data-stu-id="629e7-187">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="629e7-188">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="629e7-188">Admin consent information.</span></span>|
|<span data-ttu-id="629e7-189">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="629e7-189">deviceProtectionOverview</span></span>|[<span data-ttu-id="629e7-190">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="629e7-190">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="629e7-191">Visão geral de proteção do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="629e7-191">Device protection overview.</span></span>|
|<span data-ttu-id="629e7-192">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="629e7-192">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="629e7-193">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="629e7-193">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="629e7-194">Regra de limpeza do dispositivo</span><span class="sxs-lookup"><span data-stu-id="629e7-194">Device cleanup rule</span></span>|
|<span data-ttu-id="629e7-195">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="629e7-195">subscriptionState</span></span>|[<span data-ttu-id="629e7-196">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="629e7-196">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="629e7-197">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="629e7-197">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="629e7-198">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="629e7-198">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="629e7-199">assinaturas</span><span class="sxs-lookup"><span data-stu-id="629e7-199">subscriptions</span></span>|[<span data-ttu-id="629e7-200">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="629e7-200">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="629e7-201">Assinatura de locatário.</span><span class="sxs-lookup"><span data-stu-id="629e7-201">Tenant's Subscription.</span></span> <span data-ttu-id="629e7-202">Os possíveis valores são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="629e7-202">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="629e7-203">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="629e7-203">windowsMalwareOverview</span></span>|[<span data-ttu-id="629e7-204">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="629e7-204">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="629e7-205">Visão geral de malware para dispositivos do windows.</span><span class="sxs-lookup"><span data-stu-id="629e7-205">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="629e7-206">**Inclusão**</span><span class="sxs-lookup"><span data-stu-id="629e7-206">**Onboarding**</span></span>|
|<span data-ttu-id="629e7-207">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="629e7-207">intuneBrand</span></span>|[<span data-ttu-id="629e7-208">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="629e7-208">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="629e7-209">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="629e7-209">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="629e7-210">Suporte de propriedade de corpo de solicitação varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="629e7-210">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="629e7-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="629e7-211">Response</span></span>
<span data-ttu-id="629e7-212">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="629e7-212">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="629e7-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="629e7-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="629e7-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="629e7-214">Request</span></span>

<span data-ttu-id="629e7-215">Aqui está um exemplo de uma solicitação seguindo o fluxo de trabalho de gerenciamento de dispositivo:</span><span class="sxs-lookup"><span data-stu-id="629e7-215">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="629e7-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="629e7-216">Response</span></span>

<span data-ttu-id="629e7-217">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="629e7-217">Here is an example of the response.</span></span> 

<span data-ttu-id="629e7-218">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="629e7-218">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="629e7-219">Propriedades retornadas variam de acordo com o fluxo de trabalho e contexto.</span><span class="sxs-lookup"><span data-stu-id="629e7-219">Returned properties vary according to workflow and context.</span></span>

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



