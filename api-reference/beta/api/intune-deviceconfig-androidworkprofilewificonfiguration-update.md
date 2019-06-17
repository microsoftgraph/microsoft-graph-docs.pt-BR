---
title: Atualizar androidWorkProfileWiFiConfiguration
description: Atualiza as propriedades de um objeto androidWorkProfileWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0015b605c8601a8c0e58ca32566aadfbe5dfaec9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968865"
---
# <a name="update-androidworkprofilewificonfiguration"></a><span data-ttu-id="b582b-103">Atualizar androidWorkProfileWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="b582b-103">Update androidWorkProfileWiFiConfiguration</span></span>

> <span data-ttu-id="b582b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b582b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b582b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b582b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b582b-106">Atualiza as propriedades de um objeto [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b582b-106">Update the properties of a [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b582b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b582b-107">Prerequisites</span></span>
<span data-ttu-id="b582b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b582b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b582b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b582b-110">Permission type</span></span>|<span data-ttu-id="b582b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b582b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b582b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b582b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b582b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b582b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b582b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b582b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b582b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b582b-115">Not supported.</span></span>|
|<span data-ttu-id="b582b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b582b-116">Application</span></span>|<span data-ttu-id="b582b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b582b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b582b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b582b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b582b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b582b-119">Request headers</span></span>
|<span data-ttu-id="b582b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b582b-120">Header</span></span>|<span data-ttu-id="b582b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b582b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b582b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b582b-122">Authorization</span></span>|<span data-ttu-id="b582b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b582b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b582b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b582b-124">Accept</span></span>|<span data-ttu-id="b582b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b582b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b582b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b582b-126">Request body</span></span>
<span data-ttu-id="b582b-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b582b-127">In the request body, supply a JSON representation for the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>

<span data-ttu-id="b582b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b582b-128">The following table shows the properties that are required when you create the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span>

|<span data-ttu-id="b582b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b582b-129">Property</span></span>|<span data-ttu-id="b582b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b582b-130">Type</span></span>|<span data-ttu-id="b582b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b582b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b582b-132">id</span><span class="sxs-lookup"><span data-stu-id="b582b-132">id</span></span>|<span data-ttu-id="b582b-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b582b-133">String</span></span>|<span data-ttu-id="b582b-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b582b-134">Key of the entity.</span></span> <span data-ttu-id="b582b-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b582b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b582b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b582b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b582b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b582b-137">DateTimeOffset</span></span>|<span data-ttu-id="b582b-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b582b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b582b-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b582b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b582b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b582b-140">roleScopeTagIds</span></span>|<span data-ttu-id="b582b-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b582b-141">String collection</span></span>|<span data-ttu-id="b582b-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b582b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b582b-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b582b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b582b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b582b-144">supportsScopeTags</span></span>|<span data-ttu-id="b582b-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="b582b-145">Boolean</span></span>|<span data-ttu-id="b582b-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b582b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b582b-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b582b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b582b-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b582b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b582b-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b582b-149">This property is read-only.</span></span> <span data-ttu-id="b582b-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b582b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b582b-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b582b-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b582b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b582b-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b582b-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="b582b-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b582b-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b582b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b582b-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b582b-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b582b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b582b-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b582b-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="b582b-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b582b-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b582b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b582b-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b582b-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b582b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b582b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b582b-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="b582b-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b582b-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b582b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b582b-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b582b-163">createdDateTime</span></span>|<span data-ttu-id="b582b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b582b-164">DateTimeOffset</span></span>|<span data-ttu-id="b582b-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b582b-165">DateTime the object was created.</span></span> <span data-ttu-id="b582b-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b582b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b582b-167">descrição</span><span class="sxs-lookup"><span data-stu-id="b582b-167">description</span></span>|<span data-ttu-id="b582b-168">String</span><span class="sxs-lookup"><span data-stu-id="b582b-168">String</span></span>|<span data-ttu-id="b582b-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b582b-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b582b-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b582b-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b582b-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b582b-171">displayName</span></span>|<span data-ttu-id="b582b-172">String</span><span class="sxs-lookup"><span data-stu-id="b582b-172">String</span></span>|<span data-ttu-id="b582b-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b582b-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b582b-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b582b-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b582b-175">versão</span><span class="sxs-lookup"><span data-stu-id="b582b-175">version</span></span>|<span data-ttu-id="b582b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b582b-176">Int32</span></span>|<span data-ttu-id="b582b-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b582b-177">Version of the device configuration.</span></span> <span data-ttu-id="b582b-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b582b-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b582b-179">NetworkName</span><span class="sxs-lookup"><span data-stu-id="b582b-179">networkName</span></span>|<span data-ttu-id="b582b-180">String</span><span class="sxs-lookup"><span data-stu-id="b582b-180">String</span></span>|<span data-ttu-id="b582b-181">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="b582b-181">Network Name</span></span>|
|<span data-ttu-id="b582b-182">SSID</span><span class="sxs-lookup"><span data-stu-id="b582b-182">ssid</span></span>|<span data-ttu-id="b582b-183">String</span><span class="sxs-lookup"><span data-stu-id="b582b-183">String</span></span>|<span data-ttu-id="b582b-184">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b582b-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="b582b-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="b582b-185">connectAutomatically</span></span>|<span data-ttu-id="b582b-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="b582b-186">Boolean</span></span>|<span data-ttu-id="b582b-187">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="b582b-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="b582b-188">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b582b-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="b582b-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="b582b-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="b582b-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="b582b-190">Boolean</span></span>|<span data-ttu-id="b582b-191">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b582b-191">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="b582b-192">à</span><span class="sxs-lookup"><span data-stu-id="b582b-192">wiFiSecurityType</span></span>|[<span data-ttu-id="b582b-193">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b582b-193">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="b582b-194">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="b582b-194">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="b582b-195">Os valores possíveis são: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="b582b-195">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="b582b-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="b582b-196">Response</span></span>
<span data-ttu-id="b582b-197">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b582b-197">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b582b-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b582b-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="b582b-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b582b-199">Request</span></span>
<span data-ttu-id="b582b-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b582b-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="b582b-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="b582b-201">Response</span></span>
<span data-ttu-id="b582b-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b582b-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





