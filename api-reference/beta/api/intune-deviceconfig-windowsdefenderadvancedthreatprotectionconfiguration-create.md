---
title: Criar windowsDefenderAdvancedThreatProtectionConfiguration
description: Criar um novo objeto windowsDefenderAdvancedThreatProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e1cdcd1eae258f714e9cad0a64eda8a5a3e39c64
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946886"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="29969-103">Criar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="29969-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="29969-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29969-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29969-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29969-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29969-106">Criar um novo objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="29969-106">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29969-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29969-107">Prerequisites</span></span>
<span data-ttu-id="29969-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29969-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29969-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29969-110">Permission type</span></span>|<span data-ttu-id="29969-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="29969-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29969-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29969-112">Delegated (work or school account)</span></span>|<span data-ttu-id="29969-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29969-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="29969-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29969-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29969-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29969-115">Not supported.</span></span>|
|<span data-ttu-id="29969-116">Application</span><span class="sxs-lookup"><span data-stu-id="29969-116">Application</span></span>|<span data-ttu-id="29969-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29969-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29969-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29969-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="29969-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29969-119">Request headers</span></span>
|<span data-ttu-id="29969-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29969-120">Header</span></span>|<span data-ttu-id="29969-121">Valor</span><span class="sxs-lookup"><span data-stu-id="29969-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29969-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="29969-122">Authorization</span></span>|<span data-ttu-id="29969-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29969-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29969-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29969-124">Accept</span></span>|<span data-ttu-id="29969-125">application/json</span><span class="sxs-lookup"><span data-stu-id="29969-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29969-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29969-126">Request body</span></span>
<span data-ttu-id="29969-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="29969-127">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="29969-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="29969-128">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="29969-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29969-129">Property</span></span>|<span data-ttu-id="29969-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="29969-130">Type</span></span>|<span data-ttu-id="29969-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="29969-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29969-132">id</span><span class="sxs-lookup"><span data-stu-id="29969-132">id</span></span>|<span data-ttu-id="29969-133">String</span><span class="sxs-lookup"><span data-stu-id="29969-133">String</span></span>|<span data-ttu-id="29969-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="29969-134">Key of the entity.</span></span> <span data-ttu-id="29969-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29969-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29969-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29969-136">lastModifiedDateTime</span></span>|<span data-ttu-id="29969-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29969-137">DateTimeOffset</span></span>|<span data-ttu-id="29969-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="29969-138">DateTime the object was last modified.</span></span> <span data-ttu-id="29969-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29969-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29969-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="29969-140">roleScopeTagIds</span></span>|<span data-ttu-id="29969-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="29969-141">String collection</span></span>|<span data-ttu-id="29969-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="29969-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="29969-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29969-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29969-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="29969-144">supportsScopeTags</span></span>|<span data-ttu-id="29969-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="29969-145">Boolean</span></span>|<span data-ttu-id="29969-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="29969-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="29969-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="29969-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="29969-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="29969-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="29969-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="29969-149">This property is read-only.</span></span> <span data-ttu-id="29969-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29969-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29969-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="29969-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="29969-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="29969-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="29969-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="29969-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="29969-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29969-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29969-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="29969-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="29969-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="29969-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="29969-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="29969-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="29969-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29969-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29969-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="29969-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="29969-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="29969-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="29969-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="29969-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="29969-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29969-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29969-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29969-163">createdDateTime</span></span>|<span data-ttu-id="29969-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29969-164">DateTimeOffset</span></span>|<span data-ttu-id="29969-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="29969-165">DateTime the object was created.</span></span> <span data-ttu-id="29969-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29969-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29969-167">description</span><span class="sxs-lookup"><span data-stu-id="29969-167">description</span></span>|<span data-ttu-id="29969-168">String</span><span class="sxs-lookup"><span data-stu-id="29969-168">String</span></span>|<span data-ttu-id="29969-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="29969-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="29969-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29969-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29969-171">displayName</span><span class="sxs-lookup"><span data-stu-id="29969-171">displayName</span></span>|<span data-ttu-id="29969-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29969-172">String</span></span>|<span data-ttu-id="29969-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="29969-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="29969-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29969-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29969-175">versão</span><span class="sxs-lookup"><span data-stu-id="29969-175">version</span></span>|<span data-ttu-id="29969-176">Int32</span><span class="sxs-lookup"><span data-stu-id="29969-176">Int32</span></span>|<span data-ttu-id="29969-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="29969-177">Version of the device configuration.</span></span> <span data-ttu-id="29969-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="29969-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="29969-179">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="29969-179">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="29969-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="29969-180">String</span></span>|<span data-ttu-id="29969-181">Blob de integração do Windows Defender AdvancedThreatProtection.</span><span class="sxs-lookup"><span data-stu-id="29969-181">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="29969-182">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="29969-182">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="29969-183">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="29969-183">String</span></span>|<span data-ttu-id="29969-184">Nome do arquivo do qual o AdvancedThreatProtectionOnboardingBlob foi obtido.</span><span class="sxs-lookup"><span data-stu-id="29969-184">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="29969-185">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="29969-185">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="29969-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="29969-186">Boolean</span></span>|<span data-ttu-id="29969-187">Preencher automaticamente o blob de integração programaticamente do serviço de proteção avançada contra ameaças</span><span class="sxs-lookup"><span data-stu-id="29969-187">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="29969-188">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="29969-188">allowSampleSharing</span></span>|<span data-ttu-id="29969-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="29969-189">Boolean</span></span>|<span data-ttu-id="29969-190">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="29969-190">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="29969-191">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="29969-191">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="29969-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="29969-192">Boolean</span></span>|<span data-ttu-id="29969-193">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="29969-193">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="29969-194">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="29969-194">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="29969-195">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="29969-195">String</span></span>|<span data-ttu-id="29969-196">Blob de remoção AdvancedThreatProtection do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="29969-196">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="29969-197">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="29969-197">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="29969-198">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="29969-198">String</span></span>|<span data-ttu-id="29969-199">Nome do arquivo do qual o AdvancedThreatProtectionOffboardingBlob foi obtido.</span><span class="sxs-lookup"><span data-stu-id="29969-199">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="29969-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="29969-200">Response</span></span>
<span data-ttu-id="29969-201">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29969-201">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29969-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29969-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="29969-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29969-203">Request</span></span>
<span data-ttu-id="29969-204">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29969-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="29969-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="29969-205">Response</span></span>
<span data-ttu-id="29969-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29969-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





