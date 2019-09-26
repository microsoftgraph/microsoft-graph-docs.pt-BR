---
title: Criar unsupportedDeviceConfiguration
description: Criar um novo objeto unsupportedDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3bd4eb004bdb25a62a7d26033b142a8c29515194
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37183216"
---
# <a name="create-unsupporteddeviceconfiguration"></a><span data-ttu-id="23b01-103">Criar unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="23b01-103">Create unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="23b01-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="23b01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23b01-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23b01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23b01-106">Criar um novo objeto [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="23b01-106">Create a new [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23b01-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="23b01-107">Prerequisites</span></span>
<span data-ttu-id="23b01-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23b01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23b01-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23b01-110">Permission type</span></span>|<span data-ttu-id="23b01-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="23b01-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23b01-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23b01-112">Delegated (work or school account)</span></span>|<span data-ttu-id="23b01-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23b01-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23b01-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23b01-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23b01-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23b01-115">Not supported.</span></span>|
|<span data-ttu-id="23b01-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23b01-116">Application</span></span>|<span data-ttu-id="23b01-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23b01-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23b01-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23b01-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="23b01-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23b01-119">Request headers</span></span>
|<span data-ttu-id="23b01-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23b01-120">Header</span></span>|<span data-ttu-id="23b01-121">Valor</span><span class="sxs-lookup"><span data-stu-id="23b01-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23b01-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="23b01-122">Authorization</span></span>|<span data-ttu-id="23b01-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23b01-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23b01-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="23b01-124">Accept</span></span>|<span data-ttu-id="23b01-125">application/json</span><span class="sxs-lookup"><span data-stu-id="23b01-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23b01-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23b01-126">Request body</span></span>
<span data-ttu-id="23b01-127">No corpo da solicitação, forneça uma representação JSON do objeto unsupportedDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="23b01-127">In the request body, supply a JSON representation for the unsupportedDeviceConfiguration object.</span></span>

<span data-ttu-id="23b01-128">A tabela a seguir mostra as propriedades que são necessárias ao criar unsupportedDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="23b01-128">The following table shows the properties that are required when you create the unsupportedDeviceConfiguration.</span></span>

|<span data-ttu-id="23b01-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23b01-129">Property</span></span>|<span data-ttu-id="23b01-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="23b01-130">Type</span></span>|<span data-ttu-id="23b01-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="23b01-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23b01-132">id</span><span class="sxs-lookup"><span data-stu-id="23b01-132">id</span></span>|<span data-ttu-id="23b01-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23b01-133">String</span></span>|<span data-ttu-id="23b01-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="23b01-134">Key of the entity.</span></span> <span data-ttu-id="23b01-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23b01-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23b01-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23b01-136">lastModifiedDateTime</span></span>|<span data-ttu-id="23b01-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23b01-137">DateTimeOffset</span></span>|<span data-ttu-id="23b01-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="23b01-138">DateTime the object was last modified.</span></span> <span data-ttu-id="23b01-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23b01-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23b01-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="23b01-140">roleScopeTagIds</span></span>|<span data-ttu-id="23b01-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="23b01-141">String collection</span></span>|<span data-ttu-id="23b01-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="23b01-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="23b01-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23b01-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23b01-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="23b01-144">supportsScopeTags</span></span>|<span data-ttu-id="23b01-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="23b01-145">Boolean</span></span>|<span data-ttu-id="23b01-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="23b01-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="23b01-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="23b01-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="23b01-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="23b01-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="23b01-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23b01-149">This property is read-only.</span></span> <span data-ttu-id="23b01-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23b01-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23b01-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="23b01-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="23b01-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="23b01-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="23b01-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="23b01-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="23b01-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23b01-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23b01-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="23b01-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="23b01-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="23b01-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="23b01-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="23b01-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="23b01-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23b01-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23b01-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="23b01-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="23b01-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="23b01-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="23b01-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="23b01-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="23b01-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23b01-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23b01-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23b01-163">createdDateTime</span></span>|<span data-ttu-id="23b01-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23b01-164">DateTimeOffset</span></span>|<span data-ttu-id="23b01-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="23b01-165">DateTime the object was created.</span></span> <span data-ttu-id="23b01-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23b01-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23b01-167">descrição</span><span class="sxs-lookup"><span data-stu-id="23b01-167">description</span></span>|<span data-ttu-id="23b01-168">String</span><span class="sxs-lookup"><span data-stu-id="23b01-168">String</span></span>|<span data-ttu-id="23b01-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23b01-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="23b01-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23b01-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23b01-171">displayName</span><span class="sxs-lookup"><span data-stu-id="23b01-171">displayName</span></span>|<span data-ttu-id="23b01-172">String</span><span class="sxs-lookup"><span data-stu-id="23b01-172">String</span></span>|<span data-ttu-id="23b01-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23b01-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="23b01-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23b01-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23b01-175">versão</span><span class="sxs-lookup"><span data-stu-id="23b01-175">version</span></span>|<span data-ttu-id="23b01-176">Int32</span><span class="sxs-lookup"><span data-stu-id="23b01-176">Int32</span></span>|<span data-ttu-id="23b01-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23b01-177">Version of the device configuration.</span></span> <span data-ttu-id="23b01-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23b01-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23b01-179">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="23b01-179">originalEntityTypeName</span></span>|<span data-ttu-id="23b01-180">String</span><span class="sxs-lookup"><span data-stu-id="23b01-180">String</span></span>|<span data-ttu-id="23b01-181">O tipo de entidade que seria retornado de outra forma.</span><span class="sxs-lookup"><span data-stu-id="23b01-181">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="23b01-182">detalhes</span><span class="sxs-lookup"><span data-stu-id="23b01-182">details</span></span>|<span data-ttu-id="23b01-183">coleção [unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)</span><span class="sxs-lookup"><span data-stu-id="23b01-183">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="23b01-184">Detalhes que descrevem por que a entidade não é suportada.</span><span class="sxs-lookup"><span data-stu-id="23b01-184">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="23b01-185">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="23b01-185">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="23b01-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="23b01-186">Response</span></span>
<span data-ttu-id="23b01-187">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23b01-187">If successful, this method returns a `201 Created` response code and a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23b01-188">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23b01-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="23b01-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23b01-189">Request</span></span>
<span data-ttu-id="23b01-190">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23b01-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="23b01-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="23b01-191">Response</span></span>
<span data-ttu-id="23b01-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23b01-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




