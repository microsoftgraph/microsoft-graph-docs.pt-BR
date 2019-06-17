---
title: Criar windowsHealthMonitoringConfiguration
description: Criar um novo objeto windowsHealthMonitoringConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 63146c8bf18452a7d41b2beb3b1de83db9d526c0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961977"
---
# <a name="create-windowshealthmonitoringconfiguration"></a><span data-ttu-id="b6966-103">Criar windowsHealthMonitoringConfiguration</span><span class="sxs-lookup"><span data-stu-id="b6966-103">Create windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="b6966-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6966-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6966-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6966-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6966-106">Criar um novo objeto [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b6966-106">Create a new [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6966-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6966-107">Prerequisites</span></span>
<span data-ttu-id="b6966-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6966-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6966-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6966-110">Permission type</span></span>|<span data-ttu-id="b6966-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6966-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6966-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6966-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6966-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6966-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6966-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6966-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6966-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6966-115">Not supported.</span></span>|
|<span data-ttu-id="b6966-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6966-116">Application</span></span>|<span data-ttu-id="b6966-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6966-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6966-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6966-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b6966-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6966-119">Request headers</span></span>
|<span data-ttu-id="b6966-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6966-120">Header</span></span>|<span data-ttu-id="b6966-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b6966-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6966-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6966-122">Authorization</span></span>|<span data-ttu-id="b6966-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6966-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6966-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6966-124">Accept</span></span>|<span data-ttu-id="b6966-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6966-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6966-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6966-126">Request body</span></span>
<span data-ttu-id="b6966-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsHealthMonitoringConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b6966-127">In the request body, supply a JSON representation for the windowsHealthMonitoringConfiguration object.</span></span>

<span data-ttu-id="b6966-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsHealthMonitoringConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b6966-128">The following table shows the properties that are required when you create the windowsHealthMonitoringConfiguration.</span></span>

|<span data-ttu-id="b6966-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6966-129">Property</span></span>|<span data-ttu-id="b6966-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6966-130">Type</span></span>|<span data-ttu-id="b6966-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6966-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6966-132">id</span><span class="sxs-lookup"><span data-stu-id="b6966-132">id</span></span>|<span data-ttu-id="b6966-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6966-133">String</span></span>|<span data-ttu-id="b6966-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b6966-134">Key of the entity.</span></span> <span data-ttu-id="b6966-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6966-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6966-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6966-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b6966-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6966-137">DateTimeOffset</span></span>|<span data-ttu-id="b6966-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b6966-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b6966-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6966-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6966-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b6966-140">roleScopeTagIds</span></span>|<span data-ttu-id="b6966-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6966-141">String collection</span></span>|<span data-ttu-id="b6966-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b6966-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b6966-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6966-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6966-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b6966-144">supportsScopeTags</span></span>|<span data-ttu-id="b6966-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6966-145">Boolean</span></span>|<span data-ttu-id="b6966-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b6966-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b6966-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b6966-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b6966-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b6966-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b6966-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6966-149">This property is read-only.</span></span> <span data-ttu-id="b6966-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6966-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6966-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b6966-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b6966-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b6966-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b6966-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="b6966-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b6966-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6966-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6966-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b6966-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b6966-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b6966-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b6966-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="b6966-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b6966-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6966-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6966-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b6966-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b6966-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b6966-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b6966-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="b6966-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b6966-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6966-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6966-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b6966-163">createdDateTime</span></span>|<span data-ttu-id="b6966-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6966-164">DateTimeOffset</span></span>|<span data-ttu-id="b6966-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b6966-165">DateTime the object was created.</span></span> <span data-ttu-id="b6966-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6966-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6966-167">descrição</span><span class="sxs-lookup"><span data-stu-id="b6966-167">description</span></span>|<span data-ttu-id="b6966-168">String</span><span class="sxs-lookup"><span data-stu-id="b6966-168">String</span></span>|<span data-ttu-id="b6966-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6966-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b6966-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6966-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6966-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b6966-171">displayName</span></span>|<span data-ttu-id="b6966-172">String</span><span class="sxs-lookup"><span data-stu-id="b6966-172">String</span></span>|<span data-ttu-id="b6966-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6966-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b6966-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6966-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6966-175">versão</span><span class="sxs-lookup"><span data-stu-id="b6966-175">version</span></span>|<span data-ttu-id="b6966-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b6966-176">Int32</span></span>|<span data-ttu-id="b6966-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6966-177">Version of the device configuration.</span></span> <span data-ttu-id="b6966-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b6966-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b6966-179">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="b6966-179">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="b6966-180">habilitação</span><span class="sxs-lookup"><span data-stu-id="b6966-180">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="b6966-181">Habilita o monitoramento de integridade do dispositivo no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b6966-181">Enables device health monitoring on the device.</span></span> <span data-ttu-id="b6966-182">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="b6966-182">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="b6966-183">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="b6966-183">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="b6966-184">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="b6966-184">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="b6966-185">Especifica o conjunto de eventos coletados do dispositivo onde o monitoramento de integridade está habilitado.</span><span class="sxs-lookup"><span data-stu-id="b6966-185">Specifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="b6966-186">Os valores possíveis são: `undefined`, `healthMonitoring`, `bootPerformance`.</span><span class="sxs-lookup"><span data-stu-id="b6966-186">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`.</span></span>|
|<span data-ttu-id="b6966-187">configDeviceHealthMonitoringCustomScope</span><span class="sxs-lookup"><span data-stu-id="b6966-187">configDeviceHealthMonitoringCustomScope</span></span>|<span data-ttu-id="b6966-188">String</span><span class="sxs-lookup"><span data-stu-id="b6966-188">String</span></span>|<span data-ttu-id="b6966-189">Especifica um conjunto personalizado de eventos coletados do dispositivo onde o monitoramento de integridade está habilitado</span><span class="sxs-lookup"><span data-stu-id="b6966-189">Specifies custom set of events collected from the device where health monitoring is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="b6966-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6966-190">Response</span></span>
<span data-ttu-id="b6966-191">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6966-191">If successful, this method returns a `201 Created` response code and a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6966-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6966-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6966-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6966-193">Request</span></span>
<span data-ttu-id="b6966-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6966-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b6966-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6966-195">Response</span></span>
<span data-ttu-id="b6966-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6966-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





