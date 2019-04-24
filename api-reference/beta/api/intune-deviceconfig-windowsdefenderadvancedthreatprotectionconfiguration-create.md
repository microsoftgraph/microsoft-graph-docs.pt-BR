---
title: Criar windowsDefenderAdvancedThreatProtectionConfiguration
description: Criar um novo objeto windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5cd07f32e288fe46a4df490b23c151d3d5e9716f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32514942"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="ddd10-103">Criar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="ddd10-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="ddd10-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ddd10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddd10-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ddd10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddd10-106">Criar um novo objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ddd10-106">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddd10-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ddd10-107">Prerequisites</span></span>
<span data-ttu-id="ddd10-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddd10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddd10-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ddd10-110">Permission type</span></span>|<span data-ttu-id="ddd10-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ddd10-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddd10-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ddd10-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ddd10-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddd10-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ddd10-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ddd10-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddd10-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddd10-115">Not supported.</span></span>|
|<span data-ttu-id="ddd10-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ddd10-116">Application</span></span>|<span data-ttu-id="ddd10-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ddd10-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddd10-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ddd10-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ddd10-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ddd10-119">Request headers</span></span>
|<span data-ttu-id="ddd10-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ddd10-120">Header</span></span>|<span data-ttu-id="ddd10-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ddd10-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddd10-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ddd10-122">Authorization</span></span>|<span data-ttu-id="ddd10-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ddd10-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddd10-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ddd10-124">Accept</span></span>|<span data-ttu-id="ddd10-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ddd10-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddd10-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ddd10-126">Request body</span></span>
<span data-ttu-id="ddd10-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ddd10-127">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="ddd10-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ddd10-128">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="ddd10-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddd10-129">Property</span></span>|<span data-ttu-id="ddd10-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddd10-130">Type</span></span>|<span data-ttu-id="ddd10-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddd10-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddd10-132">id</span><span class="sxs-lookup"><span data-stu-id="ddd10-132">id</span></span>|<span data-ttu-id="ddd10-133">String</span><span class="sxs-lookup"><span data-stu-id="ddd10-133">String</span></span>|<span data-ttu-id="ddd10-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ddd10-134">Key of the entity.</span></span> <span data-ttu-id="ddd10-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddd10-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddd10-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddd10-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ddd10-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddd10-137">DateTimeOffset</span></span>|<span data-ttu-id="ddd10-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ddd10-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ddd10-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddd10-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddd10-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ddd10-140">roleScopeTagIds</span></span>|<span data-ttu-id="ddd10-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ddd10-141">String collection</span></span>|<span data-ttu-id="ddd10-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="ddd10-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ddd10-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddd10-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddd10-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ddd10-144">supportsScopeTags</span></span>|<span data-ttu-id="ddd10-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="ddd10-145">Boolean</span></span>|<span data-ttu-id="ddd10-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ddd10-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ddd10-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ddd10-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ddd10-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ddd10-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ddd10-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ddd10-149">This property is read-only.</span></span> <span data-ttu-id="ddd10-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddd10-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddd10-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ddd10-151">createdDateTime</span></span>|<span data-ttu-id="ddd10-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddd10-152">DateTimeOffset</span></span>|<span data-ttu-id="ddd10-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ddd10-153">DateTime the object was created.</span></span> <span data-ttu-id="ddd10-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddd10-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddd10-155">description</span><span class="sxs-lookup"><span data-stu-id="ddd10-155">description</span></span>|<span data-ttu-id="ddd10-156">String</span><span class="sxs-lookup"><span data-stu-id="ddd10-156">String</span></span>|<span data-ttu-id="ddd10-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ddd10-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ddd10-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddd10-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddd10-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ddd10-159">displayName</span></span>|<span data-ttu-id="ddd10-160">String</span><span class="sxs-lookup"><span data-stu-id="ddd10-160">String</span></span>|<span data-ttu-id="ddd10-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ddd10-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ddd10-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddd10-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddd10-163">versão</span><span class="sxs-lookup"><span data-stu-id="ddd10-163">version</span></span>|<span data-ttu-id="ddd10-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ddd10-164">Int32</span></span>|<span data-ttu-id="ddd10-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ddd10-165">Version of the device configuration.</span></span> <span data-ttu-id="ddd10-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddd10-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddd10-167">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="ddd10-167">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="ddd10-168">String</span><span class="sxs-lookup"><span data-stu-id="ddd10-168">String</span></span>|<span data-ttu-id="ddd10-169">Blob de integração do Windows Defender AdvancedThreatProtection.</span><span class="sxs-lookup"><span data-stu-id="ddd10-169">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="ddd10-170">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="ddd10-170">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="ddd10-171">String</span><span class="sxs-lookup"><span data-stu-id="ddd10-171">String</span></span>|<span data-ttu-id="ddd10-172">Nome do arquivo do qual o AdvancedThreatProtectionOnboardingBlob foi obtido.</span><span class="sxs-lookup"><span data-stu-id="ddd10-172">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="ddd10-173">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="ddd10-173">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="ddd10-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="ddd10-174">Boolean</span></span>|<span data-ttu-id="ddd10-175">Preencher automaticamente o blob de integração programaticamente do serviço de proteção avançada contra ameaças</span><span class="sxs-lookup"><span data-stu-id="ddd10-175">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="ddd10-176">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="ddd10-176">allowSampleSharing</span></span>|<span data-ttu-id="ddd10-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="ddd10-177">Boolean</span></span>|<span data-ttu-id="ddd10-178">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="ddd10-178">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="ddd10-179">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="ddd10-179">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="ddd10-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="ddd10-180">Boolean</span></span>|<span data-ttu-id="ddd10-181">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="ddd10-181">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="ddd10-182">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="ddd10-182">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="ddd10-183">String</span><span class="sxs-lookup"><span data-stu-id="ddd10-183">String</span></span>|<span data-ttu-id="ddd10-184">Blob de remoção AdvancedThreatProtection do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="ddd10-184">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="ddd10-185">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="ddd10-185">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="ddd10-186">String</span><span class="sxs-lookup"><span data-stu-id="ddd10-186">String</span></span>|<span data-ttu-id="ddd10-187">Nome do arquivo do qual o AdvancedThreatProtectionOffboardingBlob foi obtido.</span><span class="sxs-lookup"><span data-stu-id="ddd10-187">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="ddd10-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddd10-188">Response</span></span>
<span data-ttu-id="ddd10-189">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ddd10-189">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddd10-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ddd10-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddd10-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ddd10-191">Request</span></span>
<span data-ttu-id="ddd10-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ddd10-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 830

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="ddd10-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="ddd10-193">Response</span></span>
<span data-ttu-id="ddd10-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ddd10-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1002

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





