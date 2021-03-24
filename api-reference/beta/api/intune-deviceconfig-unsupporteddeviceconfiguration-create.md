---
title: Criar unsupportedDeviceConfiguration
description: Crie um novo objeto unsupportedDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: afd0e39f46832323c5cf218a26521030554a872f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129626"
---
# <a name="create-unsupporteddeviceconfiguration"></a><span data-ttu-id="34749-103">Criar unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="34749-103">Create unsupportedDeviceConfiguration</span></span>

<span data-ttu-id="34749-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34749-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34749-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34749-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34749-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34749-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34749-107">Crie um novo [objeto unsupportedDeviceConfiguration.](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34749-107">Create a new [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34749-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34749-108">Prerequisites</span></span>
<span data-ttu-id="34749-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34749-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34749-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34749-111">Permission type</span></span>|<span data-ttu-id="34749-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34749-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34749-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34749-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34749-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34749-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34749-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34749-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34749-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34749-116">Not supported.</span></span>|
|<span data-ttu-id="34749-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34749-117">Application</span></span>|<span data-ttu-id="34749-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34749-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34749-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34749-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="34749-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34749-120">Request headers</span></span>
|<span data-ttu-id="34749-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34749-121">Header</span></span>|<span data-ttu-id="34749-122">Valor</span><span class="sxs-lookup"><span data-stu-id="34749-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34749-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="34749-123">Authorization</span></span>|<span data-ttu-id="34749-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34749-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34749-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="34749-125">Accept</span></span>|<span data-ttu-id="34749-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34749-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34749-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34749-127">Request body</span></span>
<span data-ttu-id="34749-128">No corpo da solicitação, fornece uma representação JSON para o objeto unsupportedDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="34749-128">In the request body, supply a JSON representation for the unsupportedDeviceConfiguration object.</span></span>

<span data-ttu-id="34749-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o unsupportedDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="34749-129">The following table shows the properties that are required when you create the unsupportedDeviceConfiguration.</span></span>

|<span data-ttu-id="34749-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34749-130">Property</span></span>|<span data-ttu-id="34749-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="34749-131">Type</span></span>|<span data-ttu-id="34749-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="34749-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34749-133">id</span><span class="sxs-lookup"><span data-stu-id="34749-133">id</span></span>|<span data-ttu-id="34749-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34749-134">String</span></span>|<span data-ttu-id="34749-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="34749-135">Key of the entity.</span></span> <span data-ttu-id="34749-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34749-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34749-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34749-137">lastModifiedDateTime</span></span>|<span data-ttu-id="34749-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34749-138">DateTimeOffset</span></span>|<span data-ttu-id="34749-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="34749-139">DateTime the object was last modified.</span></span> <span data-ttu-id="34749-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34749-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34749-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="34749-141">roleScopeTagIds</span></span>|<span data-ttu-id="34749-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="34749-142">String collection</span></span>|<span data-ttu-id="34749-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="34749-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="34749-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34749-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34749-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="34749-145">supportsScopeTags</span></span>|<span data-ttu-id="34749-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="34749-146">Boolean</span></span>|<span data-ttu-id="34749-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="34749-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="34749-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="34749-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="34749-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="34749-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="34749-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="34749-150">This property is read-only.</span></span> <span data-ttu-id="34749-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34749-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34749-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="34749-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="34749-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="34749-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="34749-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="34749-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="34749-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34749-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34749-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="34749-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="34749-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="34749-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="34749-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="34749-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="34749-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34749-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34749-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="34749-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="34749-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="34749-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="34749-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="34749-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="34749-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34749-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34749-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34749-164">createdDateTime</span></span>|<span data-ttu-id="34749-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34749-165">DateTimeOffset</span></span>|<span data-ttu-id="34749-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="34749-166">DateTime the object was created.</span></span> <span data-ttu-id="34749-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34749-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34749-168">descrição</span><span class="sxs-lookup"><span data-stu-id="34749-168">description</span></span>|<span data-ttu-id="34749-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34749-169">String</span></span>|<span data-ttu-id="34749-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34749-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="34749-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34749-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34749-172">displayName</span><span class="sxs-lookup"><span data-stu-id="34749-172">displayName</span></span>|<span data-ttu-id="34749-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34749-173">String</span></span>|<span data-ttu-id="34749-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34749-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="34749-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34749-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34749-176">versão</span><span class="sxs-lookup"><span data-stu-id="34749-176">version</span></span>|<span data-ttu-id="34749-177">Int32</span><span class="sxs-lookup"><span data-stu-id="34749-177">Int32</span></span>|<span data-ttu-id="34749-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34749-178">Version of the device configuration.</span></span> <span data-ttu-id="34749-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34749-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34749-180">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="34749-180">originalEntityTypeName</span></span>|<span data-ttu-id="34749-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34749-181">String</span></span>|<span data-ttu-id="34749-182">O tipo de entidade que seria retornada caso contrário.</span><span class="sxs-lookup"><span data-stu-id="34749-182">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="34749-183">detalhes</span><span class="sxs-lookup"><span data-stu-id="34749-183">details</span></span>|<span data-ttu-id="34749-184">[coleção unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)</span><span class="sxs-lookup"><span data-stu-id="34749-184">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="34749-185">Detalhes que descrevem por que a entidade não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="34749-185">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="34749-186">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="34749-186">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="34749-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="34749-187">Response</span></span>
<span data-ttu-id="34749-188">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34749-188">If successful, this method returns a `201 Created` response code and a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34749-189">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34749-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="34749-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34749-190">Request</span></span>
<span data-ttu-id="34749-191">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34749-191">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1291

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
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
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="34749-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="34749-192">Response</span></span>
<span data-ttu-id="34749-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34749-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1463

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
  "id": "f80d6fc8-6fc8-f80d-c86f-0df8c86f0df8",
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
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```




