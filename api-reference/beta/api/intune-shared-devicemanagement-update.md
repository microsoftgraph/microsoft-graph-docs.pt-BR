---
title: Atualizar deviceManagement
description: Atualizar as propriedades de um objeto deviceManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f4ef1c7eb4711afd2aa29071f160f440dceefba3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960402"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="00a90-103">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="00a90-103">Update deviceManagement</span></span>

> <span data-ttu-id="00a90-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="00a90-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="00a90-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="00a90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00a90-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="00a90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00a90-107">Atualizar as propriedades de um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="00a90-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00a90-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="00a90-108">Prerequisites</span></span>

<span data-ttu-id="00a90-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00a90-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="00a90-111">Observe que a permissão varia de acordo com o fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="00a90-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="00a90-112">Tipo&nbsp;&nbsp;de permissão (&nbsp;por fluxo de trabalho)</span><span class="sxs-lookup"><span data-stu-id="00a90-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="00a90-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="00a90-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="00a90-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00a90-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="00a90-115">&nbsp;&nbsp; **Android para trabalho**</span><span class="sxs-lookup"><span data-stu-id="00a90-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="00a90-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a90-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="00a90-117">&nbsp; &nbsp; **Auditoria**</span><span class="sxs-lookup"><span data-stu-id="00a90-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="00a90-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a90-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="00a90-119">&nbsp; &nbsp; **Termos da empresa**</span><span class="sxs-lookup"><span data-stu-id="00a90-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="00a90-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a90-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00a90-121">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="00a90-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="00a90-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a90-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="00a90-123">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="00a90-123">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="00a90-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a90-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="00a90-125">&nbsp;&nbsp; **Sim eletrônico**</span><span class="sxs-lookup"><span data-stu-id="00a90-125">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="00a90-126">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a90-126">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="00a90-127">&nbsp;&nbsp; **Registro**</span><span class="sxs-lookup"><span data-stu-id="00a90-127">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="00a90-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a90-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00a90-129">&nbsp;&nbsp; **Isolamento**</span><span class="sxs-lookup"><span data-stu-id="00a90-129">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="00a90-130">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a90-130">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="00a90-131">&nbsp; &nbsp; **Notificação**</span><span class="sxs-lookup"><span data-stu-id="00a90-131">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="00a90-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a90-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00a90-133">&nbsp; &nbsp; **Integração**</span><span class="sxs-lookup"><span data-stu-id="00a90-133">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="00a90-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a90-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00a90-135">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="00a90-135">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="00a90-136">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a90-136">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="00a90-137">&nbsp;&nbsp; **Acesso remoto**</span><span class="sxs-lookup"><span data-stu-id="00a90-137">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="00a90-138">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="00a90-138">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="00a90-139">&nbsp;&nbsp; **Assistência remota**</span><span class="sxs-lookup"><span data-stu-id="00a90-139">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="00a90-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a90-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00a90-141">&nbsp;&nbsp; **Gerenciamento de despesas de telecomunicações**</span><span class="sxs-lookup"><span data-stu-id="00a90-141">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="00a90-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a90-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="00a90-143">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="00a90-143">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="00a90-144">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a90-144">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="00a90-145">&nbsp;&nbsp; **Proteção de informações do Windows**</span><span class="sxs-lookup"><span data-stu-id="00a90-145">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="00a90-146">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00a90-146">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="00a90-147">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00a90-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00a90-148">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00a90-148">Not supported.</span></span>|
| <span data-ttu-id="00a90-149">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00a90-149">Application</span></span> | <span data-ttu-id="00a90-150">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00a90-150">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00a90-151">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00a90-151">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="00a90-152">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00a90-152">Request headers</span></span>

|<span data-ttu-id="00a90-153">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="00a90-153">Header</span></span>|<span data-ttu-id="00a90-154">Valor</span><span class="sxs-lookup"><span data-stu-id="00a90-154">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00a90-155">Autorização</span><span class="sxs-lookup"><span data-stu-id="00a90-155">Authorization</span></span>|<span data-ttu-id="00a90-156">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00a90-156">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00a90-157">Aceitar</span><span class="sxs-lookup"><span data-stu-id="00a90-157">Accept</span></span>|<span data-ttu-id="00a90-158">application/json</span><span class="sxs-lookup"><span data-stu-id="00a90-158">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00a90-159">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00a90-159">Request body</span></span>

