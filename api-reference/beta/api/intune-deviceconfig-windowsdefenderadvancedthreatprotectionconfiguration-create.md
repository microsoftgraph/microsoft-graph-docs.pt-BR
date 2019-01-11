---
title: Criar windowsDefenderAdvancedThreatProtectionConfiguration
description: Criar um novo objeto windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 704365da447e3e6ccf702479ddceb06a3c14c4cd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836236"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="cc0c7-103">Criar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="cc0c7-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="cc0c7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc0c7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc0c7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc0c7-107">Criar um novo objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cc0c7-107">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cc0c7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cc0c7-108">Prerequisites</span></span>
<span data-ttu-id="cc0c7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc0c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc0c7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc0c7-111">Permission type</span></span>|<span data-ttu-id="cc0c7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cc0c7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc0c7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc0c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cc0c7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc0c7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc0c7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc0c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc0c7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-116">Not supported.</span></span>|
|<span data-ttu-id="cc0c7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc0c7-117">Application</span></span>|<span data-ttu-id="cc0c7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc0c7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc0c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cc0c7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc0c7-120">Request headers</span></span>
|<span data-ttu-id="cc0c7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc0c7-121">Header</span></span>|<span data-ttu-id="cc0c7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cc0c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc0c7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc0c7-123">Authorization</span></span>|<span data-ttu-id="cc0c7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc0c7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cc0c7-125">Accept</span></span>|<span data-ttu-id="cc0c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cc0c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc0c7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc0c7-127">Request body</span></span>
<span data-ttu-id="cc0c7-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-128">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="cc0c7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-129">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="cc0c7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc0c7-130">Property</span></span>|<span data-ttu-id="cc0c7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc0c7-131">Type</span></span>|<span data-ttu-id="cc0c7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc0c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc0c7-133">id</span><span class="sxs-lookup"><span data-stu-id="cc0c7-133">id</span></span>|<span data-ttu-id="cc0c7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc0c7-134">String</span></span>|<span data-ttu-id="cc0c7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-135">Key of the entity.</span></span> <span data-ttu-id="cc0c7-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc0c7-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc0c7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc0c7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="cc0c7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc0c7-138">DateTimeOffset</span></span>|<span data-ttu-id="cc0c7-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="cc0c7-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc0c7-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc0c7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cc0c7-141">roleScopeTagIds</span></span>|<span data-ttu-id="cc0c7-142">String collection</span><span class="sxs-lookup"><span data-stu-id="cc0c7-142">String collection</span></span>|<span data-ttu-id="cc0c7-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cc0c7-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc0c7-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc0c7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="cc0c7-145">supportsScopeTags</span></span>|<span data-ttu-id="cc0c7-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="cc0c7-146">Boolean</span></span>|<span data-ttu-id="cc0c7-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cc0c7-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cc0c7-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cc0c7-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-150">This property is read-only.</span></span> <span data-ttu-id="cc0c7-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc0c7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc0c7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc0c7-152">createdDateTime</span></span>|<span data-ttu-id="cc0c7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc0c7-153">DateTimeOffset</span></span>|<span data-ttu-id="cc0c7-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-154">DateTime the object was created.</span></span> <span data-ttu-id="cc0c7-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc0c7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc0c7-156">description</span><span class="sxs-lookup"><span data-stu-id="cc0c7-156">description</span></span>|<span data-ttu-id="cc0c7-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc0c7-157">String</span></span>|<span data-ttu-id="cc0c7-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cc0c7-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc0c7-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc0c7-160">displayName</span><span class="sxs-lookup"><span data-stu-id="cc0c7-160">displayName</span></span>|<span data-ttu-id="cc0c7-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc0c7-161">String</span></span>|<span data-ttu-id="cc0c7-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cc0c7-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc0c7-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc0c7-164">version</span><span class="sxs-lookup"><span data-stu-id="cc0c7-164">version</span></span>|<span data-ttu-id="cc0c7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="cc0c7-165">Int32</span></span>|<span data-ttu-id="cc0c7-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-166">Version of the device configuration.</span></span> <span data-ttu-id="cc0c7-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc0c7-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc0c7-168">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="cc0c7-168">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="cc0c7-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc0c7-169">String</span></span>|<span data-ttu-id="cc0c7-170">Windows Defender AdvancedThreatProtection inclusão Blob.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-170">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="cc0c7-171">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="cc0c7-171">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="cc0c7-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc0c7-172">String</span></span>|<span data-ttu-id="cc0c7-173">Nome do arquivo do qual AdvancedThreatProtectionOnboardingBlob foi obtido.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-173">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="cc0c7-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="cc0c7-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="cc0c7-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="cc0c7-175">Boolean</span></span>|<span data-ttu-id="cc0c7-176">Auto preencher blob de inclusão programaticamente a partir de serviço de proteção de ameaça avançadas</span><span class="sxs-lookup"><span data-stu-id="cc0c7-176">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="cc0c7-177">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="cc0c7-177">allowSampleSharing</span></span>|<span data-ttu-id="cc0c7-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="cc0c7-178">Boolean</span></span>|<span data-ttu-id="cc0c7-179">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="cc0c7-179">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="cc0c7-180">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="cc0c7-180">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="cc0c7-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="cc0c7-181">Boolean</span></span>|<span data-ttu-id="cc0c7-182">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-182">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="cc0c7-183">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="cc0c7-183">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="cc0c7-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc0c7-184">String</span></span>|<span data-ttu-id="cc0c7-185">Windows Defender AdvancedThreatProtection exclusão Blob.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-185">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="cc0c7-186">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="cc0c7-186">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="cc0c7-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc0c7-187">String</span></span>|<span data-ttu-id="cc0c7-188">Nome do arquivo do qual AdvancedThreatProtectionOffboardingBlob foi obtido.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-188">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="cc0c7-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc0c7-189">Response</span></span>
<span data-ttu-id="cc0c7-190">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-190">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc0c7-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc0c7-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="cc0c7-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc0c7-192">Request</span></span>
<span data-ttu-id="cc0c7-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 894

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
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

### <a name="response"></a><span data-ttu-id="cc0c7-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc0c7-194">Response</span></span>
<span data-ttu-id="cc0c7-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc0c7-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





