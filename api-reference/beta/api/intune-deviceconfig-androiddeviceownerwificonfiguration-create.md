---
title: Criar androidDeviceOwnerWiFiConfiguration
description: Crie um novo objeto androidDeviceOwnerWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cbf653050d19110d9485cd09f9c476d9a906f823
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138481"
---
# <a name="create-androiddeviceownerwificonfiguration"></a><span data-ttu-id="686a8-103">Criar androidDeviceOwnerWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="686a8-103">Create androidDeviceOwnerWiFiConfiguration</span></span>

<span data-ttu-id="686a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="686a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="686a8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="686a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="686a8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="686a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="686a8-107">Crie um novo [objeto androidDeviceOwnerWiFiConfiguration.](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="686a8-107">Create a new [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="686a8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="686a8-108">Prerequisites</span></span>
<span data-ttu-id="686a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="686a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="686a8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="686a8-111">Permission type</span></span>|<span data-ttu-id="686a8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="686a8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="686a8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="686a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="686a8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="686a8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="686a8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="686a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="686a8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="686a8-116">Not supported.</span></span>|
|<span data-ttu-id="686a8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="686a8-117">Application</span></span>|<span data-ttu-id="686a8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="686a8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="686a8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="686a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="686a8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="686a8-120">Request headers</span></span>
|<span data-ttu-id="686a8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="686a8-121">Header</span></span>|<span data-ttu-id="686a8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="686a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="686a8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="686a8-123">Authorization</span></span>|<span data-ttu-id="686a8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="686a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="686a8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="686a8-125">Accept</span></span>|<span data-ttu-id="686a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="686a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="686a8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="686a8-127">Request body</span></span>
<span data-ttu-id="686a8-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidDeviceOwnerWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="686a8-128">In the request body, supply a JSON representation for the androidDeviceOwnerWiFiConfiguration object.</span></span>

<span data-ttu-id="686a8-129">A tabela a seguir mostra as propriedades necessárias ao criar androidDeviceOwnerWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="686a8-129">The following table shows the properties that are required when you create the androidDeviceOwnerWiFiConfiguration.</span></span>

|<span data-ttu-id="686a8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="686a8-130">Property</span></span>|<span data-ttu-id="686a8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="686a8-131">Type</span></span>|<span data-ttu-id="686a8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="686a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="686a8-133">id</span><span class="sxs-lookup"><span data-stu-id="686a8-133">id</span></span>|<span data-ttu-id="686a8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="686a8-134">String</span></span>|<span data-ttu-id="686a8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="686a8-135">Key of the entity.</span></span> <span data-ttu-id="686a8-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="686a8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="686a8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="686a8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="686a8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="686a8-138">DateTimeOffset</span></span>|<span data-ttu-id="686a8-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="686a8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="686a8-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="686a8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="686a8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="686a8-141">roleScopeTagIds</span></span>|<span data-ttu-id="686a8-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="686a8-142">String collection</span></span>|<span data-ttu-id="686a8-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="686a8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="686a8-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="686a8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="686a8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="686a8-145">supportsScopeTags</span></span>|<span data-ttu-id="686a8-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="686a8-146">Boolean</span></span>|<span data-ttu-id="686a8-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="686a8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="686a8-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="686a8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="686a8-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="686a8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="686a8-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="686a8-150">This property is read-only.</span></span> <span data-ttu-id="686a8-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="686a8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="686a8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="686a8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="686a8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="686a8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="686a8-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="686a8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="686a8-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="686a8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="686a8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="686a8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="686a8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="686a8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="686a8-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="686a8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="686a8-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="686a8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="686a8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="686a8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="686a8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="686a8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="686a8-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="686a8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="686a8-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="686a8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="686a8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="686a8-164">createdDateTime</span></span>|<span data-ttu-id="686a8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="686a8-165">DateTimeOffset</span></span>|<span data-ttu-id="686a8-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="686a8-166">DateTime the object was created.</span></span> <span data-ttu-id="686a8-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="686a8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="686a8-168">descrição</span><span class="sxs-lookup"><span data-stu-id="686a8-168">description</span></span>|<span data-ttu-id="686a8-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="686a8-169">String</span></span>|<span data-ttu-id="686a8-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="686a8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="686a8-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="686a8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="686a8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="686a8-172">displayName</span></span>|<span data-ttu-id="686a8-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="686a8-173">String</span></span>|<span data-ttu-id="686a8-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="686a8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="686a8-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="686a8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="686a8-176">versão</span><span class="sxs-lookup"><span data-stu-id="686a8-176">version</span></span>|<span data-ttu-id="686a8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="686a8-177">Int32</span></span>|<span data-ttu-id="686a8-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="686a8-178">Version of the device configuration.</span></span> <span data-ttu-id="686a8-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="686a8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="686a8-180">networkName</span><span class="sxs-lookup"><span data-stu-id="686a8-180">networkName</span></span>|<span data-ttu-id="686a8-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="686a8-181">String</span></span>|<span data-ttu-id="686a8-182">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="686a8-182">Network Name</span></span>|
|<span data-ttu-id="686a8-183">ssid</span><span class="sxs-lookup"><span data-stu-id="686a8-183">ssid</span></span>|<span data-ttu-id="686a8-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="686a8-184">String</span></span>|<span data-ttu-id="686a8-185">Esse é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="686a8-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="686a8-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="686a8-186">connectAutomatically</span></span>|<span data-ttu-id="686a8-187">Booleano</span><span class="sxs-lookup"><span data-stu-id="686a8-187">Boolean</span></span>|<span data-ttu-id="686a8-188">Conecte-se automaticamente quando essa rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="686a8-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="686a8-189">Definir isso como true ignorará o prompt do usuário e conectará automaticamente o dispositivo Wi-Fi rede.</span><span class="sxs-lookup"><span data-stu-id="686a8-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="686a8-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="686a8-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="686a8-191">Booleano</span><span class="sxs-lookup"><span data-stu-id="686a8-191">Boolean</span></span>|<span data-ttu-id="686a8-192">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="686a8-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="686a8-193">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="686a8-193">wiFiSecurityType</span></span>|[<span data-ttu-id="686a8-194">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="686a8-194">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="686a8-195">Indica se Wi-Fi ponto de extremidade usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="686a8-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="686a8-196">Os valores possíveis são: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="686a8-196">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="686a8-197">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="686a8-197">preSharedKey</span></span>|<span data-ttu-id="686a8-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="686a8-198">String</span></span>|<span data-ttu-id="686a8-199">Esta é a chave pré-compartilhada para a rede WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="686a8-199">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="686a8-200">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="686a8-200">preSharedKeyIsSet</span></span>|<span data-ttu-id="686a8-201">Booleano</span><span class="sxs-lookup"><span data-stu-id="686a8-201">Boolean</span></span>|<span data-ttu-id="686a8-202">Esta é a chave pré-compartilhada para a rede WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="686a8-202">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="686a8-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="686a8-203">Response</span></span>
<span data-ttu-id="686a8-204">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="686a8-204">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="686a8-205">Exemplo</span><span class="sxs-lookup"><span data-stu-id="686a8-205">Example</span></span>

### <a name="request"></a><span data-ttu-id="686a8-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="686a8-206">Request</span></span>
<span data-ttu-id="686a8-207">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="686a8-207">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="686a8-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="686a8-208">Response</span></span>
<span data-ttu-id="686a8-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="686a8-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




