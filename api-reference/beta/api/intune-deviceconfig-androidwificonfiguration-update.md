---
title: Atualizar androidWiFiConfiguration
description: Atualiza as propriedades de um objeto androidWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 96a6ac4ea96e9b6bb20cddb406cb536029703260
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954213"
---
# <a name="update-androidwificonfiguration"></a><span data-ttu-id="06810-103">Atualizar androidWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="06810-103">Update androidWiFiConfiguration</span></span>

> <span data-ttu-id="06810-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="06810-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06810-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06810-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06810-106">Atualiza as propriedades de um objeto [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="06810-106">Update the properties of a [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06810-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="06810-107">Prerequisites</span></span>
<span data-ttu-id="06810-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06810-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06810-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06810-110">Permission type</span></span>|<span data-ttu-id="06810-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="06810-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06810-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06810-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06810-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06810-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06810-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06810-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06810-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06810-115">Not supported.</span></span>|
|<span data-ttu-id="06810-116">Application</span><span class="sxs-lookup"><span data-stu-id="06810-116">Application</span></span>|<span data-ttu-id="06810-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06810-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06810-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06810-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="06810-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06810-119">Request headers</span></span>
|<span data-ttu-id="06810-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="06810-120">Header</span></span>|<span data-ttu-id="06810-121">Valor</span><span class="sxs-lookup"><span data-stu-id="06810-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06810-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="06810-122">Authorization</span></span>|<span data-ttu-id="06810-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06810-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06810-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="06810-124">Accept</span></span>|<span data-ttu-id="06810-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06810-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06810-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06810-126">Request body</span></span>
<span data-ttu-id="06810-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="06810-127">In the request body, supply a JSON representation for the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

<span data-ttu-id="06810-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06810-128">The following table shows the properties that are required when you create the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span>

|<span data-ttu-id="06810-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06810-129">Property</span></span>|<span data-ttu-id="06810-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="06810-130">Type</span></span>|<span data-ttu-id="06810-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="06810-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06810-132">id</span><span class="sxs-lookup"><span data-stu-id="06810-132">id</span></span>|<span data-ttu-id="06810-133">String</span><span class="sxs-lookup"><span data-stu-id="06810-133">String</span></span>|<span data-ttu-id="06810-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="06810-134">Key of the entity.</span></span> <span data-ttu-id="06810-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06810-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06810-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06810-136">lastModifiedDateTime</span></span>|<span data-ttu-id="06810-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06810-137">DateTimeOffset</span></span>|<span data-ttu-id="06810-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="06810-138">DateTime the object was last modified.</span></span> <span data-ttu-id="06810-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06810-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06810-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="06810-140">roleScopeTagIds</span></span>|<span data-ttu-id="06810-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="06810-141">String collection</span></span>|<span data-ttu-id="06810-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="06810-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="06810-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06810-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06810-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="06810-144">supportsScopeTags</span></span>|<span data-ttu-id="06810-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="06810-145">Boolean</span></span>|<span data-ttu-id="06810-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="06810-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="06810-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="06810-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="06810-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="06810-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="06810-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="06810-149">This property is read-only.</span></span> <span data-ttu-id="06810-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06810-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06810-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="06810-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="06810-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="06810-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="06810-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="06810-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="06810-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06810-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06810-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="06810-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="06810-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="06810-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="06810-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="06810-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="06810-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06810-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06810-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="06810-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="06810-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="06810-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="06810-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="06810-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="06810-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06810-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06810-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06810-163">createdDateTime</span></span>|<span data-ttu-id="06810-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06810-164">DateTimeOffset</span></span>|<span data-ttu-id="06810-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="06810-165">DateTime the object was created.</span></span> <span data-ttu-id="06810-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06810-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06810-167">description</span><span class="sxs-lookup"><span data-stu-id="06810-167">description</span></span>|<span data-ttu-id="06810-168">String</span><span class="sxs-lookup"><span data-stu-id="06810-168">String</span></span>|<span data-ttu-id="06810-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06810-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="06810-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06810-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06810-171">displayName</span><span class="sxs-lookup"><span data-stu-id="06810-171">displayName</span></span>|<span data-ttu-id="06810-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06810-172">String</span></span>|<span data-ttu-id="06810-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06810-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="06810-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06810-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06810-175">versão</span><span class="sxs-lookup"><span data-stu-id="06810-175">version</span></span>|<span data-ttu-id="06810-176">Int32</span><span class="sxs-lookup"><span data-stu-id="06810-176">Int32</span></span>|<span data-ttu-id="06810-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06810-177">Version of the device configuration.</span></span> <span data-ttu-id="06810-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="06810-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06810-179">NetworkName</span><span class="sxs-lookup"><span data-stu-id="06810-179">networkName</span></span>|<span data-ttu-id="06810-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="06810-180">String</span></span>|<span data-ttu-id="06810-181">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="06810-181">Network Name</span></span>|
|<span data-ttu-id="06810-182">SSID</span><span class="sxs-lookup"><span data-stu-id="06810-182">ssid</span></span>|<span data-ttu-id="06810-183">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="06810-183">String</span></span>|<span data-ttu-id="06810-184">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="06810-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="06810-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="06810-185">connectAutomatically</span></span>|<span data-ttu-id="06810-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="06810-186">Boolean</span></span>|<span data-ttu-id="06810-187">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="06810-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="06810-188">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="06810-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="06810-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="06810-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="06810-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="06810-190">Boolean</span></span>|<span data-ttu-id="06810-191">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="06810-191">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="06810-192">à</span><span class="sxs-lookup"><span data-stu-id="06810-192">wiFiSecurityType</span></span>|[<span data-ttu-id="06810-193">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="06810-193">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="06810-194">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="06810-194">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="06810-195">Os valores possíveis são: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="06810-195">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="06810-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="06810-196">Response</span></span>
<span data-ttu-id="06810-197">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06810-197">If successful, this method returns a `200 OK` response code and an updated [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06810-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06810-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="06810-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06810-199">Request</span></span>
<span data-ttu-id="06810-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06810-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1208

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise"
}
```

### <a name="response"></a><span data-ttu-id="06810-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="06810-201">Response</span></span>
<span data-ttu-id="06810-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06810-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1380

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
  "id": "51cfd26f-d26f-51cf-6fd2-cf516fd2cf51",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise"
}
```





