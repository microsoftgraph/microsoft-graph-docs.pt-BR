---
title: Atualizar windowsPhone81CustomConfiguration
description: Atualizar as propriedades de um objeto windowsPhone81CustomConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 771e7472087ad384761833b1d13a4137660f283b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36344172"
---
# <a name="update-windowsphone81customconfiguration"></a><span data-ttu-id="62f99-103">Atualizar windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="62f99-103">Update windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="62f99-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62f99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62f99-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62f99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62f99-106">Atualizar as propriedades de um objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62f99-106">Update the properties of a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62f99-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62f99-107">Prerequisites</span></span>
<span data-ttu-id="62f99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62f99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62f99-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62f99-110">Permission type</span></span>|<span data-ttu-id="62f99-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62f99-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62f99-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62f99-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62f99-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62f99-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="62f99-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62f99-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62f99-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62f99-115">Not supported.</span></span>|
|<span data-ttu-id="62f99-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62f99-116">Application</span></span>|<span data-ttu-id="62f99-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62f99-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62f99-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62f99-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="62f99-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62f99-119">Request headers</span></span>
|<span data-ttu-id="62f99-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62f99-120">Header</span></span>|<span data-ttu-id="62f99-121">Valor</span><span class="sxs-lookup"><span data-stu-id="62f99-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62f99-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="62f99-122">Authorization</span></span>|<span data-ttu-id="62f99-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62f99-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62f99-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62f99-124">Accept</span></span>|<span data-ttu-id="62f99-125">application/json</span><span class="sxs-lookup"><span data-stu-id="62f99-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62f99-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62f99-126">Request body</span></span>
<span data-ttu-id="62f99-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62f99-127">In the request body, supply a JSON representation for the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

<span data-ttu-id="62f99-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62f99-128">The following table shows the properties that are required when you create the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

|<span data-ttu-id="62f99-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62f99-129">Property</span></span>|<span data-ttu-id="62f99-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="62f99-130">Type</span></span>|<span data-ttu-id="62f99-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="62f99-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62f99-132">id</span><span class="sxs-lookup"><span data-stu-id="62f99-132">id</span></span>|<span data-ttu-id="62f99-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62f99-133">String</span></span>|<span data-ttu-id="62f99-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="62f99-134">Key of the entity.</span></span> <span data-ttu-id="62f99-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62f99-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62f99-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62f99-136">lastModifiedDateTime</span></span>|<span data-ttu-id="62f99-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62f99-137">DateTimeOffset</span></span>|<span data-ttu-id="62f99-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="62f99-138">DateTime the object was last modified.</span></span> <span data-ttu-id="62f99-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62f99-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62f99-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="62f99-140">roleScopeTagIds</span></span>|<span data-ttu-id="62f99-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="62f99-141">String collection</span></span>|<span data-ttu-id="62f99-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="62f99-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="62f99-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62f99-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62f99-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="62f99-144">supportsScopeTags</span></span>|<span data-ttu-id="62f99-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="62f99-145">Boolean</span></span>|<span data-ttu-id="62f99-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="62f99-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="62f99-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="62f99-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="62f99-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="62f99-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="62f99-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="62f99-149">This property is read-only.</span></span> <span data-ttu-id="62f99-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62f99-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62f99-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="62f99-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="62f99-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="62f99-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="62f99-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="62f99-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="62f99-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62f99-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62f99-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="62f99-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="62f99-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="62f99-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="62f99-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="62f99-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="62f99-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62f99-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62f99-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="62f99-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="62f99-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="62f99-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="62f99-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="62f99-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="62f99-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62f99-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62f99-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62f99-163">createdDateTime</span></span>|<span data-ttu-id="62f99-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62f99-164">DateTimeOffset</span></span>|<span data-ttu-id="62f99-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="62f99-165">DateTime the object was created.</span></span> <span data-ttu-id="62f99-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62f99-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62f99-167">descrição</span><span class="sxs-lookup"><span data-stu-id="62f99-167">description</span></span>|<span data-ttu-id="62f99-168">String</span><span class="sxs-lookup"><span data-stu-id="62f99-168">String</span></span>|<span data-ttu-id="62f99-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="62f99-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="62f99-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62f99-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62f99-171">displayName</span><span class="sxs-lookup"><span data-stu-id="62f99-171">displayName</span></span>|<span data-ttu-id="62f99-172">String</span><span class="sxs-lookup"><span data-stu-id="62f99-172">String</span></span>|<span data-ttu-id="62f99-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="62f99-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="62f99-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62f99-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62f99-175">versão</span><span class="sxs-lookup"><span data-stu-id="62f99-175">version</span></span>|<span data-ttu-id="62f99-176">Int32</span><span class="sxs-lookup"><span data-stu-id="62f99-176">Int32</span></span>|<span data-ttu-id="62f99-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="62f99-177">Version of the device configuration.</span></span> <span data-ttu-id="62f99-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="62f99-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="62f99-179">omaSettings</span><span class="sxs-lookup"><span data-stu-id="62f99-179">omaSettings</span></span>|<span data-ttu-id="62f99-180">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="62f99-180">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="62f99-181">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="62f99-181">OMA settings.</span></span> <span data-ttu-id="62f99-182">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="62f99-182">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="62f99-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="62f99-183">Response</span></span>
<span data-ttu-id="62f99-184">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62f99-184">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62f99-185">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62f99-185">Example</span></span>

### <a name="request"></a><span data-ttu-id="62f99-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62f99-186">Request</span></span>
<span data-ttu-id="62f99-187">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62f99-187">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1301

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5,
      "isReadOnly": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="62f99-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="62f99-188">Response</span></span>
<span data-ttu-id="62f99-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62f99-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1473

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5,
      "isReadOnly": true
    }
  ]
}
```






