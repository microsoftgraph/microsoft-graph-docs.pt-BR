---
title: Criar windowsDefenderAdvancedThreatProtectionConfiguration
description: Criar um novo objeto windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7c53224373ee8ad7139ecf2b02154de16e6b1b6f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965099"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="8e5e2-103">Criar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="8e5e2-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="8e5e2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e5e2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e5e2-106">Criar um novo objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8e5e2-106">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e5e2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e5e2-107">Prerequisites</span></span>
<span data-ttu-id="8e5e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e5e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e5e2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e5e2-110">Permission type</span></span>|<span data-ttu-id="8e5e2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8e5e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e5e2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e5e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e5e2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e5e2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e5e2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e5e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e5e2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-115">Not supported.</span></span>|
|<span data-ttu-id="8e5e2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e5e2-116">Application</span></span>|<span data-ttu-id="8e5e2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e5e2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e5e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8e5e2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e5e2-119">Request headers</span></span>
|<span data-ttu-id="8e5e2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e5e2-120">Header</span></span>|<span data-ttu-id="8e5e2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8e5e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e5e2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e5e2-122">Authorization</span></span>|<span data-ttu-id="8e5e2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e5e2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e5e2-124">Accept</span></span>|<span data-ttu-id="8e5e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8e5e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e5e2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e5e2-126">Request body</span></span>
<span data-ttu-id="8e5e2-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-127">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="8e5e2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-128">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="8e5e2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e5e2-129">Property</span></span>|<span data-ttu-id="8e5e2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e5e2-130">Type</span></span>|<span data-ttu-id="8e5e2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e5e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e5e2-132">id</span><span class="sxs-lookup"><span data-stu-id="8e5e2-132">id</span></span>|<span data-ttu-id="8e5e2-133">String</span><span class="sxs-lookup"><span data-stu-id="8e5e2-133">String</span></span>|<span data-ttu-id="8e5e2-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-134">Key of the entity.</span></span> <span data-ttu-id="8e5e2-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e5e2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e5e2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e5e2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8e5e2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e5e2-137">DateTimeOffset</span></span>|<span data-ttu-id="8e5e2-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8e5e2-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e5e2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e5e2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8e5e2-140">roleScopeTagIds</span></span>|<span data-ttu-id="8e5e2-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="8e5e2-141">String collection</span></span>|<span data-ttu-id="8e5e2-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8e5e2-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e5e2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e5e2-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8e5e2-144">supportsScopeTags</span></span>|<span data-ttu-id="8e5e2-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e5e2-145">Boolean</span></span>|<span data-ttu-id="8e5e2-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8e5e2-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8e5e2-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8e5e2-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-149">This property is read-only.</span></span> <span data-ttu-id="8e5e2-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e5e2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e5e2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e5e2-151">createdDateTime</span></span>|<span data-ttu-id="8e5e2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e5e2-152">DateTimeOffset</span></span>|<span data-ttu-id="8e5e2-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-153">DateTime the object was created.</span></span> <span data-ttu-id="8e5e2-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e5e2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e5e2-155">descrição</span><span class="sxs-lookup"><span data-stu-id="8e5e2-155">description</span></span>|<span data-ttu-id="8e5e2-156">String</span><span class="sxs-lookup"><span data-stu-id="8e5e2-156">String</span></span>|<span data-ttu-id="8e5e2-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8e5e2-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e5e2-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e5e2-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8e5e2-159">displayName</span></span>|<span data-ttu-id="8e5e2-160">String</span><span class="sxs-lookup"><span data-stu-id="8e5e2-160">String</span></span>|<span data-ttu-id="8e5e2-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8e5e2-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e5e2-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e5e2-163">versão</span><span class="sxs-lookup"><span data-stu-id="8e5e2-163">version</span></span>|<span data-ttu-id="8e5e2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8e5e2-164">Int32</span></span>|<span data-ttu-id="8e5e2-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-165">Version of the device configuration.</span></span> <span data-ttu-id="8e5e2-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8e5e2-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8e5e2-167">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="8e5e2-167">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="8e5e2-168">String</span><span class="sxs-lookup"><span data-stu-id="8e5e2-168">String</span></span>|<span data-ttu-id="8e5e2-169">Blob de integração do Windows Defender AdvancedThreatProtection.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-169">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="8e5e2-170">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="8e5e2-170">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="8e5e2-171">String</span><span class="sxs-lookup"><span data-stu-id="8e5e2-171">String</span></span>|<span data-ttu-id="8e5e2-172">Nome do arquivo do qual o AdvancedThreatProtectionOnboardingBlob foi obtido.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-172">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="8e5e2-173">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="8e5e2-173">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="8e5e2-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e5e2-174">Boolean</span></span>|<span data-ttu-id="8e5e2-175">Preencher automaticamente o blob de integração programaticamente do serviço de proteção avançada contra ameaças</span><span class="sxs-lookup"><span data-stu-id="8e5e2-175">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="8e5e2-176">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="8e5e2-176">allowSampleSharing</span></span>|<span data-ttu-id="8e5e2-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e5e2-177">Boolean</span></span>|<span data-ttu-id="8e5e2-178">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="8e5e2-178">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="8e5e2-179">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="8e5e2-179">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="8e5e2-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="8e5e2-180">Boolean</span></span>|<span data-ttu-id="8e5e2-181">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-181">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="8e5e2-182">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="8e5e2-182">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="8e5e2-183">String</span><span class="sxs-lookup"><span data-stu-id="8e5e2-183">String</span></span>|<span data-ttu-id="8e5e2-184">Blob de remoção AdvancedThreatProtection do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-184">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="8e5e2-185">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="8e5e2-185">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="8e5e2-186">String</span><span class="sxs-lookup"><span data-stu-id="8e5e2-186">String</span></span>|<span data-ttu-id="8e5e2-187">Nome do arquivo do qual o AdvancedThreatProtectionOffboardingBlob foi obtido.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-187">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="8e5e2-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e5e2-188">Response</span></span>
<span data-ttu-id="8e5e2-189">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-189">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e5e2-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e5e2-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e5e2-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e5e2-191">Request</span></span>
<span data-ttu-id="8e5e2-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8e5e2-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e5e2-193">Response</span></span>
<span data-ttu-id="8e5e2-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e5e2-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




