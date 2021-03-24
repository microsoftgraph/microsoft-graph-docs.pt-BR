---
title: Atualizar windowsHealthMonitoringConfiguration
description: Atualize as propriedades de um objeto windowsHealthMonitoringConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 914018f78b5a3f90594f1c03b6134f5387d65725
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127267"
---
# <a name="update-windowshealthmonitoringconfiguration"></a><span data-ttu-id="0e4a5-103">Atualizar windowsHealthMonitoringConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e4a5-103">Update windowsHealthMonitoringConfiguration</span></span>

<span data-ttu-id="0e4a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e4a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e4a5-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e4a5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e4a5-107">Atualize as propriedades de um [objeto windowsHealthMonitoringConfiguration.](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4a5-107">Update the properties of a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e4a5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0e4a5-108">Prerequisites</span></span>
<span data-ttu-id="0e4a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e4a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e4a5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e4a5-111">Permission type</span></span>|<span data-ttu-id="0e4a5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e4a5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e4a5-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e4a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e4a5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e4a5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e4a5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e4a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e4a5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-116">Not supported.</span></span>|
|<span data-ttu-id="0e4a5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e4a5-117">Application</span></span>|<span data-ttu-id="0e4a5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e4a5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e4a5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e4a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0e4a5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e4a5-120">Request headers</span></span>
|<span data-ttu-id="0e4a5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e4a5-121">Header</span></span>|<span data-ttu-id="0e4a5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0e4a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e4a5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e4a5-123">Authorization</span></span>|<span data-ttu-id="0e4a5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e4a5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0e4a5-125">Accept</span></span>|<span data-ttu-id="0e4a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e4a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e4a5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e4a5-127">Request body</span></span>
<span data-ttu-id="0e4a5-128">No corpo da solicitação, fornece uma representação JSON para o [objeto windowsHealthMonitoringConfiguration.](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4a5-128">In the request body, supply a JSON representation for the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

<span data-ttu-id="0e4a5-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0e4a5-129">The following table shows the properties that are required when you create the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md).</span></span>

|<span data-ttu-id="0e4a5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e4a5-130">Property</span></span>|<span data-ttu-id="0e4a5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e4a5-131">Type</span></span>|<span data-ttu-id="0e4a5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e4a5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e4a5-133">id</span><span class="sxs-lookup"><span data-stu-id="0e4a5-133">id</span></span>|<span data-ttu-id="0e4a5-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e4a5-134">String</span></span>|<span data-ttu-id="0e4a5-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-135">Key of the entity.</span></span> <span data-ttu-id="0e4a5-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4a5-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4a5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e4a5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0e4a5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e4a5-138">DateTimeOffset</span></span>|<span data-ttu-id="0e4a5-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0e4a5-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4a5-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4a5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0e4a5-141">roleScopeTagIds</span></span>|<span data-ttu-id="0e4a5-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e4a5-142">String collection</span></span>|<span data-ttu-id="0e4a5-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0e4a5-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4a5-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4a5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0e4a5-145">supportsScopeTags</span></span>|<span data-ttu-id="0e4a5-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="0e4a5-146">Boolean</span></span>|<span data-ttu-id="0e4a5-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0e4a5-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0e4a5-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0e4a5-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-150">This property is read-only.</span></span> <span data-ttu-id="0e4a5-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4a5-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4a5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0e4a5-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0e4a5-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0e4a5-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0e4a5-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0e4a5-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4a5-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4a5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0e4a5-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0e4a5-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0e4a5-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0e4a5-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0e4a5-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4a5-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4a5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0e4a5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0e4a5-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0e4a5-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0e4a5-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0e4a5-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4a5-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4a5-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e4a5-164">createdDateTime</span></span>|<span data-ttu-id="0e4a5-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e4a5-165">DateTimeOffset</span></span>|<span data-ttu-id="0e4a5-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-166">DateTime the object was created.</span></span> <span data-ttu-id="0e4a5-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4a5-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4a5-168">descrição</span><span class="sxs-lookup"><span data-stu-id="0e4a5-168">description</span></span>|<span data-ttu-id="0e4a5-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e4a5-169">String</span></span>|<span data-ttu-id="0e4a5-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0e4a5-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4a5-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4a5-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0e4a5-172">displayName</span></span>|<span data-ttu-id="0e4a5-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e4a5-173">String</span></span>|<span data-ttu-id="0e4a5-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0e4a5-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4a5-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4a5-176">versão</span><span class="sxs-lookup"><span data-stu-id="0e4a5-176">version</span></span>|<span data-ttu-id="0e4a5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0e4a5-177">Int32</span></span>|<span data-ttu-id="0e4a5-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-178">Version of the device configuration.</span></span> <span data-ttu-id="0e4a5-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0e4a5-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0e4a5-180">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="0e4a5-180">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="0e4a5-181">enablement</span><span class="sxs-lookup"><span data-stu-id="0e4a5-181">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="0e4a5-182">Habilita o monitoramento de saúde do dispositivo no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-182">Enables device health monitoring on the device.</span></span> <span data-ttu-id="0e4a5-183">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-183">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="0e4a5-184">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="0e4a5-184">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="0e4a5-185">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="0e4a5-185">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="0e4a5-186">Especifica o conjunto de eventos coletados do dispositivo onde o monitoramento de saúde está habilitado.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-186">Specifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="0e4a5-187">Os valores possíveis são: `undefined`, `healthMonitoring`, `bootPerformance`, `windowsUpdates`.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-187">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`, `windowsUpdates`.</span></span>|
|<span data-ttu-id="0e4a5-188">configDeviceHealthMonitoringCustomScope</span><span class="sxs-lookup"><span data-stu-id="0e4a5-188">configDeviceHealthMonitoringCustomScope</span></span>|<span data-ttu-id="0e4a5-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e4a5-189">String</span></span>|<span data-ttu-id="0e4a5-190">Especifica o conjunto personalizado de eventos coletados do dispositivo em que o monitoramento de saúde está habilitado</span><span class="sxs-lookup"><span data-stu-id="0e4a5-190">Specifies custom set of events collected from the device where health monitoring is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="0e4a5-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e4a5-191">Response</span></span>
<span data-ttu-id="0e4a5-192">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-192">If successful, this method returns a `200 OK` response code and an updated [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e4a5-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e4a5-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e4a5-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e4a5-194">Request</span></span>
<span data-ttu-id="0e4a5-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="0e4a5-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e4a5-196">Response</span></span>
<span data-ttu-id="0e4a5-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e4a5-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




