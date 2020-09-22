---
title: Criar androidForWorkWiFiConfiguration
description: Criar um novo objeto androidForWorkWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 788540e97d9310b4a5cb4cb1419a854fc9f31f9c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066184"
---
# <a name="create-androidforworkwificonfiguration"></a><span data-ttu-id="f0f2e-103">Criar androidForWorkWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="f0f2e-103">Create androidForWorkWiFiConfiguration</span></span>

<span data-ttu-id="f0f2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0f2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0f2e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0f2e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0f2e-107">Criar um novo objeto [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f0f2e-107">Create a new [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0f2e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f0f2e-108">Prerequisites</span></span>
<span data-ttu-id="f0f2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0f2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0f2e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0f2e-111">Permission type</span></span>|<span data-ttu-id="f0f2e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f0f2e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0f2e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0f2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0f2e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0f2e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0f2e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0f2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0f2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-116">Not supported.</span></span>|
|<span data-ttu-id="f0f2e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0f2e-117">Application</span></span>|<span data-ttu-id="f0f2e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0f2e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0f2e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0f2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f0f2e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0f2e-120">Request headers</span></span>
|<span data-ttu-id="f0f2e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f0f2e-121">Header</span></span>|<span data-ttu-id="f0f2e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f0f2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0f2e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0f2e-123">Authorization</span></span>|<span data-ttu-id="f0f2e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0f2e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f0f2e-125">Accept</span></span>|<span data-ttu-id="f0f2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0f2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0f2e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0f2e-127">Request body</span></span>
<span data-ttu-id="f0f2e-128">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-128">In the request body, supply a JSON representation for the androidForWorkWiFiConfiguration object.</span></span>

<span data-ttu-id="f0f2e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-129">The following table shows the properties that are required when you create the androidForWorkWiFiConfiguration.</span></span>

|<span data-ttu-id="f0f2e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0f2e-130">Property</span></span>|<span data-ttu-id="f0f2e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0f2e-131">Type</span></span>|<span data-ttu-id="f0f2e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0f2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0f2e-133">id</span><span class="sxs-lookup"><span data-stu-id="f0f2e-133">id</span></span>|<span data-ttu-id="f0f2e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0f2e-134">String</span></span>|<span data-ttu-id="f0f2e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-135">Key of the entity.</span></span> <span data-ttu-id="f0f2e-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0f2e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f2e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0f2e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f0f2e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0f2e-138">DateTimeOffset</span></span>|<span data-ttu-id="f0f2e-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f0f2e-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0f2e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f2e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f0f2e-141">roleScopeTagIds</span></span>|<span data-ttu-id="f0f2e-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0f2e-142">String collection</span></span>|<span data-ttu-id="f0f2e-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f0f2e-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0f2e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f2e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f0f2e-145">supportsScopeTags</span></span>|<span data-ttu-id="f0f2e-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0f2e-146">Boolean</span></span>|<span data-ttu-id="f0f2e-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f0f2e-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f0f2e-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f0f2e-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-150">This property is read-only.</span></span> <span data-ttu-id="f0f2e-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0f2e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f2e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f0f2e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f0f2e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f0f2e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f0f2e-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f0f2e-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0f2e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f2e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f0f2e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f0f2e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f0f2e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f0f2e-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f0f2e-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0f2e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f2e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f0f2e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f0f2e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f0f2e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f0f2e-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f0f2e-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0f2e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f2e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0f2e-164">createdDateTime</span></span>|<span data-ttu-id="f0f2e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0f2e-165">DateTimeOffset</span></span>|<span data-ttu-id="f0f2e-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-166">DateTime the object was created.</span></span> <span data-ttu-id="f0f2e-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0f2e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f2e-168">description</span><span class="sxs-lookup"><span data-stu-id="f0f2e-168">description</span></span>|<span data-ttu-id="f0f2e-169">String</span><span class="sxs-lookup"><span data-stu-id="f0f2e-169">String</span></span>|<span data-ttu-id="f0f2e-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f0f2e-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0f2e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f2e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f0f2e-172">displayName</span></span>|<span data-ttu-id="f0f2e-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0f2e-173">String</span></span>|<span data-ttu-id="f0f2e-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f0f2e-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0f2e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f2e-176">versão</span><span class="sxs-lookup"><span data-stu-id="f0f2e-176">version</span></span>|<span data-ttu-id="f0f2e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f0f2e-177">Int32</span></span>|<span data-ttu-id="f0f2e-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-178">Version of the device configuration.</span></span> <span data-ttu-id="f0f2e-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0f2e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0f2e-180">NetworkName</span><span class="sxs-lookup"><span data-stu-id="f0f2e-180">networkName</span></span>|<span data-ttu-id="f0f2e-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0f2e-181">String</span></span>|<span data-ttu-id="f0f2e-182">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="f0f2e-182">Network Name</span></span>|
|<span data-ttu-id="f0f2e-183">SSID</span><span class="sxs-lookup"><span data-stu-id="f0f2e-183">ssid</span></span>|<span data-ttu-id="f0f2e-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0f2e-184">String</span></span>|<span data-ttu-id="f0f2e-185">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="f0f2e-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="f0f2e-186">connectAutomatically</span></span>|<span data-ttu-id="f0f2e-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0f2e-187">Boolean</span></span>|<span data-ttu-id="f0f2e-188">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="f0f2e-189">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="f0f2e-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="f0f2e-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="f0f2e-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0f2e-191">Boolean</span></span>|<span data-ttu-id="f0f2e-192">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="f0f2e-193">à</span><span class="sxs-lookup"><span data-stu-id="f0f2e-193">wiFiSecurityType</span></span>|[<span data-ttu-id="f0f2e-194">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="f0f2e-194">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="f0f2e-195">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="f0f2e-196">Os valores possíveis são: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-196">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="f0f2e-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0f2e-197">Response</span></span>
<span data-ttu-id="f0f2e-198">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-198">If successful, this method returns a `201 Created` response code and a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0f2e-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0f2e-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0f2e-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0f2e-200">Request</span></span>
<span data-ttu-id="f0f2e-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f0f2e-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0f2e-202">Response</span></span>
<span data-ttu-id="f0f2e-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0f2e-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






