---
title: Atualizar windowsDefenderAdvancedThreatProtectionConfiguration
description: Atualizar as propriedades de um objeto windowsDefenderAdvancedThreatProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b0ae580e19f2d6572fc3e48dab957bde4b1ad245
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723389"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="18a72-103">Atualizar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="18a72-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

<span data-ttu-id="18a72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18a72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18a72-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="18a72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18a72-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18a72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18a72-107">Atualizar as propriedades de um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18a72-107">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18a72-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="18a72-108">Prerequisites</span></span>
<span data-ttu-id="18a72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18a72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18a72-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18a72-111">Permission type</span></span>|<span data-ttu-id="18a72-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="18a72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18a72-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18a72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18a72-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18a72-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18a72-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18a72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18a72-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18a72-116">Not supported.</span></span>|
|<span data-ttu-id="18a72-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18a72-117">Application</span></span>|<span data-ttu-id="18a72-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18a72-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18a72-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18a72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="18a72-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18a72-120">Request headers</span></span>
|<span data-ttu-id="18a72-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18a72-121">Header</span></span>|<span data-ttu-id="18a72-122">Valor</span><span class="sxs-lookup"><span data-stu-id="18a72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18a72-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="18a72-123">Authorization</span></span>|<span data-ttu-id="18a72-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18a72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18a72-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="18a72-125">Accept</span></span>|<span data-ttu-id="18a72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18a72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18a72-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18a72-127">Request body</span></span>
<span data-ttu-id="18a72-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18a72-128">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="18a72-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18a72-129">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="18a72-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18a72-130">Property</span></span>|<span data-ttu-id="18a72-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="18a72-131">Type</span></span>|<span data-ttu-id="18a72-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="18a72-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18a72-133">id</span><span class="sxs-lookup"><span data-stu-id="18a72-133">id</span></span>|<span data-ttu-id="18a72-134">String</span><span class="sxs-lookup"><span data-stu-id="18a72-134">String</span></span>|<span data-ttu-id="18a72-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="18a72-135">Key of the entity.</span></span> <span data-ttu-id="18a72-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18a72-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a72-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18a72-137">lastModifiedDateTime</span></span>|<span data-ttu-id="18a72-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18a72-138">DateTimeOffset</span></span>|<span data-ttu-id="18a72-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="18a72-139">DateTime the object was last modified.</span></span> <span data-ttu-id="18a72-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18a72-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a72-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="18a72-141">roleScopeTagIds</span></span>|<span data-ttu-id="18a72-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="18a72-142">String collection</span></span>|<span data-ttu-id="18a72-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="18a72-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="18a72-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18a72-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a72-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="18a72-145">supportsScopeTags</span></span>|<span data-ttu-id="18a72-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="18a72-146">Boolean</span></span>|<span data-ttu-id="18a72-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="18a72-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="18a72-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="18a72-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="18a72-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="18a72-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="18a72-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="18a72-150">This property is read-only.</span></span> <span data-ttu-id="18a72-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18a72-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a72-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="18a72-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="18a72-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="18a72-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="18a72-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="18a72-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="18a72-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18a72-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a72-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="18a72-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="18a72-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="18a72-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="18a72-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="18a72-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="18a72-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18a72-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a72-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="18a72-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="18a72-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="18a72-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="18a72-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="18a72-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="18a72-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18a72-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a72-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18a72-164">createdDateTime</span></span>|<span data-ttu-id="18a72-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18a72-165">DateTimeOffset</span></span>|<span data-ttu-id="18a72-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="18a72-166">DateTime the object was created.</span></span> <span data-ttu-id="18a72-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18a72-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a72-168">description</span><span class="sxs-lookup"><span data-stu-id="18a72-168">description</span></span>|<span data-ttu-id="18a72-169">String</span><span class="sxs-lookup"><span data-stu-id="18a72-169">String</span></span>|<span data-ttu-id="18a72-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18a72-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="18a72-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18a72-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a72-172">displayName</span><span class="sxs-lookup"><span data-stu-id="18a72-172">displayName</span></span>|<span data-ttu-id="18a72-173">String</span><span class="sxs-lookup"><span data-stu-id="18a72-173">String</span></span>|<span data-ttu-id="18a72-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18a72-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="18a72-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18a72-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a72-176">versão</span><span class="sxs-lookup"><span data-stu-id="18a72-176">version</span></span>|<span data-ttu-id="18a72-177">Int32</span><span class="sxs-lookup"><span data-stu-id="18a72-177">Int32</span></span>|<span data-ttu-id="18a72-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18a72-178">Version of the device configuration.</span></span> <span data-ttu-id="18a72-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18a72-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18a72-180">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="18a72-180">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="18a72-181">String</span><span class="sxs-lookup"><span data-stu-id="18a72-181">String</span></span>|<span data-ttu-id="18a72-182">Blob de integração do Windows Defender AdvancedThreatProtection.</span><span class="sxs-lookup"><span data-stu-id="18a72-182">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="18a72-183">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="18a72-183">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="18a72-184">String</span><span class="sxs-lookup"><span data-stu-id="18a72-184">String</span></span>|<span data-ttu-id="18a72-185">Nome do arquivo do qual o AdvancedThreatProtectionOnboardingBlob foi obtido.</span><span class="sxs-lookup"><span data-stu-id="18a72-185">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="18a72-186">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="18a72-186">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="18a72-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="18a72-187">Boolean</span></span>|<span data-ttu-id="18a72-188">Preencher automaticamente o blob de integração programaticamente do serviço de proteção avançada contra ameaças</span><span class="sxs-lookup"><span data-stu-id="18a72-188">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="18a72-189">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="18a72-189">allowSampleSharing</span></span>|<span data-ttu-id="18a72-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="18a72-190">Boolean</span></span>|<span data-ttu-id="18a72-191">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="18a72-191">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="18a72-192">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="18a72-192">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="18a72-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="18a72-193">Boolean</span></span>|<span data-ttu-id="18a72-194">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="18a72-194">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="18a72-195">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="18a72-195">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="18a72-196">String</span><span class="sxs-lookup"><span data-stu-id="18a72-196">String</span></span>|<span data-ttu-id="18a72-197">Blob de remoção AdvancedThreatProtection do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="18a72-197">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="18a72-198">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="18a72-198">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="18a72-199">String</span><span class="sxs-lookup"><span data-stu-id="18a72-199">String</span></span>|<span data-ttu-id="18a72-200">Nome do arquivo do qual o AdvancedThreatProtectionOffboardingBlob foi obtido.</span><span class="sxs-lookup"><span data-stu-id="18a72-200">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="18a72-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="18a72-201">Response</span></span>
<span data-ttu-id="18a72-202">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18a72-202">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18a72-203">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18a72-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="18a72-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18a72-204">Request</span></span>
<span data-ttu-id="18a72-205">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18a72-205">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="18a72-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="18a72-206">Response</span></span>
<span data-ttu-id="18a72-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18a72-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





