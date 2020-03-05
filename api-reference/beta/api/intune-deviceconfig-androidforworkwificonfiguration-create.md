---
title: Criar androidForWorkWiFiConfiguration
description: Criar um novo objeto androidForWorkWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9be76883610634c7af0ce45247a7a7f706d93009
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449751"
---
# <a name="create-androidforworkwificonfiguration"></a><span data-ttu-id="a1054-103">Criar androidForWorkWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1054-103">Create androidForWorkWiFiConfiguration</span></span>

<span data-ttu-id="a1054-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a1054-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1054-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1054-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1054-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1054-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1054-107">Criar um novo objeto [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a1054-107">Create a new [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1054-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1054-108">Prerequisites</span></span>
<span data-ttu-id="a1054-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1054-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1054-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1054-111">Permission type</span></span>|<span data-ttu-id="a1054-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1054-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1054-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1054-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1054-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1054-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1054-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1054-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1054-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1054-116">Not supported.</span></span>|
|<span data-ttu-id="a1054-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1054-117">Application</span></span>|<span data-ttu-id="a1054-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1054-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1054-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1054-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a1054-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1054-120">Request headers</span></span>
|<span data-ttu-id="a1054-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1054-121">Header</span></span>|<span data-ttu-id="a1054-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a1054-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1054-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1054-123">Authorization</span></span>|<span data-ttu-id="a1054-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1054-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1054-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1054-125">Accept</span></span>|<span data-ttu-id="a1054-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1054-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1054-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1054-127">Request body</span></span>
<span data-ttu-id="a1054-128">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a1054-128">In the request body, supply a JSON representation for the androidForWorkWiFiConfiguration object.</span></span>

<span data-ttu-id="a1054-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a1054-129">The following table shows the properties that are required when you create the androidForWorkWiFiConfiguration.</span></span>

|<span data-ttu-id="a1054-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1054-130">Property</span></span>|<span data-ttu-id="a1054-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1054-131">Type</span></span>|<span data-ttu-id="a1054-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1054-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1054-133">id</span><span class="sxs-lookup"><span data-stu-id="a1054-133">id</span></span>|<span data-ttu-id="a1054-134">String</span><span class="sxs-lookup"><span data-stu-id="a1054-134">String</span></span>|<span data-ttu-id="a1054-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a1054-135">Key of the entity.</span></span> <span data-ttu-id="a1054-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1054-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1054-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1054-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a1054-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1054-138">DateTimeOffset</span></span>|<span data-ttu-id="a1054-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a1054-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a1054-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1054-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1054-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a1054-141">roleScopeTagIds</span></span>|<span data-ttu-id="a1054-142">String collection</span><span class="sxs-lookup"><span data-stu-id="a1054-142">String collection</span></span>|<span data-ttu-id="a1054-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a1054-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a1054-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1054-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1054-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a1054-145">supportsScopeTags</span></span>|<span data-ttu-id="a1054-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1054-146">Boolean</span></span>|<span data-ttu-id="a1054-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a1054-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a1054-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a1054-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a1054-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a1054-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a1054-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a1054-150">This property is read-only.</span></span> <span data-ttu-id="a1054-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1054-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1054-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a1054-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a1054-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a1054-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a1054-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="a1054-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a1054-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1054-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1054-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a1054-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a1054-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a1054-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a1054-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="a1054-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a1054-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1054-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1054-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a1054-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a1054-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a1054-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a1054-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="a1054-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a1054-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1054-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1054-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1054-164">createdDateTime</span></span>|<span data-ttu-id="a1054-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1054-165">DateTimeOffset</span></span>|<span data-ttu-id="a1054-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a1054-166">DateTime the object was created.</span></span> <span data-ttu-id="a1054-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1054-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1054-168">description</span><span class="sxs-lookup"><span data-stu-id="a1054-168">description</span></span>|<span data-ttu-id="a1054-169">String</span><span class="sxs-lookup"><span data-stu-id="a1054-169">String</span></span>|<span data-ttu-id="a1054-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1054-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a1054-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1054-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1054-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a1054-172">displayName</span></span>|<span data-ttu-id="a1054-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1054-173">String</span></span>|<span data-ttu-id="a1054-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1054-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a1054-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1054-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1054-176">versão</span><span class="sxs-lookup"><span data-stu-id="a1054-176">version</span></span>|<span data-ttu-id="a1054-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a1054-177">Int32</span></span>|<span data-ttu-id="a1054-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a1054-178">Version of the device configuration.</span></span> <span data-ttu-id="a1054-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1054-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1054-180">NetworkName</span><span class="sxs-lookup"><span data-stu-id="a1054-180">networkName</span></span>|<span data-ttu-id="a1054-181">String</span><span class="sxs-lookup"><span data-stu-id="a1054-181">String</span></span>|<span data-ttu-id="a1054-182">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="a1054-182">Network Name</span></span>|
|<span data-ttu-id="a1054-183">SSID</span><span class="sxs-lookup"><span data-stu-id="a1054-183">ssid</span></span>|<span data-ttu-id="a1054-184">String</span><span class="sxs-lookup"><span data-stu-id="a1054-184">String</span></span>|<span data-ttu-id="a1054-185">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a1054-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="a1054-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="a1054-186">connectAutomatically</span></span>|<span data-ttu-id="a1054-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1054-187">Boolean</span></span>|<span data-ttu-id="a1054-188">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="a1054-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="a1054-189">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="a1054-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="a1054-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="a1054-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="a1054-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1054-191">Boolean</span></span>|<span data-ttu-id="a1054-192">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a1054-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="a1054-193">à</span><span class="sxs-lookup"><span data-stu-id="a1054-193">wiFiSecurityType</span></span>|[<span data-ttu-id="a1054-194">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="a1054-194">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="a1054-195">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="a1054-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="a1054-196">Os valores possíveis são: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="a1054-196">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="a1054-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1054-197">Response</span></span>
<span data-ttu-id="a1054-198">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1054-198">If successful, this method returns a `201 Created` response code and a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1054-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1054-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1054-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1054-200">Request</span></span>
<span data-ttu-id="a1054-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1054-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1215

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="a1054-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1054-202">Response</span></span>
<span data-ttu-id="a1054-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1054-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1387

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
  "id": "58bcfe05-fe05-58bc-05fe-bc5805febc58",
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





