---
title: Criar iosDerivedCredentialAuthenticationConfiguration
description: Crie um novo objeto iosDerivedCredentialAuthenticationConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9b2b70ee48c6e3e862a0e3972b8e42491cafe5e2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151372"
---
# <a name="create-iosderivedcredentialauthenticationconfiguration"></a><span data-ttu-id="afa98-103">Criar iosDerivedCredentialAuthenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="afa98-103">Create iosDerivedCredentialAuthenticationConfiguration</span></span>

<span data-ttu-id="afa98-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afa98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afa98-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="afa98-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afa98-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="afa98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afa98-107">Crie um novo [objeto iosDerivedCredentialAuthenticationConfiguration.](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afa98-107">Create a new [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afa98-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="afa98-108">Prerequisites</span></span>
<span data-ttu-id="afa98-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afa98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afa98-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afa98-111">Permission type</span></span>|<span data-ttu-id="afa98-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="afa98-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afa98-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afa98-113">Delegated (work or school account)</span></span>|<span data-ttu-id="afa98-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afa98-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="afa98-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afa98-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afa98-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afa98-116">Not supported.</span></span>|
|<span data-ttu-id="afa98-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="afa98-117">Application</span></span>|<span data-ttu-id="afa98-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afa98-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="afa98-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afa98-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="afa98-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afa98-120">Request headers</span></span>
|<span data-ttu-id="afa98-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="afa98-121">Header</span></span>|<span data-ttu-id="afa98-122">Valor</span><span class="sxs-lookup"><span data-stu-id="afa98-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afa98-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="afa98-123">Authorization</span></span>|<span data-ttu-id="afa98-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afa98-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afa98-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="afa98-125">Accept</span></span>|<span data-ttu-id="afa98-126">application/json</span><span class="sxs-lookup"><span data-stu-id="afa98-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afa98-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afa98-127">Request body</span></span>
<span data-ttu-id="afa98-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosDerivedCredentialAuthenticationConfiguration.</span><span class="sxs-lookup"><span data-stu-id="afa98-128">In the request body, supply a JSON representation for the iosDerivedCredentialAuthenticationConfiguration object.</span></span>

<span data-ttu-id="afa98-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosDerivedCredentialAuthenticationConfiguration.</span><span class="sxs-lookup"><span data-stu-id="afa98-129">The following table shows the properties that are required when you create the iosDerivedCredentialAuthenticationConfiguration.</span></span>

|<span data-ttu-id="afa98-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="afa98-130">Property</span></span>|<span data-ttu-id="afa98-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="afa98-131">Type</span></span>|<span data-ttu-id="afa98-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="afa98-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afa98-133">id</span><span class="sxs-lookup"><span data-stu-id="afa98-133">id</span></span>|<span data-ttu-id="afa98-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afa98-134">String</span></span>|<span data-ttu-id="afa98-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="afa98-135">Key of the entity.</span></span> <span data-ttu-id="afa98-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afa98-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afa98-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="afa98-137">lastModifiedDateTime</span></span>|<span data-ttu-id="afa98-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afa98-138">DateTimeOffset</span></span>|<span data-ttu-id="afa98-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="afa98-139">DateTime the object was last modified.</span></span> <span data-ttu-id="afa98-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afa98-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afa98-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="afa98-141">roleScopeTagIds</span></span>|<span data-ttu-id="afa98-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="afa98-142">String collection</span></span>|<span data-ttu-id="afa98-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="afa98-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="afa98-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afa98-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afa98-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="afa98-145">supportsScopeTags</span></span>|<span data-ttu-id="afa98-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="afa98-146">Boolean</span></span>|<span data-ttu-id="afa98-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="afa98-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="afa98-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="afa98-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="afa98-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="afa98-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="afa98-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="afa98-150">This property is read-only.</span></span> <span data-ttu-id="afa98-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afa98-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afa98-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="afa98-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="afa98-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="afa98-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="afa98-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="afa98-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="afa98-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afa98-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afa98-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="afa98-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="afa98-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="afa98-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="afa98-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="afa98-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="afa98-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afa98-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afa98-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="afa98-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="afa98-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="afa98-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="afa98-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="afa98-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="afa98-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afa98-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afa98-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="afa98-164">createdDateTime</span></span>|<span data-ttu-id="afa98-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afa98-165">DateTimeOffset</span></span>|<span data-ttu-id="afa98-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="afa98-166">DateTime the object was created.</span></span> <span data-ttu-id="afa98-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afa98-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afa98-168">descrição</span><span class="sxs-lookup"><span data-stu-id="afa98-168">description</span></span>|<span data-ttu-id="afa98-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afa98-169">String</span></span>|<span data-ttu-id="afa98-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="afa98-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="afa98-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afa98-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afa98-172">displayName</span><span class="sxs-lookup"><span data-stu-id="afa98-172">displayName</span></span>|<span data-ttu-id="afa98-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afa98-173">String</span></span>|<span data-ttu-id="afa98-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="afa98-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="afa98-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afa98-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afa98-176">versão</span><span class="sxs-lookup"><span data-stu-id="afa98-176">version</span></span>|<span data-ttu-id="afa98-177">Int32</span><span class="sxs-lookup"><span data-stu-id="afa98-177">Int32</span></span>|<span data-ttu-id="afa98-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="afa98-178">Version of the device configuration.</span></span> <span data-ttu-id="afa98-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afa98-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="afa98-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="afa98-180">Response</span></span>
<span data-ttu-id="afa98-181">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="afa98-181">If successful, this method returns a `201 Created` response code and a [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afa98-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="afa98-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="afa98-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="afa98-183">Request</span></span>
<span data-ttu-id="afa98-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="afa98-184">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1050

{
  "@odata.type": "#microsoft.graph.iosDerivedCredentialAuthenticationConfiguration",
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
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="afa98-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="afa98-185">Response</span></span>
<span data-ttu-id="afa98-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="afa98-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1222

{
  "@odata.type": "#microsoft.graph.iosDerivedCredentialAuthenticationConfiguration",
  "id": "01713f58-3f58-0171-583f-7101583f7101",
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
  "version": 7
}
```




