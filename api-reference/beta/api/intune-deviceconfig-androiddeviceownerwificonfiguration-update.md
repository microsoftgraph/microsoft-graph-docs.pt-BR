---
title: Atualizar androidDeviceOwnerWiFiConfiguration
description: Atualiza as propriedades de um objeto androidDeviceOwnerWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dae7ef0330d94ccdc81c017907edc14cd65df845
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996014"
---
# <a name="update-androiddeviceownerwificonfiguration"></a><span data-ttu-id="92db7-103">Atualizar androidDeviceOwnerWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="92db7-103">Update androidDeviceOwnerWiFiConfiguration</span></span>

<span data-ttu-id="92db7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92db7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92db7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92db7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92db7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92db7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92db7-107">Atualiza as propriedades de um objeto [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="92db7-107">Update the properties of a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92db7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92db7-108">Prerequisites</span></span>
<span data-ttu-id="92db7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92db7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92db7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92db7-111">Permission type</span></span>|<span data-ttu-id="92db7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92db7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92db7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92db7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92db7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92db7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92db7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92db7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92db7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92db7-116">Not supported.</span></span>|
|<span data-ttu-id="92db7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92db7-117">Application</span></span>|<span data-ttu-id="92db7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92db7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92db7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92db7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="92db7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92db7-120">Request headers</span></span>
|<span data-ttu-id="92db7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92db7-121">Header</span></span>|<span data-ttu-id="92db7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="92db7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92db7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="92db7-123">Authorization</span></span>|<span data-ttu-id="92db7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92db7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92db7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92db7-125">Accept</span></span>|<span data-ttu-id="92db7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92db7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92db7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92db7-127">Request body</span></span>
<span data-ttu-id="92db7-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="92db7-128">In the request body, supply a JSON representation for the [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

<span data-ttu-id="92db7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="92db7-129">The following table shows the properties that are required when you create the [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span></span>

|<span data-ttu-id="92db7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92db7-130">Property</span></span>|<span data-ttu-id="92db7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="92db7-131">Type</span></span>|<span data-ttu-id="92db7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="92db7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92db7-133">id</span><span class="sxs-lookup"><span data-stu-id="92db7-133">id</span></span>|<span data-ttu-id="92db7-134">String</span><span class="sxs-lookup"><span data-stu-id="92db7-134">String</span></span>|<span data-ttu-id="92db7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="92db7-135">Key of the entity.</span></span> <span data-ttu-id="92db7-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92db7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92db7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92db7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="92db7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92db7-138">DateTimeOffset</span></span>|<span data-ttu-id="92db7-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="92db7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="92db7-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92db7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92db7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="92db7-141">roleScopeTagIds</span></span>|<span data-ttu-id="92db7-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="92db7-142">String collection</span></span>|<span data-ttu-id="92db7-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="92db7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="92db7-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92db7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92db7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="92db7-145">supportsScopeTags</span></span>|<span data-ttu-id="92db7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="92db7-146">Boolean</span></span>|<span data-ttu-id="92db7-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="92db7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="92db7-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="92db7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="92db7-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="92db7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="92db7-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="92db7-150">This property is read-only.</span></span> <span data-ttu-id="92db7-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92db7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92db7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="92db7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="92db7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="92db7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="92db7-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="92db7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="92db7-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92db7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92db7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="92db7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="92db7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="92db7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="92db7-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="92db7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="92db7-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92db7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92db7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="92db7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="92db7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="92db7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="92db7-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="92db7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="92db7-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92db7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92db7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92db7-164">createdDateTime</span></span>|<span data-ttu-id="92db7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92db7-165">DateTimeOffset</span></span>|<span data-ttu-id="92db7-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="92db7-166">DateTime the object was created.</span></span> <span data-ttu-id="92db7-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92db7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92db7-168">description</span><span class="sxs-lookup"><span data-stu-id="92db7-168">description</span></span>|<span data-ttu-id="92db7-169">String</span><span class="sxs-lookup"><span data-stu-id="92db7-169">String</span></span>|<span data-ttu-id="92db7-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92db7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="92db7-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92db7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92db7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="92db7-172">displayName</span></span>|<span data-ttu-id="92db7-173">String</span><span class="sxs-lookup"><span data-stu-id="92db7-173">String</span></span>|<span data-ttu-id="92db7-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92db7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="92db7-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92db7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92db7-176">versão</span><span class="sxs-lookup"><span data-stu-id="92db7-176">version</span></span>|<span data-ttu-id="92db7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="92db7-177">Int32</span></span>|<span data-ttu-id="92db7-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="92db7-178">Version of the device configuration.</span></span> <span data-ttu-id="92db7-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="92db7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="92db7-180">NetworkName</span><span class="sxs-lookup"><span data-stu-id="92db7-180">networkName</span></span>|<span data-ttu-id="92db7-181">String</span><span class="sxs-lookup"><span data-stu-id="92db7-181">String</span></span>|<span data-ttu-id="92db7-182">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="92db7-182">Network Name</span></span>|
|<span data-ttu-id="92db7-183">SSID</span><span class="sxs-lookup"><span data-stu-id="92db7-183">ssid</span></span>|<span data-ttu-id="92db7-184">String</span><span class="sxs-lookup"><span data-stu-id="92db7-184">String</span></span>|<span data-ttu-id="92db7-185">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="92db7-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="92db7-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="92db7-186">connectAutomatically</span></span>|<span data-ttu-id="92db7-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="92db7-187">Boolean</span></span>|<span data-ttu-id="92db7-188">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="92db7-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="92db7-189">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="92db7-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="92db7-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="92db7-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="92db7-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="92db7-191">Boolean</span></span>|<span data-ttu-id="92db7-192">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="92db7-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="92db7-193">à</span><span class="sxs-lookup"><span data-stu-id="92db7-193">wiFiSecurityType</span></span>|[<span data-ttu-id="92db7-194">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="92db7-194">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="92db7-195">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="92db7-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="92db7-196">Os valores possíveis são: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="92db7-196">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="92db7-197">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="92db7-197">preSharedKey</span></span>|<span data-ttu-id="92db7-198">String</span><span class="sxs-lookup"><span data-stu-id="92db7-198">String</span></span>|<span data-ttu-id="92db7-199">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="92db7-199">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="92db7-200">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="92db7-200">preSharedKeyIsSet</span></span>|<span data-ttu-id="92db7-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="92db7-201">Boolean</span></span>|<span data-ttu-id="92db7-202">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="92db7-202">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="92db7-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="92db7-203">Response</span></span>
<span data-ttu-id="92db7-204">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92db7-204">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92db7-205">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92db7-205">Example</span></span>

### <a name="request"></a><span data-ttu-id="92db7-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92db7-206">Request</span></span>
<span data-ttu-id="92db7-207">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92db7-207">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="92db7-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="92db7-208">Response</span></span>
<span data-ttu-id="92db7-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92db7-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






