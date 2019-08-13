---
title: Atualizar androidWorkProfileWiFiConfiguration
description: Atualiza as propriedades de um objeto androidWorkProfileWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 46fcab5a702a60aa93330508b0b5fad88760a2f0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36340461"
---
# <a name="update-androidworkprofilewificonfiguration"></a><span data-ttu-id="b4582-103">Atualizar androidWorkProfileWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="b4582-103">Update androidWorkProfileWiFiConfiguration</span></span>

> <span data-ttu-id="b4582-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b4582-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4582-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4582-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4582-106">Atualiza as propriedades de um objeto [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b4582-106">Update the properties of a [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4582-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b4582-107">Prerequisites</span></span>
<span data-ttu-id="b4582-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4582-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4582-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4582-110">Permission type</span></span>|<span data-ttu-id="b4582-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b4582-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4582-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4582-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b4582-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4582-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4582-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4582-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4582-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4582-115">Not supported.</span></span>|
|<span data-ttu-id="b4582-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4582-116">Application</span></span>|<span data-ttu-id="b4582-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4582-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4582-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4582-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b4582-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4582-119">Request headers</span></span>
|<span data-ttu-id="b4582-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4582-120">Header</span></span>|<span data-ttu-id="b4582-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b4582-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4582-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4582-122">Authorization</span></span>|<span data-ttu-id="b4582-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4582-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4582-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b4582-124">Accept</span></span>|<span data-ttu-id="b4582-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b4582-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4582-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4582-126">Request body</span></span>
<span data-ttu-id="b4582-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b4582-127">In the request body, supply a JSON representation for the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>

<span data-ttu-id="b4582-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4582-128">The following table shows the properties that are required when you create the [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span>

|<span data-ttu-id="b4582-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4582-129">Property</span></span>|<span data-ttu-id="b4582-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4582-130">Type</span></span>|<span data-ttu-id="b4582-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4582-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4582-132">id</span><span class="sxs-lookup"><span data-stu-id="b4582-132">id</span></span>|<span data-ttu-id="b4582-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4582-133">String</span></span>|<span data-ttu-id="b4582-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b4582-134">Key of the entity.</span></span> <span data-ttu-id="b4582-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4582-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4582-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4582-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b4582-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4582-137">DateTimeOffset</span></span>|<span data-ttu-id="b4582-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b4582-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b4582-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4582-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4582-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b4582-140">roleScopeTagIds</span></span>|<span data-ttu-id="b4582-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b4582-141">String collection</span></span>|<span data-ttu-id="b4582-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b4582-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b4582-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4582-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4582-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b4582-144">supportsScopeTags</span></span>|<span data-ttu-id="b4582-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="b4582-145">Boolean</span></span>|<span data-ttu-id="b4582-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b4582-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b4582-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b4582-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b4582-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b4582-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b4582-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b4582-149">This property is read-only.</span></span> <span data-ttu-id="b4582-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4582-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4582-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b4582-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b4582-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b4582-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b4582-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="b4582-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b4582-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4582-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4582-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b4582-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b4582-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b4582-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b4582-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="b4582-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b4582-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4582-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4582-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b4582-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b4582-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b4582-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b4582-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="b4582-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b4582-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4582-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4582-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4582-163">createdDateTime</span></span>|<span data-ttu-id="b4582-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4582-164">DateTimeOffset</span></span>|<span data-ttu-id="b4582-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b4582-165">DateTime the object was created.</span></span> <span data-ttu-id="b4582-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4582-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4582-167">descrição</span><span class="sxs-lookup"><span data-stu-id="b4582-167">description</span></span>|<span data-ttu-id="b4582-168">String</span><span class="sxs-lookup"><span data-stu-id="b4582-168">String</span></span>|<span data-ttu-id="b4582-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4582-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b4582-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4582-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4582-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b4582-171">displayName</span></span>|<span data-ttu-id="b4582-172">String</span><span class="sxs-lookup"><span data-stu-id="b4582-172">String</span></span>|<span data-ttu-id="b4582-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4582-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b4582-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4582-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4582-175">versão</span><span class="sxs-lookup"><span data-stu-id="b4582-175">version</span></span>|<span data-ttu-id="b4582-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b4582-176">Int32</span></span>|<span data-ttu-id="b4582-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b4582-177">Version of the device configuration.</span></span> <span data-ttu-id="b4582-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4582-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4582-179">NetworkName</span><span class="sxs-lookup"><span data-stu-id="b4582-179">networkName</span></span>|<span data-ttu-id="b4582-180">String</span><span class="sxs-lookup"><span data-stu-id="b4582-180">String</span></span>|<span data-ttu-id="b4582-181">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="b4582-181">Network Name</span></span>|
|<span data-ttu-id="b4582-182">SSID</span><span class="sxs-lookup"><span data-stu-id="b4582-182">ssid</span></span>|<span data-ttu-id="b4582-183">String</span><span class="sxs-lookup"><span data-stu-id="b4582-183">String</span></span>|<span data-ttu-id="b4582-184">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b4582-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="b4582-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="b4582-185">connectAutomatically</span></span>|<span data-ttu-id="b4582-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="b4582-186">Boolean</span></span>|<span data-ttu-id="b4582-187">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="b4582-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="b4582-188">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b4582-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="b4582-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="b4582-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="b4582-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="b4582-190">Boolean</span></span>|<span data-ttu-id="b4582-191">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b4582-191">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="b4582-192">à</span><span class="sxs-lookup"><span data-stu-id="b4582-192">wiFiSecurityType</span></span>|[<span data-ttu-id="b4582-193">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b4582-193">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="b4582-194">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="b4582-194">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="b4582-195">Os valores possíveis são: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="b4582-195">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="b4582-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4582-196">Response</span></span>
<span data-ttu-id="b4582-197">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4582-197">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4582-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4582-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4582-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4582-199">Request</span></span>
<span data-ttu-id="b4582-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4582-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b4582-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4582-201">Response</span></span>
<span data-ttu-id="b4582-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4582-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






