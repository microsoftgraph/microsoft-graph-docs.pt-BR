---
title: Criar androidDeviceOwnerWiFiConfiguration
description: Criar um novo objeto androidDeviceOwnerWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73c0ec47f811270479cb4b86df169a3cd867ff7f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958092"
---
# <a name="create-androiddeviceownerwificonfiguration"></a><span data-ttu-id="ac7d7-103">Criar androidDeviceOwnerWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="ac7d7-103">Create androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="ac7d7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac7d7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac7d7-106">Criar um novo objeto [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ac7d7-106">Create a new [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac7d7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ac7d7-107">Prerequisites</span></span>
<span data-ttu-id="ac7d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac7d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac7d7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac7d7-110">Permission type</span></span>|<span data-ttu-id="ac7d7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ac7d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac7d7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac7d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ac7d7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac7d7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ac7d7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac7d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac7d7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-115">Not supported.</span></span>|
|<span data-ttu-id="ac7d7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac7d7-116">Application</span></span>|<span data-ttu-id="ac7d7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac7d7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac7d7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ac7d7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac7d7-119">Request headers</span></span>
|<span data-ttu-id="ac7d7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac7d7-120">Header</span></span>|<span data-ttu-id="ac7d7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ac7d7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac7d7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac7d7-122">Authorization</span></span>|<span data-ttu-id="ac7d7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac7d7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ac7d7-124">Accept</span></span>|<span data-ttu-id="ac7d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ac7d7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac7d7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac7d7-126">Request body</span></span>
<span data-ttu-id="ac7d7-127">No corpo da solicitação, forneça uma representação JSON do objeto androidDeviceOwnerWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-127">In the request body, supply a JSON representation for the androidDeviceOwnerWiFiConfiguration object.</span></span>

<span data-ttu-id="ac7d7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-128">The following table shows the properties that are required when you create the androidDeviceOwnerWiFiConfiguration.</span></span>

|<span data-ttu-id="ac7d7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac7d7-129">Property</span></span>|<span data-ttu-id="ac7d7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac7d7-130">Type</span></span>|<span data-ttu-id="ac7d7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac7d7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac7d7-132">id</span><span class="sxs-lookup"><span data-stu-id="ac7d7-132">id</span></span>|<span data-ttu-id="ac7d7-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac7d7-133">String</span></span>|<span data-ttu-id="ac7d7-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-134">Key of the entity.</span></span> <span data-ttu-id="ac7d7-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac7d7-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac7d7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac7d7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ac7d7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac7d7-137">DateTimeOffset</span></span>|<span data-ttu-id="ac7d7-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ac7d7-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac7d7-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac7d7-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ac7d7-140">roleScopeTagIds</span></span>|<span data-ttu-id="ac7d7-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac7d7-141">String collection</span></span>|<span data-ttu-id="ac7d7-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ac7d7-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac7d7-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac7d7-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ac7d7-144">supportsScopeTags</span></span>|<span data-ttu-id="ac7d7-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac7d7-145">Boolean</span></span>|<span data-ttu-id="ac7d7-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ac7d7-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ac7d7-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ac7d7-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-149">This property is read-only.</span></span> <span data-ttu-id="ac7d7-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac7d7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac7d7-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ac7d7-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ac7d7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ac7d7-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ac7d7-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ac7d7-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac7d7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac7d7-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ac7d7-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ac7d7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ac7d7-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ac7d7-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ac7d7-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac7d7-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac7d7-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ac7d7-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ac7d7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ac7d7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ac7d7-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ac7d7-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac7d7-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac7d7-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac7d7-163">createdDateTime</span></span>|<span data-ttu-id="ac7d7-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac7d7-164">DateTimeOffset</span></span>|<span data-ttu-id="ac7d7-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-165">DateTime the object was created.</span></span> <span data-ttu-id="ac7d7-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac7d7-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac7d7-167">descrição</span><span class="sxs-lookup"><span data-stu-id="ac7d7-167">description</span></span>|<span data-ttu-id="ac7d7-168">String</span><span class="sxs-lookup"><span data-stu-id="ac7d7-168">String</span></span>|<span data-ttu-id="ac7d7-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ac7d7-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac7d7-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac7d7-171">displayName</span><span class="sxs-lookup"><span data-stu-id="ac7d7-171">displayName</span></span>|<span data-ttu-id="ac7d7-172">String</span><span class="sxs-lookup"><span data-stu-id="ac7d7-172">String</span></span>|<span data-ttu-id="ac7d7-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ac7d7-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac7d7-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac7d7-175">versão</span><span class="sxs-lookup"><span data-stu-id="ac7d7-175">version</span></span>|<span data-ttu-id="ac7d7-176">Int32</span><span class="sxs-lookup"><span data-stu-id="ac7d7-176">Int32</span></span>|<span data-ttu-id="ac7d7-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-177">Version of the device configuration.</span></span> <span data-ttu-id="ac7d7-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac7d7-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ac7d7-179">NetworkName</span><span class="sxs-lookup"><span data-stu-id="ac7d7-179">networkName</span></span>|<span data-ttu-id="ac7d7-180">String</span><span class="sxs-lookup"><span data-stu-id="ac7d7-180">String</span></span>|<span data-ttu-id="ac7d7-181">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="ac7d7-181">Network Name</span></span>|
|<span data-ttu-id="ac7d7-182">SSID</span><span class="sxs-lookup"><span data-stu-id="ac7d7-182">ssid</span></span>|<span data-ttu-id="ac7d7-183">String</span><span class="sxs-lookup"><span data-stu-id="ac7d7-183">String</span></span>|<span data-ttu-id="ac7d7-184">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="ac7d7-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="ac7d7-185">connectAutomatically</span></span>|<span data-ttu-id="ac7d7-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac7d7-186">Boolean</span></span>|<span data-ttu-id="ac7d7-187">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="ac7d7-188">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="ac7d7-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="ac7d7-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="ac7d7-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac7d7-190">Boolean</span></span>|<span data-ttu-id="ac7d7-191">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-191">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="ac7d7-192">à</span><span class="sxs-lookup"><span data-stu-id="ac7d7-192">wiFiSecurityType</span></span>|[<span data-ttu-id="ac7d7-193">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="ac7d7-193">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="ac7d7-194">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-194">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="ac7d7-195">Os valores possíveis são: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-195">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="ac7d7-196">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="ac7d7-196">preSharedKey</span></span>|<span data-ttu-id="ac7d7-197">String</span><span class="sxs-lookup"><span data-stu-id="ac7d7-197">String</span></span>|<span data-ttu-id="ac7d7-198">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-198">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="ac7d7-199">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="ac7d7-199">preSharedKeyIsSet</span></span>|<span data-ttu-id="ac7d7-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac7d7-200">Boolean</span></span>|<span data-ttu-id="ac7d7-201">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-201">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="ac7d7-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac7d7-202">Response</span></span>
<span data-ttu-id="ac7d7-203">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-203">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac7d7-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac7d7-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac7d7-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac7d7-205">Request</span></span>
<span data-ttu-id="ac7d7-206">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1282

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
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
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true
}
```

### <a name="response"></a><span data-ttu-id="ac7d7-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac7d7-207">Response</span></span>
<span data-ttu-id="ac7d7-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac7d7-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1454

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "id": "8d25beba-beba-8d25-babe-258dbabe258d",
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
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true
}
```





