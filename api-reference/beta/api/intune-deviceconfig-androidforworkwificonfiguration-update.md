---
title: Atualizar androidForWorkWiFiConfiguration
description: Atualize as propriedades de um objeto androidForWorkWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a8f45dd609964ae1800d0a1d952a584ee2e5e154
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130228"
---
# <a name="update-androidforworkwificonfiguration"></a><span data-ttu-id="f2ebf-103">Atualizar androidForWorkWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2ebf-103">Update androidForWorkWiFiConfiguration</span></span>

<span data-ttu-id="f2ebf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2ebf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2ebf-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2ebf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2ebf-107">Atualize as propriedades de um [objeto androidForWorkWiFiConfiguration.](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2ebf-107">Update the properties of a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2ebf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2ebf-108">Prerequisites</span></span>
<span data-ttu-id="f2ebf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2ebf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2ebf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2ebf-111">Permission type</span></span>|<span data-ttu-id="f2ebf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f2ebf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2ebf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2ebf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2ebf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2ebf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f2ebf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2ebf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2ebf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-116">Not supported.</span></span>|
|<span data-ttu-id="f2ebf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2ebf-117">Application</span></span>|<span data-ttu-id="f2ebf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2ebf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2ebf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2ebf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f2ebf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2ebf-120">Request headers</span></span>
|<span data-ttu-id="f2ebf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2ebf-121">Header</span></span>|<span data-ttu-id="f2ebf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f2ebf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2ebf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2ebf-123">Authorization</span></span>|<span data-ttu-id="f2ebf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2ebf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2ebf-125">Accept</span></span>|<span data-ttu-id="f2ebf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2ebf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2ebf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2ebf-127">Request body</span></span>
<span data-ttu-id="f2ebf-128">No corpo da solicitação, fornece uma representação JSON para o [objeto androidForWorkWiFiConfiguration.](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2ebf-128">In the request body, supply a JSON representation for the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

<span data-ttu-id="f2ebf-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2ebf-129">The following table shows the properties that are required when you create the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span>

|<span data-ttu-id="f2ebf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2ebf-130">Property</span></span>|<span data-ttu-id="f2ebf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2ebf-131">Type</span></span>|<span data-ttu-id="f2ebf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2ebf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2ebf-133">id</span><span class="sxs-lookup"><span data-stu-id="f2ebf-133">id</span></span>|<span data-ttu-id="f2ebf-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2ebf-134">String</span></span>|<span data-ttu-id="f2ebf-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-135">Key of the entity.</span></span> <span data-ttu-id="f2ebf-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2ebf-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ebf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2ebf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f2ebf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2ebf-138">DateTimeOffset</span></span>|<span data-ttu-id="f2ebf-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f2ebf-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2ebf-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ebf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f2ebf-141">roleScopeTagIds</span></span>|<span data-ttu-id="f2ebf-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2ebf-142">String collection</span></span>|<span data-ttu-id="f2ebf-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f2ebf-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2ebf-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ebf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f2ebf-145">supportsScopeTags</span></span>|<span data-ttu-id="f2ebf-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="f2ebf-146">Boolean</span></span>|<span data-ttu-id="f2ebf-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f2ebf-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f2ebf-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f2ebf-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-150">This property is read-only.</span></span> <span data-ttu-id="f2ebf-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2ebf-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ebf-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f2ebf-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f2ebf-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f2ebf-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f2ebf-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f2ebf-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2ebf-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ebf-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f2ebf-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f2ebf-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f2ebf-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f2ebf-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f2ebf-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2ebf-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ebf-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f2ebf-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f2ebf-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f2ebf-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f2ebf-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f2ebf-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2ebf-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ebf-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2ebf-164">createdDateTime</span></span>|<span data-ttu-id="f2ebf-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2ebf-165">DateTimeOffset</span></span>|<span data-ttu-id="f2ebf-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-166">DateTime the object was created.</span></span> <span data-ttu-id="f2ebf-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2ebf-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ebf-168">descrição</span><span class="sxs-lookup"><span data-stu-id="f2ebf-168">description</span></span>|<span data-ttu-id="f2ebf-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2ebf-169">String</span></span>|<span data-ttu-id="f2ebf-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f2ebf-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2ebf-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ebf-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f2ebf-172">displayName</span></span>|<span data-ttu-id="f2ebf-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2ebf-173">String</span></span>|<span data-ttu-id="f2ebf-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f2ebf-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2ebf-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ebf-176">versão</span><span class="sxs-lookup"><span data-stu-id="f2ebf-176">version</span></span>|<span data-ttu-id="f2ebf-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f2ebf-177">Int32</span></span>|<span data-ttu-id="f2ebf-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-178">Version of the device configuration.</span></span> <span data-ttu-id="f2ebf-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2ebf-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2ebf-180">networkName</span><span class="sxs-lookup"><span data-stu-id="f2ebf-180">networkName</span></span>|<span data-ttu-id="f2ebf-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2ebf-181">String</span></span>|<span data-ttu-id="f2ebf-182">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="f2ebf-182">Network Name</span></span>|
|<span data-ttu-id="f2ebf-183">ssid</span><span class="sxs-lookup"><span data-stu-id="f2ebf-183">ssid</span></span>|<span data-ttu-id="f2ebf-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2ebf-184">String</span></span>|<span data-ttu-id="f2ebf-185">Esse é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="f2ebf-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="f2ebf-186">connectAutomatically</span></span>|<span data-ttu-id="f2ebf-187">Booleano</span><span class="sxs-lookup"><span data-stu-id="f2ebf-187">Boolean</span></span>|<span data-ttu-id="f2ebf-188">Conecte-se automaticamente quando essa rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="f2ebf-189">Definir isso como true ignorará o prompt do usuário e conectará automaticamente o dispositivo Wi-Fi rede.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="f2ebf-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="f2ebf-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="f2ebf-191">Booleano</span><span class="sxs-lookup"><span data-stu-id="f2ebf-191">Boolean</span></span>|<span data-ttu-id="f2ebf-192">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="f2ebf-193">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="f2ebf-193">wiFiSecurityType</span></span>|[<span data-ttu-id="f2ebf-194">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="f2ebf-194">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="f2ebf-195">Indica se Wi-Fi ponto de extremidade usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="f2ebf-196">Os valores possíveis são: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-196">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="f2ebf-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2ebf-197">Response</span></span>
<span data-ttu-id="f2ebf-198">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-198">If successful, this method returns a `200 OK` response code and an updated [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2ebf-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2ebf-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2ebf-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2ebf-200">Request</span></span>
<span data-ttu-id="f2ebf-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="f2ebf-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2ebf-202">Response</span></span>
<span data-ttu-id="f2ebf-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2ebf-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




