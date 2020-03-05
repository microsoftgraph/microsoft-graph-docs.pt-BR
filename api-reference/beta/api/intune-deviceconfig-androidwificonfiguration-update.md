---
title: Atualizar androidWiFiConfiguration
description: Atualiza as propriedades de um objeto androidWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 43bfe7835c0cb2ee34fe23975df7893ad3137343
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449604"
---
# <a name="update-androidwificonfiguration"></a><span data-ttu-id="52944-103">Atualizar androidWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="52944-103">Update androidWiFiConfiguration</span></span>

<span data-ttu-id="52944-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="52944-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52944-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52944-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52944-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52944-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52944-107">Atualiza as propriedades de um objeto [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="52944-107">Update the properties of a [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52944-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52944-108">Prerequisites</span></span>
<span data-ttu-id="52944-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52944-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52944-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52944-111">Permission type</span></span>|<span data-ttu-id="52944-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="52944-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52944-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52944-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52944-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52944-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="52944-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52944-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52944-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52944-116">Not supported.</span></span>|
|<span data-ttu-id="52944-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52944-117">Application</span></span>|<span data-ttu-id="52944-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52944-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52944-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52944-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="52944-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52944-120">Request headers</span></span>
|<span data-ttu-id="52944-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52944-121">Header</span></span>|<span data-ttu-id="52944-122">Valor</span><span class="sxs-lookup"><span data-stu-id="52944-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52944-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="52944-123">Authorization</span></span>|<span data-ttu-id="52944-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52944-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52944-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52944-125">Accept</span></span>|<span data-ttu-id="52944-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52944-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52944-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52944-127">Request body</span></span>
<span data-ttu-id="52944-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="52944-128">In the request body, supply a JSON representation for the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

<span data-ttu-id="52944-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="52944-129">The following table shows the properties that are required when you create the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span>

|<span data-ttu-id="52944-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52944-130">Property</span></span>|<span data-ttu-id="52944-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="52944-131">Type</span></span>|<span data-ttu-id="52944-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="52944-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52944-133">id</span><span class="sxs-lookup"><span data-stu-id="52944-133">id</span></span>|<span data-ttu-id="52944-134">String</span><span class="sxs-lookup"><span data-stu-id="52944-134">String</span></span>|<span data-ttu-id="52944-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="52944-135">Key of the entity.</span></span> <span data-ttu-id="52944-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52944-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52944-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52944-137">lastModifiedDateTime</span></span>|<span data-ttu-id="52944-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52944-138">DateTimeOffset</span></span>|<span data-ttu-id="52944-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="52944-139">DateTime the object was last modified.</span></span> <span data-ttu-id="52944-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52944-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52944-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="52944-141">roleScopeTagIds</span></span>|<span data-ttu-id="52944-142">String collection</span><span class="sxs-lookup"><span data-stu-id="52944-142">String collection</span></span>|<span data-ttu-id="52944-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="52944-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="52944-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52944-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52944-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="52944-145">supportsScopeTags</span></span>|<span data-ttu-id="52944-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="52944-146">Boolean</span></span>|<span data-ttu-id="52944-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="52944-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="52944-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="52944-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="52944-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="52944-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="52944-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="52944-150">This property is read-only.</span></span> <span data-ttu-id="52944-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52944-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52944-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="52944-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="52944-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="52944-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="52944-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="52944-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="52944-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52944-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52944-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="52944-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="52944-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="52944-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="52944-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="52944-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="52944-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52944-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52944-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="52944-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="52944-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="52944-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="52944-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="52944-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="52944-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52944-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52944-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="52944-164">createdDateTime</span></span>|<span data-ttu-id="52944-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52944-165">DateTimeOffset</span></span>|<span data-ttu-id="52944-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="52944-166">DateTime the object was created.</span></span> <span data-ttu-id="52944-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52944-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52944-168">description</span><span class="sxs-lookup"><span data-stu-id="52944-168">description</span></span>|<span data-ttu-id="52944-169">String</span><span class="sxs-lookup"><span data-stu-id="52944-169">String</span></span>|<span data-ttu-id="52944-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52944-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="52944-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52944-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52944-172">displayName</span><span class="sxs-lookup"><span data-stu-id="52944-172">displayName</span></span>|<span data-ttu-id="52944-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52944-173">String</span></span>|<span data-ttu-id="52944-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52944-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="52944-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52944-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52944-176">versão</span><span class="sxs-lookup"><span data-stu-id="52944-176">version</span></span>|<span data-ttu-id="52944-177">Int32</span><span class="sxs-lookup"><span data-stu-id="52944-177">Int32</span></span>|<span data-ttu-id="52944-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="52944-178">Version of the device configuration.</span></span> <span data-ttu-id="52944-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="52944-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52944-180">NetworkName</span><span class="sxs-lookup"><span data-stu-id="52944-180">networkName</span></span>|<span data-ttu-id="52944-181">String</span><span class="sxs-lookup"><span data-stu-id="52944-181">String</span></span>|<span data-ttu-id="52944-182">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="52944-182">Network Name</span></span>|
|<span data-ttu-id="52944-183">SSID</span><span class="sxs-lookup"><span data-stu-id="52944-183">ssid</span></span>|<span data-ttu-id="52944-184">String</span><span class="sxs-lookup"><span data-stu-id="52944-184">String</span></span>|<span data-ttu-id="52944-185">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="52944-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="52944-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="52944-186">connectAutomatically</span></span>|<span data-ttu-id="52944-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="52944-187">Boolean</span></span>|<span data-ttu-id="52944-188">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="52944-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="52944-189">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="52944-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="52944-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="52944-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="52944-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="52944-191">Boolean</span></span>|<span data-ttu-id="52944-192">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="52944-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="52944-193">à</span><span class="sxs-lookup"><span data-stu-id="52944-193">wiFiSecurityType</span></span>|[<span data-ttu-id="52944-194">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="52944-194">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="52944-195">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="52944-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="52944-196">Os valores possíveis são: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="52944-196">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="52944-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="52944-197">Response</span></span>
<span data-ttu-id="52944-198">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52944-198">If successful, this method returns a `200 OK` response code and an updated [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52944-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52944-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="52944-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52944-200">Request</span></span>
<span data-ttu-id="52944-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52944-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="52944-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="52944-202">Response</span></span>
<span data-ttu-id="52944-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52944-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





