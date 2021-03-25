---
title: Criar windowsHealthMonitoringConfiguration
description: Crie um novo objeto windowsHealthMonitoringConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d840f3a25d4fa8621a945a497030fbcdcf3d3b7d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154909"
---
# <a name="create-windowshealthmonitoringconfiguration"></a><span data-ttu-id="ca951-103">Criar windowsHealthMonitoringConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca951-103">Create windowsHealthMonitoringConfiguration</span></span>

<span data-ttu-id="ca951-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca951-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca951-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca951-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca951-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca951-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca951-107">Crie um novo [objeto windowsHealthMonitoringConfiguration.](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca951-107">Create a new [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca951-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca951-108">Prerequisites</span></span>
<span data-ttu-id="ca951-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca951-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca951-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca951-111">Permission type</span></span>|<span data-ttu-id="ca951-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca951-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca951-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca951-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca951-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca951-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca951-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca951-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca951-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca951-116">Not supported.</span></span>|
|<span data-ttu-id="ca951-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca951-117">Application</span></span>|<span data-ttu-id="ca951-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca951-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca951-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca951-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ca951-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca951-120">Request headers</span></span>
|<span data-ttu-id="ca951-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca951-121">Header</span></span>|<span data-ttu-id="ca951-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ca951-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca951-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca951-123">Authorization</span></span>|<span data-ttu-id="ca951-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca951-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca951-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca951-125">Accept</span></span>|<span data-ttu-id="ca951-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca951-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca951-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca951-127">Request body</span></span>
<span data-ttu-id="ca951-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsHealthMonitoringConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ca951-128">In the request body, supply a JSON representation for the windowsHealthMonitoringConfiguration object.</span></span>

<span data-ttu-id="ca951-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsHealthMonitoringConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ca951-129">The following table shows the properties that are required when you create the windowsHealthMonitoringConfiguration.</span></span>

|<span data-ttu-id="ca951-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca951-130">Property</span></span>|<span data-ttu-id="ca951-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca951-131">Type</span></span>|<span data-ttu-id="ca951-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca951-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca951-133">id</span><span class="sxs-lookup"><span data-stu-id="ca951-133">id</span></span>|<span data-ttu-id="ca951-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca951-134">String</span></span>|<span data-ttu-id="ca951-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ca951-135">Key of the entity.</span></span> <span data-ttu-id="ca951-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca951-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca951-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca951-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ca951-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca951-138">DateTimeOffset</span></span>|<span data-ttu-id="ca951-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ca951-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ca951-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca951-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca951-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ca951-141">roleScopeTagIds</span></span>|<span data-ttu-id="ca951-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca951-142">String collection</span></span>|<span data-ttu-id="ca951-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="ca951-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ca951-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca951-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca951-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ca951-145">supportsScopeTags</span></span>|<span data-ttu-id="ca951-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca951-146">Boolean</span></span>|<span data-ttu-id="ca951-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ca951-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ca951-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ca951-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ca951-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ca951-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ca951-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca951-150">This property is read-only.</span></span> <span data-ttu-id="ca951-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca951-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca951-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ca951-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ca951-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ca951-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ca951-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ca951-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ca951-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca951-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca951-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ca951-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ca951-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ca951-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ca951-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ca951-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ca951-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca951-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca951-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ca951-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ca951-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ca951-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ca951-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ca951-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ca951-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca951-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca951-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca951-164">createdDateTime</span></span>|<span data-ttu-id="ca951-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca951-165">DateTimeOffset</span></span>|<span data-ttu-id="ca951-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ca951-166">DateTime the object was created.</span></span> <span data-ttu-id="ca951-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca951-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca951-168">descrição</span><span class="sxs-lookup"><span data-stu-id="ca951-168">description</span></span>|<span data-ttu-id="ca951-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca951-169">String</span></span>|<span data-ttu-id="ca951-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca951-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ca951-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca951-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca951-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ca951-172">displayName</span></span>|<span data-ttu-id="ca951-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca951-173">String</span></span>|<span data-ttu-id="ca951-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca951-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ca951-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca951-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca951-176">versão</span><span class="sxs-lookup"><span data-stu-id="ca951-176">version</span></span>|<span data-ttu-id="ca951-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ca951-177">Int32</span></span>|<span data-ttu-id="ca951-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca951-178">Version of the device configuration.</span></span> <span data-ttu-id="ca951-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca951-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca951-180">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="ca951-180">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="ca951-181">enablement</span><span class="sxs-lookup"><span data-stu-id="ca951-181">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="ca951-182">Habilita o monitoramento de saúde do dispositivo no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca951-182">Enables device health monitoring on the device.</span></span> <span data-ttu-id="ca951-183">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="ca951-183">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ca951-184">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="ca951-184">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="ca951-185">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="ca951-185">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="ca951-186">Especifica o conjunto de eventos coletados do dispositivo onde o monitoramento de saúde está habilitado.</span><span class="sxs-lookup"><span data-stu-id="ca951-186">Specifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="ca951-187">Os valores possíveis são: `undefined`, `healthMonitoring`, `bootPerformance`, `windowsUpdates`.</span><span class="sxs-lookup"><span data-stu-id="ca951-187">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`, `windowsUpdates`.</span></span>|
|<span data-ttu-id="ca951-188">configDeviceHealthMonitoringCustomScope</span><span class="sxs-lookup"><span data-stu-id="ca951-188">configDeviceHealthMonitoringCustomScope</span></span>|<span data-ttu-id="ca951-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca951-189">String</span></span>|<span data-ttu-id="ca951-190">Especifica o conjunto personalizado de eventos coletados do dispositivo em que o monitoramento de saúde está habilitado</span><span class="sxs-lookup"><span data-stu-id="ca951-190">Specifies custom set of events collected from the device where health monitoring is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="ca951-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca951-191">Response</span></span>
<span data-ttu-id="ca951-192">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca951-192">If successful, this method returns a `201 Created` response code and a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca951-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca951-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca951-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca951-194">Request</span></span>
<span data-ttu-id="ca951-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca951-195">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ca951-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca951-196">Response</span></span>
<span data-ttu-id="ca951-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca951-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




