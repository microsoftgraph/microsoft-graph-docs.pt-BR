---
title: Atualizar windowsDefenderAdvancedThreatProtectionConfiguration
description: Atualizar as propriedades de um objeto windowsDefenderAdvancedThreatProtectionConfiguration.
ms.openlocfilehash: b21ad952d5b8abefc9d4c6bb275474437aceefa8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037944"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="a1126-103">Atualizar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1126-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="a1126-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a1126-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1126-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a1126-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1126-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a1126-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1126-107">Atualizar as propriedades de um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1126-107">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1126-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1126-108">Prerequisites</span></span>
<span data-ttu-id="a1126-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1126-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1126-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1126-111">Permission type</span></span>|<span data-ttu-id="a1126-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1126-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1126-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1126-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1126-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1126-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1126-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1126-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1126-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1126-116">Not supported.</span></span>|
|<span data-ttu-id="a1126-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1126-117">Application</span></span>|<span data-ttu-id="a1126-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1126-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1126-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1126-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a1126-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1126-120">Request headers</span></span>
|<span data-ttu-id="a1126-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1126-121">Header</span></span>|<span data-ttu-id="a1126-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a1126-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1126-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1126-123">Authorization</span></span>|<span data-ttu-id="a1126-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1126-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1126-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a1126-125">Accept</span></span>|<span data-ttu-id="a1126-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1126-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1126-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1126-127">Request body</span></span>
<span data-ttu-id="a1126-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1126-128">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="a1126-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1126-129">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="a1126-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1126-130">Property</span></span>|<span data-ttu-id="a1126-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1126-131">Type</span></span>|<span data-ttu-id="a1126-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1126-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1126-133">id</span><span class="sxs-lookup"><span data-stu-id="a1126-133">id</span></span>|<span data-ttu-id="a1126-134">String</span><span class="sxs-lookup"><span data-stu-id="a1126-134">String</span></span>|<span data-ttu-id="a1126-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a1126-135">Key of the entity.</span></span> <span data-ttu-id="a1126-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1126-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1126-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1126-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a1126-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1126-138">DateTimeOffset</span></span>|<span data-ttu-id="a1126-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a1126-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a1126-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1126-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1126-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a1126-141">roleScopeTagIds</span></span>|<span data-ttu-id="a1126-142">String collection</span><span class="sxs-lookup"><span data-stu-id="a1126-142">String collection</span></span>|<span data-ttu-id="a1126-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="a1126-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a1126-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1126-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1126-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a1126-145">supportsScopeTags</span></span>|<span data-ttu-id="a1126-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1126-146">Boolean</span></span>|<span data-ttu-id="a1126-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a1126-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a1126-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a1126-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a1126-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="a1126-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a1126-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a1126-150">This property is read-only.</span></span> <span data-ttu-id="a1126-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1126-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1126-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1126-152">createdDateTime</span></span>|<span data-ttu-id="a1126-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1126-153">DateTimeOffset</span></span>|<span data-ttu-id="a1126-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a1126-154">DateTime the object was created.</span></span> <span data-ttu-id="a1126-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1126-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1126-156">description</span><span class="sxs-lookup"><span data-stu-id="a1126-156">description</span></span>|<span data-ttu-id="a1126-157">String</span><span class="sxs-lookup"><span data-stu-id="a1126-157">String</span></span>|<span data-ttu-id="a1126-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1126-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a1126-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1126-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1126-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a1126-160">displayName</span></span>|<span data-ttu-id="a1126-161">String</span><span class="sxs-lookup"><span data-stu-id="a1126-161">String</span></span>|<span data-ttu-id="a1126-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1126-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a1126-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1126-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1126-164">version</span><span class="sxs-lookup"><span data-stu-id="a1126-164">version</span></span>|<span data-ttu-id="a1126-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a1126-165">Int32</span></span>|<span data-ttu-id="a1126-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1126-166">Version of the device configuration.</span></span> <span data-ttu-id="a1126-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1126-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1126-168">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="a1126-168">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="a1126-169">String</span><span class="sxs-lookup"><span data-stu-id="a1126-169">String</span></span>|<span data-ttu-id="a1126-170">Windows Defender AdvancedThreatProtection inclusão Blob.</span><span class="sxs-lookup"><span data-stu-id="a1126-170">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="a1126-171">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="a1126-171">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="a1126-172">String</span><span class="sxs-lookup"><span data-stu-id="a1126-172">String</span></span>|<span data-ttu-id="a1126-173">Nome do arquivo do qual AdvancedThreatProtectionOnboardingBlob foi obtido.</span><span class="sxs-lookup"><span data-stu-id="a1126-173">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="a1126-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="a1126-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="a1126-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1126-175">Boolean</span></span>|<span data-ttu-id="a1126-176">Auto preencher blob de inclusão programaticamente a partir de serviço de proteção de ameaça avançadas</span><span class="sxs-lookup"><span data-stu-id="a1126-176">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="a1126-177">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="a1126-177">allowSampleSharing</span></span>|<span data-ttu-id="a1126-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1126-178">Boolean</span></span>|<span data-ttu-id="a1126-179">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="a1126-179">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="a1126-180">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="a1126-180">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="a1126-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1126-181">Boolean</span></span>|<span data-ttu-id="a1126-182">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="a1126-182">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="a1126-183">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="a1126-183">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="a1126-184">String</span><span class="sxs-lookup"><span data-stu-id="a1126-184">String</span></span>|<span data-ttu-id="a1126-185">Windows Defender AdvancedThreatProtection exclusão Blob.</span><span class="sxs-lookup"><span data-stu-id="a1126-185">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="a1126-186">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="a1126-186">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="a1126-187">String</span><span class="sxs-lookup"><span data-stu-id="a1126-187">String</span></span>|<span data-ttu-id="a1126-188">Nome do arquivo do qual AdvancedThreatProtectionOffboardingBlob foi obtido.</span><span class="sxs-lookup"><span data-stu-id="a1126-188">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="a1126-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1126-189">Response</span></span>
<span data-ttu-id="a1126-190">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1126-190">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1126-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1126-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1126-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1126-192">Request</span></span>
<span data-ttu-id="a1126-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1126-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 803

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="a1126-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1126-194">Response</span></span>
<span data-ttu-id="a1126-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1126-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





