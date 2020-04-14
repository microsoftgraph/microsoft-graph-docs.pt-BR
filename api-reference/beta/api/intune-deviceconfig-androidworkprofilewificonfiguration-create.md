---
title: Criar androidWorkProfileWiFiConfiguration
description: Criar um novo objeto androidWorkProfileWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ddc1523d68fce2fa6bc6e8a92e0dacc7a092f56
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43434594"
---
# <a name="create-androidworkprofilewificonfiguration"></a><span data-ttu-id="b1309-103">Criar androidWorkProfileWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="b1309-103">Create androidWorkProfileWiFiConfiguration</span></span>

<span data-ttu-id="b1309-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1309-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1309-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1309-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1309-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1309-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1309-107">Criar um novo objeto [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b1309-107">Create a new [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1309-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b1309-108">Prerequisites</span></span>
<span data-ttu-id="b1309-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1309-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1309-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1309-111">Permission type</span></span>|<span data-ttu-id="b1309-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b1309-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1309-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1309-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1309-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1309-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1309-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1309-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1309-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1309-116">Not supported.</span></span>|
|<span data-ttu-id="b1309-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1309-117">Application</span></span>|<span data-ttu-id="b1309-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1309-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1309-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1309-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b1309-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1309-120">Request headers</span></span>
|<span data-ttu-id="b1309-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1309-121">Header</span></span>|<span data-ttu-id="b1309-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b1309-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1309-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1309-123">Authorization</span></span>|<span data-ttu-id="b1309-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1309-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1309-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b1309-125">Accept</span></span>|<span data-ttu-id="b1309-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1309-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1309-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1309-127">Request body</span></span>
<span data-ttu-id="b1309-128">No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfileWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b1309-128">In the request body, supply a JSON representation for the androidWorkProfileWiFiConfiguration object.</span></span>

<span data-ttu-id="b1309-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWorkProfileWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b1309-129">The following table shows the properties that are required when you create the androidWorkProfileWiFiConfiguration.</span></span>

|<span data-ttu-id="b1309-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1309-130">Property</span></span>|<span data-ttu-id="b1309-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1309-131">Type</span></span>|<span data-ttu-id="b1309-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1309-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1309-133">id</span><span class="sxs-lookup"><span data-stu-id="b1309-133">id</span></span>|<span data-ttu-id="b1309-134">String</span><span class="sxs-lookup"><span data-stu-id="b1309-134">String</span></span>|<span data-ttu-id="b1309-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b1309-135">Key of the entity.</span></span> <span data-ttu-id="b1309-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1309-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1309-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1309-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b1309-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1309-138">DateTimeOffset</span></span>|<span data-ttu-id="b1309-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b1309-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b1309-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1309-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1309-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b1309-141">roleScopeTagIds</span></span>|<span data-ttu-id="b1309-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b1309-142">String collection</span></span>|<span data-ttu-id="b1309-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b1309-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b1309-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1309-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1309-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b1309-145">supportsScopeTags</span></span>|<span data-ttu-id="b1309-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1309-146">Boolean</span></span>|<span data-ttu-id="b1309-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b1309-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b1309-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b1309-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b1309-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b1309-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b1309-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b1309-150">This property is read-only.</span></span> <span data-ttu-id="b1309-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1309-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1309-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b1309-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b1309-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b1309-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b1309-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="b1309-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b1309-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1309-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1309-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b1309-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b1309-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b1309-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b1309-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="b1309-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b1309-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1309-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1309-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b1309-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b1309-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b1309-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b1309-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="b1309-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b1309-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1309-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1309-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1309-164">createdDateTime</span></span>|<span data-ttu-id="b1309-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1309-165">DateTimeOffset</span></span>|<span data-ttu-id="b1309-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b1309-166">DateTime the object was created.</span></span> <span data-ttu-id="b1309-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1309-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1309-168">description</span><span class="sxs-lookup"><span data-stu-id="b1309-168">description</span></span>|<span data-ttu-id="b1309-169">String</span><span class="sxs-lookup"><span data-stu-id="b1309-169">String</span></span>|<span data-ttu-id="b1309-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1309-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b1309-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1309-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1309-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b1309-172">displayName</span></span>|<span data-ttu-id="b1309-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1309-173">String</span></span>|<span data-ttu-id="b1309-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1309-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b1309-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1309-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1309-176">versão</span><span class="sxs-lookup"><span data-stu-id="b1309-176">version</span></span>|<span data-ttu-id="b1309-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b1309-177">Int32</span></span>|<span data-ttu-id="b1309-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b1309-178">Version of the device configuration.</span></span> <span data-ttu-id="b1309-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1309-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1309-180">NetworkName</span><span class="sxs-lookup"><span data-stu-id="b1309-180">networkName</span></span>|<span data-ttu-id="b1309-181">String</span><span class="sxs-lookup"><span data-stu-id="b1309-181">String</span></span>|<span data-ttu-id="b1309-182">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="b1309-182">Network Name</span></span>|
|<span data-ttu-id="b1309-183">SSID</span><span class="sxs-lookup"><span data-stu-id="b1309-183">ssid</span></span>|<span data-ttu-id="b1309-184">String</span><span class="sxs-lookup"><span data-stu-id="b1309-184">String</span></span>|<span data-ttu-id="b1309-185">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b1309-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="b1309-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="b1309-186">connectAutomatically</span></span>|<span data-ttu-id="b1309-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1309-187">Boolean</span></span>|<span data-ttu-id="b1309-188">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="b1309-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="b1309-189">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b1309-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="b1309-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="b1309-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="b1309-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1309-191">Boolean</span></span>|<span data-ttu-id="b1309-192">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b1309-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="b1309-193">à</span><span class="sxs-lookup"><span data-stu-id="b1309-193">wiFiSecurityType</span></span>|[<span data-ttu-id="b1309-194">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b1309-194">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="b1309-195">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="b1309-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="b1309-196">Os valores possíveis são: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="b1309-196">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="b1309-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1309-197">Response</span></span>
<span data-ttu-id="b1309-198">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1309-198">If successful, this method returns a `201 Created` response code and a [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1309-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1309-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1309-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1309-200">Request</span></span>
<span data-ttu-id="b1309-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1309-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1219

{
  "@odata.type": "#microsoft.graph.androidWorkProfileWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="b1309-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1309-202">Response</span></span>
<span data-ttu-id="b1309-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1309-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1391

{
  "@odata.type": "#microsoft.graph.androidWorkProfileWiFiConfiguration",
  "id": "8400d131-d131-8400-31d1-008431d10084",
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



