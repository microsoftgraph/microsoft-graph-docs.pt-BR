---
title: Atualizar unsupportedDeviceConfiguration
description: Atualiza as propriedades de um objeto unsupportedDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 744afcf32a8850bc6cbf1a759800c2f0068ec1d1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947712"
---
# <a name="update-unsupporteddeviceconfiguration"></a><span data-ttu-id="44429-103">Atualizar unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="44429-103">Update unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="44429-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="44429-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44429-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44429-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44429-106">Atualiza as propriedades de um objeto [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="44429-106">Update the properties of a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44429-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="44429-107">Prerequisites</span></span>
<span data-ttu-id="44429-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44429-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44429-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44429-110">Permission type</span></span>|<span data-ttu-id="44429-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="44429-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44429-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44429-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44429-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44429-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44429-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44429-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44429-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44429-115">Not supported.</span></span>|
|<span data-ttu-id="44429-116">Application</span><span class="sxs-lookup"><span data-stu-id="44429-116">Application</span></span>|<span data-ttu-id="44429-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44429-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44429-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44429-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="44429-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44429-119">Request headers</span></span>
|<span data-ttu-id="44429-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="44429-120">Header</span></span>|<span data-ttu-id="44429-121">Valor</span><span class="sxs-lookup"><span data-stu-id="44429-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44429-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="44429-122">Authorization</span></span>|<span data-ttu-id="44429-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44429-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44429-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="44429-124">Accept</span></span>|<span data-ttu-id="44429-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44429-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44429-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44429-126">Request body</span></span>
<span data-ttu-id="44429-127">No corpo da solicitação, forneça uma representação JSON do objeto [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="44429-127">In the request body, supply a JSON representation for the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

<span data-ttu-id="44429-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="44429-128">The following table shows the properties that are required when you create the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span></span>

|<span data-ttu-id="44429-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44429-129">Property</span></span>|<span data-ttu-id="44429-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="44429-130">Type</span></span>|<span data-ttu-id="44429-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="44429-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44429-132">id</span><span class="sxs-lookup"><span data-stu-id="44429-132">id</span></span>|<span data-ttu-id="44429-133">String</span><span class="sxs-lookup"><span data-stu-id="44429-133">String</span></span>|<span data-ttu-id="44429-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="44429-134">Key of the entity.</span></span> <span data-ttu-id="44429-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44429-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44429-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44429-136">lastModifiedDateTime</span></span>|<span data-ttu-id="44429-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44429-137">DateTimeOffset</span></span>|<span data-ttu-id="44429-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="44429-138">DateTime the object was last modified.</span></span> <span data-ttu-id="44429-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44429-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44429-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="44429-140">roleScopeTagIds</span></span>|<span data-ttu-id="44429-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="44429-141">String collection</span></span>|<span data-ttu-id="44429-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="44429-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="44429-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44429-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44429-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="44429-144">supportsScopeTags</span></span>|<span data-ttu-id="44429-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="44429-145">Boolean</span></span>|<span data-ttu-id="44429-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="44429-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="44429-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="44429-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="44429-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="44429-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="44429-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44429-149">This property is read-only.</span></span> <span data-ttu-id="44429-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44429-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44429-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="44429-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="44429-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="44429-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="44429-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="44429-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="44429-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44429-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44429-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="44429-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="44429-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="44429-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="44429-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="44429-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="44429-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44429-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44429-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="44429-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="44429-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="44429-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="44429-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="44429-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="44429-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44429-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44429-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44429-163">createdDateTime</span></span>|<span data-ttu-id="44429-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44429-164">DateTimeOffset</span></span>|<span data-ttu-id="44429-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="44429-165">DateTime the object was created.</span></span> <span data-ttu-id="44429-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44429-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44429-167">description</span><span class="sxs-lookup"><span data-stu-id="44429-167">description</span></span>|<span data-ttu-id="44429-168">String</span><span class="sxs-lookup"><span data-stu-id="44429-168">String</span></span>|<span data-ttu-id="44429-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44429-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="44429-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44429-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44429-171">displayName</span><span class="sxs-lookup"><span data-stu-id="44429-171">displayName</span></span>|<span data-ttu-id="44429-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44429-172">String</span></span>|<span data-ttu-id="44429-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44429-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="44429-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44429-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44429-175">versão</span><span class="sxs-lookup"><span data-stu-id="44429-175">version</span></span>|<span data-ttu-id="44429-176">Int32</span><span class="sxs-lookup"><span data-stu-id="44429-176">Int32</span></span>|<span data-ttu-id="44429-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44429-177">Version of the device configuration.</span></span> <span data-ttu-id="44429-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44429-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44429-179">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="44429-179">originalEntityTypeName</span></span>|<span data-ttu-id="44429-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="44429-180">String</span></span>|<span data-ttu-id="44429-181">O tipo de entidade que seria retornado de outra forma.</span><span class="sxs-lookup"><span data-stu-id="44429-181">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="44429-182">detalhes</span><span class="sxs-lookup"><span data-stu-id="44429-182">details</span></span>|<span data-ttu-id="44429-183">coleção [unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)</span><span class="sxs-lookup"><span data-stu-id="44429-183">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="44429-184">Detalhes que descrevem por que a entidade não é suportada.</span><span class="sxs-lookup"><span data-stu-id="44429-184">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="44429-185">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="44429-185">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="44429-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="44429-186">Response</span></span>
<span data-ttu-id="44429-187">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44429-187">If successful, this method returns a `200 OK` response code and an updated [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44429-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44429-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="44429-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44429-189">Request</span></span>
<span data-ttu-id="44429-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44429-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="44429-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="44429-191">Response</span></span>
<span data-ttu-id="44429-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44429-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





