---
title: Criar windowsHealthMonitoringConfiguration
description: Criar um novo objeto windowsHealthMonitoringConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fece8f0095067393da3d13b773291b89daa2325d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982169"
---
# <a name="create-windowshealthmonitoringconfiguration"></a><span data-ttu-id="a383a-103">Criar windowsHealthMonitoringConfiguration</span><span class="sxs-lookup"><span data-stu-id="a383a-103">Create windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="a383a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a383a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a383a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a383a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a383a-106">Criar um novo objeto [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a383a-106">Create a new [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a383a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a383a-107">Prerequisites</span></span>
<span data-ttu-id="a383a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a383a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a383a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a383a-110">Permission type</span></span>|<span data-ttu-id="a383a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a383a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a383a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a383a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a383a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a383a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a383a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a383a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a383a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a383a-115">Not supported.</span></span>|
|<span data-ttu-id="a383a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a383a-116">Application</span></span>|<span data-ttu-id="a383a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a383a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a383a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a383a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a383a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a383a-119">Request headers</span></span>
|<span data-ttu-id="a383a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a383a-120">Header</span></span>|<span data-ttu-id="a383a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a383a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a383a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a383a-122">Authorization</span></span>|<span data-ttu-id="a383a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a383a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a383a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a383a-124">Accept</span></span>|<span data-ttu-id="a383a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a383a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a383a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a383a-126">Request body</span></span>
<span data-ttu-id="a383a-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsHealthMonitoringConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a383a-127">In the request body, supply a JSON representation for the windowsHealthMonitoringConfiguration object.</span></span>

<span data-ttu-id="a383a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsHealthMonitoringConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a383a-128">The following table shows the properties that are required when you create the windowsHealthMonitoringConfiguration.</span></span>

|<span data-ttu-id="a383a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a383a-129">Property</span></span>|<span data-ttu-id="a383a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a383a-130">Type</span></span>|<span data-ttu-id="a383a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a383a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a383a-132">id</span><span class="sxs-lookup"><span data-stu-id="a383a-132">id</span></span>|<span data-ttu-id="a383a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a383a-133">String</span></span>|<span data-ttu-id="a383a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a383a-134">Key of the entity.</span></span> <span data-ttu-id="a383a-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a383a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a383a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a383a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a383a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a383a-137">DateTimeOffset</span></span>|<span data-ttu-id="a383a-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a383a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a383a-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a383a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a383a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a383a-140">roleScopeTagIds</span></span>|<span data-ttu-id="a383a-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a383a-141">String collection</span></span>|<span data-ttu-id="a383a-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a383a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a383a-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a383a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a383a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a383a-144">supportsScopeTags</span></span>|<span data-ttu-id="a383a-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="a383a-145">Boolean</span></span>|<span data-ttu-id="a383a-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a383a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a383a-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a383a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a383a-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a383a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a383a-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a383a-149">This property is read-only.</span></span> <span data-ttu-id="a383a-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a383a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a383a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a383a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a383a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a383a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a383a-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="a383a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a383a-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a383a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a383a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a383a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a383a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a383a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a383a-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="a383a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a383a-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a383a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a383a-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a383a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a383a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a383a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a383a-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="a383a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a383a-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a383a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a383a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a383a-163">createdDateTime</span></span>|<span data-ttu-id="a383a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a383a-164">DateTimeOffset</span></span>|<span data-ttu-id="a383a-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a383a-165">DateTime the object was created.</span></span> <span data-ttu-id="a383a-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a383a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a383a-167">descrição</span><span class="sxs-lookup"><span data-stu-id="a383a-167">description</span></span>|<span data-ttu-id="a383a-168">String</span><span class="sxs-lookup"><span data-stu-id="a383a-168">String</span></span>|<span data-ttu-id="a383a-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a383a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a383a-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a383a-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a383a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a383a-171">displayName</span></span>|<span data-ttu-id="a383a-172">String</span><span class="sxs-lookup"><span data-stu-id="a383a-172">String</span></span>|<span data-ttu-id="a383a-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a383a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a383a-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a383a-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a383a-175">versão</span><span class="sxs-lookup"><span data-stu-id="a383a-175">version</span></span>|<span data-ttu-id="a383a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a383a-176">Int32</span></span>|<span data-ttu-id="a383a-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a383a-177">Version of the device configuration.</span></span> <span data-ttu-id="a383a-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a383a-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a383a-179">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="a383a-179">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="a383a-180">habilitação</span><span class="sxs-lookup"><span data-stu-id="a383a-180">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a383a-181">Habilita o monitoramento de integridade do dispositivo no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a383a-181">Enables device health monitoring on the device.</span></span> <span data-ttu-id="a383a-182">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="a383a-182">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a383a-183">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="a383a-183">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="a383a-184">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="a383a-184">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="a383a-185">Especifica o conjunto de eventos coletados do dispositivo onde o monitoramento de integridade está habilitado.</span><span class="sxs-lookup"><span data-stu-id="a383a-185">Specifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="a383a-186">Os valores possíveis são: `undefined`, `healthMonitoring`, `bootPerformance`.</span><span class="sxs-lookup"><span data-stu-id="a383a-186">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`.</span></span>|
|<span data-ttu-id="a383a-187">configDeviceHealthMonitoringCustomScope</span><span class="sxs-lookup"><span data-stu-id="a383a-187">configDeviceHealthMonitoringCustomScope</span></span>|<span data-ttu-id="a383a-188">String</span><span class="sxs-lookup"><span data-stu-id="a383a-188">String</span></span>|<span data-ttu-id="a383a-189">Especifica um conjunto personalizado de eventos coletados do dispositivo onde o monitoramento de integridade está habilitado</span><span class="sxs-lookup"><span data-stu-id="a383a-189">Specifies custom set of events collected from the device where health monitoring is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="a383a-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="a383a-190">Response</span></span>
<span data-ttu-id="a383a-191">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a383a-191">If successful, this method returns a `201 Created` response code and a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a383a-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a383a-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="a383a-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a383a-193">Request</span></span>
<span data-ttu-id="a383a-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a383a-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1244

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
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
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring",
  "configDeviceHealthMonitoringCustomScope": "Config Device Health Monitoring Custom Scope value"
}
```

### <a name="response"></a><span data-ttu-id="a383a-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="a383a-195">Response</span></span>
<span data-ttu-id="a383a-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a383a-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1416

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
  "id": "3439bcec-bcec-3439-ecbc-3934ecbc3934",
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
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring",
  "configDeviceHealthMonitoringCustomScope": "Config Device Health Monitoring Custom Scope value"
}
```