<span data-ttu-id="00a90-160">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="00a90-160">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="00a90-161">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagement](../resources/intune-shared-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="00a90-161">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="00a90-162">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00a90-162">Property</span></span>|<span data-ttu-id="00a90-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="00a90-163">Type</span></span>|<span data-ttu-id="00a90-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="00a90-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00a90-165">id</span><span class="sxs-lookup"><span data-stu-id="00a90-165">id</span></span>|<span data-ttu-id="00a90-166">String</span><span class="sxs-lookup"><span data-stu-id="00a90-166">String</span></span>|<span data-ttu-id="00a90-167">Identificador exclusivo do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00a90-167">Unique identifier for the device.</span></span>|
|<span data-ttu-id="00a90-168">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="00a90-168">**Device configuration**</span></span>|
|<span data-ttu-id="00a90-169">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="00a90-169">intuneAccountId</span></span>|<span data-ttu-id="00a90-170">GUID</span><span class="sxs-lookup"><span data-stu-id="00a90-170">GUID</span></span>|<span data-ttu-id="00a90-171">ID da conta do Intune para determinado locatário</span><span class="sxs-lookup"><span data-stu-id="00a90-171">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="00a90-172">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="00a90-172">legacyPcManangementEnabled</span></span>|<span data-ttu-id="00a90-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="00a90-173">Boolean</span></span>|<span data-ttu-id="00a90-174">A propriedade para habilitar o gerenciamento de computador herdado não MDM gerenciado para esta conta.</span><span class="sxs-lookup"><span data-stu-id="00a90-174">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="00a90-175">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="00a90-175">This property is read-only.</span></span>|
|<span data-ttu-id="00a90-176">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="00a90-176">maximumDepTokens</span></span>|<span data-ttu-id="00a90-177">Int32</span><span class="sxs-lookup"><span data-stu-id="00a90-177">Int32</span></span>|<span data-ttu-id="00a90-178">Número máximo de tokens DEP permitidos por locatário.</span><span class="sxs-lookup"><span data-stu-id="00a90-178">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="00a90-179">settings</span><span class="sxs-lookup"><span data-stu-id="00a90-179">settings</span></span>|[<span data-ttu-id="00a90-180">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="00a90-180">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="00a90-181">Configurações de nível da conta.</span><span class="sxs-lookup"><span data-stu-id="00a90-181">Account level settings.</span></span>|
|<span data-ttu-id="00a90-182">**Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="00a90-182">**Device management**</span></span>|
|<span data-ttu-id="00a90-183">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="00a90-183">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="00a90-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00a90-184">DateTimeOffset</span></span>|<span data-ttu-id="00a90-185">A data & hora em que os dados do locatário são movidos entre ScaleUnits.</span><span class="sxs-lookup"><span data-stu-id="00a90-185">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="00a90-186">adminConsent</span><span class="sxs-lookup"><span data-stu-id="00a90-186">adminConsent</span></span>|[<span data-ttu-id="00a90-187">adminConsent</span><span class="sxs-lookup"><span data-stu-id="00a90-187">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="00a90-188">Informações de consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="00a90-188">Admin consent information.</span></span>|
|<span data-ttu-id="00a90-189">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="00a90-189">deviceProtectionOverview</span></span>|[<span data-ttu-id="00a90-190">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="00a90-190">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="00a90-191">Visão geral da proteção de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="00a90-191">Device protection overview.</span></span>|
|<span data-ttu-id="00a90-192">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="00a90-192">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="00a90-193">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="00a90-193">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="00a90-194">Regra de limpeza de dispositivo</span><span class="sxs-lookup"><span data-stu-id="00a90-194">Device cleanup rule</span></span>|
|<span data-ttu-id="00a90-195">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="00a90-195">subscriptionState</span></span>|[<span data-ttu-id="00a90-196">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="00a90-196">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="00a90-197">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="00a90-197">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="00a90-198">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="00a90-198">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="00a90-199">assinaturas</span><span class="sxs-lookup"><span data-stu-id="00a90-199">subscriptions</span></span>|[<span data-ttu-id="00a90-200">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="00a90-200">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="00a90-201">Assinatura do locatário.</span><span class="sxs-lookup"><span data-stu-id="00a90-201">Tenant's Subscription.</span></span> <span data-ttu-id="00a90-202">Os valores possíveis são: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span><span class="sxs-lookup"><span data-stu-id="00a90-202">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="00a90-203">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="00a90-203">windowsMalwareOverview</span></span>|[<span data-ttu-id="00a90-204">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="00a90-204">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="00a90-205">Visão geral de malware para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="00a90-205">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="00a90-206">**Integração**</span><span class="sxs-lookup"><span data-stu-id="00a90-206">**Onboarding**</span></span>|
|<span data-ttu-id="00a90-207">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="00a90-207">intuneBrand</span></span>|[<span data-ttu-id="00a90-208">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="00a90-208">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="00a90-209">intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.</span><span class="sxs-lookup"><span data-stu-id="00a90-209">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="00a90-210">O suporte à propriedade do corpo da solicitação varia de acordo com o fluxo de trabalho</span><span class="sxs-lookup"><span data-stu-id="00a90-210">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="00a90-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="00a90-211">Response</span></span>
<span data-ttu-id="00a90-212">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceManagement](../resources/intune-shared-devicemanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00a90-212">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00a90-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00a90-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="00a90-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00a90-214">Request</span></span>

<span data-ttu-id="00a90-215">Veja a seguir um exemplo de uma solicitação após o fluxo de trabalho de gerenciamento de dispositivos:</span><span class="sxs-lookup"><span data-stu-id="00a90-215">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="00a90-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="00a90-216">Response</span></span>

<span data-ttu-id="00a90-217">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00a90-217">Here is an example of the response.</span></span> 

<span data-ttu-id="00a90-218">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="00a90-218">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="00a90-219">As propriedades retornadas variam de acordo com o fluxo de trabalho e o contexto.</span><span class="sxs-lookup"><span data-stu-id="00a90-219">Returned properties vary according to workflow and context.</span></span>

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



