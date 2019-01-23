---
title: Criar windowsDefenderAdvancedThreatProtectionConfiguration
description: Criar um novo objeto windowsDefenderAdvancedThreatProtectionConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1f6147a054d2addd5159c46f66d0d2133ce9e7bb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400498"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="54707-103">Criar windowsDefenderAdvancedThreatProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="54707-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="54707-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="54707-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="54707-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="54707-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54707-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="54707-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54707-107">Criar um novo objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54707-107">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54707-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54707-108">Prerequisites</span></span>
<span data-ttu-id="54707-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="54707-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="54707-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54707-111">Permission type</span></span>|<span data-ttu-id="54707-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="54707-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54707-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54707-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54707-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54707-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="54707-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54707-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54707-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54707-116">Not supported.</span></span>|
|<span data-ttu-id="54707-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54707-117">Application</span></span>|<span data-ttu-id="54707-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54707-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54707-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54707-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="54707-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54707-120">Request headers</span></span>
|<span data-ttu-id="54707-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54707-121">Header</span></span>|<span data-ttu-id="54707-122">Valor</span><span class="sxs-lookup"><span data-stu-id="54707-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54707-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="54707-123">Authorization</span></span>|<span data-ttu-id="54707-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54707-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54707-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="54707-125">Accept</span></span>|<span data-ttu-id="54707-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54707-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54707-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54707-127">Request body</span></span>
<span data-ttu-id="54707-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="54707-128">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="54707-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsDefenderAdvancedThreatProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="54707-129">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="54707-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54707-130">Property</span></span>|<span data-ttu-id="54707-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="54707-131">Type</span></span>|<span data-ttu-id="54707-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="54707-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54707-133">id</span><span class="sxs-lookup"><span data-stu-id="54707-133">id</span></span>|<span data-ttu-id="54707-134">String</span><span class="sxs-lookup"><span data-stu-id="54707-134">String</span></span>|<span data-ttu-id="54707-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="54707-135">Key of the entity.</span></span> <span data-ttu-id="54707-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54707-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54707-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54707-137">lastModifiedDateTime</span></span>|<span data-ttu-id="54707-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54707-138">DateTimeOffset</span></span>|<span data-ttu-id="54707-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="54707-139">DateTime the object was last modified.</span></span> <span data-ttu-id="54707-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54707-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54707-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="54707-141">roleScopeTagIds</span></span>|<span data-ttu-id="54707-142">String collection</span><span class="sxs-lookup"><span data-stu-id="54707-142">String collection</span></span>|<span data-ttu-id="54707-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="54707-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="54707-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54707-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54707-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="54707-145">supportsScopeTags</span></span>|<span data-ttu-id="54707-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="54707-146">Boolean</span></span>|<span data-ttu-id="54707-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="54707-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="54707-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="54707-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="54707-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="54707-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="54707-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54707-150">This property is read-only.</span></span> <span data-ttu-id="54707-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54707-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54707-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54707-152">createdDateTime</span></span>|<span data-ttu-id="54707-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54707-153">DateTimeOffset</span></span>|<span data-ttu-id="54707-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="54707-154">DateTime the object was created.</span></span> <span data-ttu-id="54707-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54707-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54707-156">description</span><span class="sxs-lookup"><span data-stu-id="54707-156">description</span></span>|<span data-ttu-id="54707-157">String</span><span class="sxs-lookup"><span data-stu-id="54707-157">String</span></span>|<span data-ttu-id="54707-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54707-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="54707-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54707-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54707-160">displayName</span><span class="sxs-lookup"><span data-stu-id="54707-160">displayName</span></span>|<span data-ttu-id="54707-161">String</span><span class="sxs-lookup"><span data-stu-id="54707-161">String</span></span>|<span data-ttu-id="54707-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54707-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="54707-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54707-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54707-164">version</span><span class="sxs-lookup"><span data-stu-id="54707-164">version</span></span>|<span data-ttu-id="54707-165">Int32</span><span class="sxs-lookup"><span data-stu-id="54707-165">Int32</span></span>|<span data-ttu-id="54707-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54707-166">Version of the device configuration.</span></span> <span data-ttu-id="54707-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54707-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54707-168">advancedThreatProtectionOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="54707-168">advancedThreatProtectionOnboardingBlob</span></span>|<span data-ttu-id="54707-169">String</span><span class="sxs-lookup"><span data-stu-id="54707-169">String</span></span>|<span data-ttu-id="54707-170">Windows Defender AdvancedThreatProtection inclusão Blob.</span><span class="sxs-lookup"><span data-stu-id="54707-170">Windows Defender AdvancedThreatProtection Onboarding Blob.</span></span>|
|<span data-ttu-id="54707-171">advancedThreatProtectionOnboardingFilename</span><span class="sxs-lookup"><span data-stu-id="54707-171">advancedThreatProtectionOnboardingFilename</span></span>|<span data-ttu-id="54707-172">String</span><span class="sxs-lookup"><span data-stu-id="54707-172">String</span></span>|<span data-ttu-id="54707-173">Nome do arquivo do qual AdvancedThreatProtectionOnboardingBlob foi obtido.</span><span class="sxs-lookup"><span data-stu-id="54707-173">Name of the file from which AdvancedThreatProtectionOnboardingBlob was obtained.</span></span>|
|<span data-ttu-id="54707-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span><span class="sxs-lookup"><span data-stu-id="54707-174">advancedThreatProtectionAutoPopulateOnboardingBlob</span></span>|<span data-ttu-id="54707-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="54707-175">Boolean</span></span>|<span data-ttu-id="54707-176">Auto preencher blob de inclusão programaticamente a partir de serviço de proteção de ameaça avançadas</span><span class="sxs-lookup"><span data-stu-id="54707-176">Auto populate onboarding blob programmatically from Advanced Threat protection service</span></span>|
|<span data-ttu-id="54707-177">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="54707-177">allowSampleSharing</span></span>|<span data-ttu-id="54707-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="54707-178">Boolean</span></span>|<span data-ttu-id="54707-179">Regra para "Permitir o compartilhamento de exemplo" de AdvancedThreatProtection do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="54707-179">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="54707-180">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="54707-180">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="54707-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="54707-181">Boolean</span></span>|<span data-ttu-id="54707-182">Acelera a frequência de relatórios de telemetria da Proteção Avançada Contra Ameaças do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="54707-182">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|
|<span data-ttu-id="54707-183">advancedThreatProtectionOffboardingBlob</span><span class="sxs-lookup"><span data-stu-id="54707-183">advancedThreatProtectionOffboardingBlob</span></span>|<span data-ttu-id="54707-184">String</span><span class="sxs-lookup"><span data-stu-id="54707-184">String</span></span>|<span data-ttu-id="54707-185">Windows Defender AdvancedThreatProtection exclusão Blob.</span><span class="sxs-lookup"><span data-stu-id="54707-185">Windows Defender AdvancedThreatProtection Offboarding Blob.</span></span>|
|<span data-ttu-id="54707-186">advancedThreatProtectionOffboardingFilename</span><span class="sxs-lookup"><span data-stu-id="54707-186">advancedThreatProtectionOffboardingFilename</span></span>|<span data-ttu-id="54707-187">String</span><span class="sxs-lookup"><span data-stu-id="54707-187">String</span></span>|<span data-ttu-id="54707-188">Nome do arquivo do qual AdvancedThreatProtectionOffboardingBlob foi obtido.</span><span class="sxs-lookup"><span data-stu-id="54707-188">Name of the file from which AdvancedThreatProtectionOffboardingBlob was obtained.</span></span>|



## <a name="response"></a><span data-ttu-id="54707-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="54707-189">Response</span></span>
<span data-ttu-id="54707-190">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54707-190">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54707-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54707-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="54707-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54707-192">Request</span></span>
<span data-ttu-id="54707-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54707-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="54707-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="54707-194">Response</span></span>
<span data-ttu-id="54707-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54707-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




