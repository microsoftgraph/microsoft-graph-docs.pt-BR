---
title: Atualizar windowsDefenderAdvancedThreatProtectionConfiguration
description: Atualizar as propriedades de um objeto windowsDefenderAdvancedThreatProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8015919cd1bc9f84c7495f3e36fb9f1d8a78a47
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962026"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="9e810-103">Atualizar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e810-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="9e810-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9e810-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e810-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e810-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e810-106">Atualizar as propriedades de um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e810-106">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e810-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e810-107">Prerequisites</span></span>
<span data-ttu-id="9e810-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e810-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e810-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e810-110">Permission type</span></span>|<span data-ttu-id="9e810-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9e810-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e810-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e810-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e810-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e810-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e810-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e810-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e810-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e810-115">Not supported.</span></span>|
|<span data-ttu-id="9e810-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e810-116">Application</span></span>|<span data-ttu-id="9e810-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e810-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e810-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e810-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9e810-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e810-119">Request headers</span></span>
|<span data-ttu-id="9e810-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e810-120">Header</span></span>|<span data-ttu-id="9e810-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9e810-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e810-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e810-122">Authorization</span></span>|<span data-ttu-id="9e810-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e810-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e810-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9e810-124">Accept</span></span>|<span data-ttu-id="9e810-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e810-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e810-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e810-126">Request body</span></span>
<span data-ttu-id="9e810-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e810-127">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="9e810-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e810-128">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="9e810-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e810-129">Property</span></span>|<span data-ttu-id="9e810-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e810-130">Type</span></span>|<span data-ttu-id="9e810-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e810-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e810-132">id</span><span class="sxs-lookup"><span data-stu-id="9e810-132">id</span></span>|<span data-ttu-id="9e810-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e810-133">String</span></span>|<span data-ttu-id="9e810-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9e810-134">Key of the entity.</span></span> <span data-ttu-id="9e810-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e810-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e810-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e810-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9e810-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e810-137">DateTimeOffset</span></span>|<span data-ttu-id="9e810-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9e810-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9e810-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e810-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e810-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9e810-140">roleScopeTagIds</span></span>|<span data-ttu-id="9e810-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e810-141">String collection</span></span>|<span data-ttu-id="9e810-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="9e810-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9e810-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e810-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e810-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9e810-144">supportsScopeTags</span></span>|<span data-ttu-id="9e810-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e810-145">Boolean</span></span>|<span data-ttu-id="9e810-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9e810-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9e810-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9e810-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9e810-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9e810-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9e810-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e810-149">This property is read-only.</span></span> <span data-ttu-id="9e810-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e810-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e810-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9e810-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9e810-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9e810-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9e810-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="9e810-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9e810-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e810-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e810-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9e810-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9e810-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9e810-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9e810-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="9e810-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9e810-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e810-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e810-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9e810-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9e810-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9e810-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9e810-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="9e810-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9e810-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e810-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e810-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e810-163">createdDateTime</span></span>|<span data-ttu-id="9e810-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e810-164">DateTimeOffset</span></span>|<span data-ttu-id="9e810-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9e810-165">DateTime the object was created.</span></span> <span data-ttu-id="9e810-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e810-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e810-167">descrição</span><span class="sxs-lookup"><span data-stu-id="9e810-167">description</span></span>|<span data-ttu-id="9e810-168">String</span><span class="sxs-lookup"><span data-stu-id="9e810-168">String</span></span>|<span data-ttu-id="9e810-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e810-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9e810-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e810-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e810-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9e810-171">displayName</span></span>|<span data-ttu-id="9e810-172">String</span><span class="sxs-lookup"><span data-stu-id="9e810-172">String</span></span>|<span data-ttu-id="9e810-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e810-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9e810-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e810-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e810-175">versão</span><span class="sxs-lookup"><span data-stu-id="9e810-175">version</span></span>|<span data-ttu-id="9e810-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9e810-176">Int32</span></span>|<span data-ttu-id="9e810-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e810-177">Version of the device configuration.</span></span> <span data-ttu-id="9e810-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e810-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e810-179">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="9e810-179">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="9e810-180">String</span><span class="sxs-lookup"><span data-stu-id="9e810-180">String</span></span>|<span data-ttu-id="9e810-181">Blob de integração do Windows Defender AdvancedThreatProtection.</span><span class="sxs-lookup"><span data-stu-id="9e810-181">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="9e810-182">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="9e810-182">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="9e810-183">String</span><span class="sxs-lookup"><span data-stu-id="9e810-183">String</span></span>|<span data-ttu-id="9e810-184">Nome do arquivo do qual o AdvancedThreatProtectionOnboardingBlob foi obtido.</span><span class="sxs-lookup"><span data-stu-id="9e810-184">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="9e810-185">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="9e810-185">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="9e810-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e810-186">Boolean</span></span>|<span data-ttu-id="9e810-187">Preencher automaticamente o blob de integração programaticamente do serviço de proteção avançada contra ameaças</span><span class="sxs-lookup"><span data-stu-id="9e810-187">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="9e810-188">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="9e810-188">allowSampleSharing</span></span>|<span data-ttu-id="9e810-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e810-189">Boolean</span></span>|<span data-ttu-id="9e810-190">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="9e810-190">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="9e810-191">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="9e810-191">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="9e810-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e810-192">Boolean</span></span>|<span data-ttu-id="9e810-193">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="9e810-193">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="9e810-194">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="9e810-194">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="9e810-195">String</span><span class="sxs-lookup"><span data-stu-id="9e810-195">String</span></span>|<span data-ttu-id="9e810-196">Blob de remoção AdvancedThreatProtection do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="9e810-196">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="9e810-197">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="9e810-197">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="9e810-198">String</span><span class="sxs-lookup"><span data-stu-id="9e810-198">String</span></span>|<span data-ttu-id="9e810-199">Nome do arquivo do qual o AdvancedThreatProtectionOffboardingBlob foi obtido.</span><span class="sxs-lookup"><span data-stu-id="9e810-199">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="9e810-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e810-200">Response</span></span>
<span data-ttu-id="9e810-201">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e810-201">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e810-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e810-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e810-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e810-203">Request</span></span>
<span data-ttu-id="9e810-204">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e810-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1603

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "advancedThreatProtectionOnboardingBlob": "Advanced Threat Protection Onboarding Blob value",
  "advancedThreatProtectionOnboardingFilename": "Advanced Threat Protection Onboarding Filename value",
  "advancedThreatProtectionAutoPopulateOnboardingBlob": true,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true,
  "advancedThreatProtectionOffboardingBlob": "Advanced Threat Protection Offboarding Blob value",
  "advancedThreatProtectionOffboardingFilename": "Advanced Threat Protection Offboarding Filename value"
}
```

### <a name="response"></a><span data-ttu-id="9e810-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e810-205">Response</span></span>
<span data-ttu-id="9e810-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e810-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1775

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "advancedThreatProtectionOnboardingBlob": "Advanced Threat Protection Onboarding Blob value",
  "advancedThreatProtectionOnboardingFilename": "Advanced Threat Protection Onboarding Filename value",
  "advancedThreatProtectionAutoPopulateOnboardingBlob": true,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true,
  "advancedThreatProtectionOffboardingBlob": "Advanced Threat Protection Offboarding Blob value",
  "advancedThreatProtectionOffboardingFilename": "Advanced Threat Protection Offboarding Filename value"
}
```





