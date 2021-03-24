---
title: Atualizar androidWiFiConfiguration
description: Atualize as propriedades de um objeto androidWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1592961ec01233edcf092f68eb3881dfcc8b193a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131789"
---
# <a name="update-androidwificonfiguration"></a><span data-ttu-id="f87a2-103">Atualizar androidWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="f87a2-103">Update androidWiFiConfiguration</span></span>

<span data-ttu-id="f87a2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f87a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f87a2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f87a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f87a2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f87a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f87a2-107">Atualize as propriedades de um [objeto androidWiFiConfiguration.](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f87a2-107">Update the properties of a [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f87a2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f87a2-108">Prerequisites</span></span>
<span data-ttu-id="f87a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f87a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f87a2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f87a2-111">Permission type</span></span>|<span data-ttu-id="f87a2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f87a2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f87a2-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f87a2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f87a2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f87a2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f87a2-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f87a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f87a2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f87a2-116">Not supported.</span></span>|
|<span data-ttu-id="f87a2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f87a2-117">Application</span></span>|<span data-ttu-id="f87a2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f87a2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f87a2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f87a2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f87a2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f87a2-120">Request headers</span></span>
|<span data-ttu-id="f87a2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f87a2-121">Header</span></span>|<span data-ttu-id="f87a2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f87a2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f87a2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f87a2-123">Authorization</span></span>|<span data-ttu-id="f87a2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f87a2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f87a2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f87a2-125">Accept</span></span>|<span data-ttu-id="f87a2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f87a2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f87a2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f87a2-127">Request body</span></span>
<span data-ttu-id="f87a2-128">No corpo da solicitação, fornece uma representação JSON para o [objeto androidWiFiConfiguration.](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f87a2-128">In the request body, supply a JSON representation for the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

<span data-ttu-id="f87a2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f87a2-129">The following table shows the properties that are required when you create the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span>

|<span data-ttu-id="f87a2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f87a2-130">Property</span></span>|<span data-ttu-id="f87a2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f87a2-131">Type</span></span>|<span data-ttu-id="f87a2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f87a2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f87a2-133">id</span><span class="sxs-lookup"><span data-stu-id="f87a2-133">id</span></span>|<span data-ttu-id="f87a2-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f87a2-134">String</span></span>|<span data-ttu-id="f87a2-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f87a2-135">Key of the entity.</span></span> <span data-ttu-id="f87a2-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f87a2-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f87a2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f87a2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f87a2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f87a2-138">DateTimeOffset</span></span>|<span data-ttu-id="f87a2-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f87a2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f87a2-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f87a2-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f87a2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f87a2-141">roleScopeTagIds</span></span>|<span data-ttu-id="f87a2-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f87a2-142">String collection</span></span>|<span data-ttu-id="f87a2-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="f87a2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f87a2-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f87a2-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f87a2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f87a2-145">supportsScopeTags</span></span>|<span data-ttu-id="f87a2-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="f87a2-146">Boolean</span></span>|<span data-ttu-id="f87a2-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f87a2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f87a2-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f87a2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f87a2-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f87a2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f87a2-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f87a2-150">This property is read-only.</span></span> <span data-ttu-id="f87a2-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f87a2-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f87a2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f87a2-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f87a2-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f87a2-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f87a2-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="f87a2-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f87a2-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f87a2-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f87a2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f87a2-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f87a2-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f87a2-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f87a2-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="f87a2-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f87a2-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f87a2-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f87a2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f87a2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f87a2-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f87a2-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f87a2-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="f87a2-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f87a2-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f87a2-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f87a2-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f87a2-164">createdDateTime</span></span>|<span data-ttu-id="f87a2-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f87a2-165">DateTimeOffset</span></span>|<span data-ttu-id="f87a2-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f87a2-166">DateTime the object was created.</span></span> <span data-ttu-id="f87a2-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f87a2-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f87a2-168">descrição</span><span class="sxs-lookup"><span data-stu-id="f87a2-168">description</span></span>|<span data-ttu-id="f87a2-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f87a2-169">String</span></span>|<span data-ttu-id="f87a2-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f87a2-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f87a2-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f87a2-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f87a2-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f87a2-172">displayName</span></span>|<span data-ttu-id="f87a2-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f87a2-173">String</span></span>|<span data-ttu-id="f87a2-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f87a2-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f87a2-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f87a2-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f87a2-176">versão</span><span class="sxs-lookup"><span data-stu-id="f87a2-176">version</span></span>|<span data-ttu-id="f87a2-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f87a2-177">Int32</span></span>|<span data-ttu-id="f87a2-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f87a2-178">Version of the device configuration.</span></span> <span data-ttu-id="f87a2-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f87a2-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f87a2-180">networkName</span><span class="sxs-lookup"><span data-stu-id="f87a2-180">networkName</span></span>|<span data-ttu-id="f87a2-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f87a2-181">String</span></span>|<span data-ttu-id="f87a2-182">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="f87a2-182">Network Name</span></span>|
|<span data-ttu-id="f87a2-183">ssid</span><span class="sxs-lookup"><span data-stu-id="f87a2-183">ssid</span></span>|<span data-ttu-id="f87a2-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f87a2-184">String</span></span>|<span data-ttu-id="f87a2-185">Esse é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f87a2-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="f87a2-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="f87a2-186">connectAutomatically</span></span>|<span data-ttu-id="f87a2-187">Booleano</span><span class="sxs-lookup"><span data-stu-id="f87a2-187">Boolean</span></span>|<span data-ttu-id="f87a2-188">Conecte-se automaticamente quando essa rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="f87a2-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="f87a2-189">Definir isso como true ignorará o prompt do usuário e conectará automaticamente o dispositivo Wi-Fi rede.</span><span class="sxs-lookup"><span data-stu-id="f87a2-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="f87a2-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="f87a2-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="f87a2-191">Booleano</span><span class="sxs-lookup"><span data-stu-id="f87a2-191">Boolean</span></span>|<span data-ttu-id="f87a2-192">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f87a2-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="f87a2-193">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="f87a2-193">wiFiSecurityType</span></span>|[<span data-ttu-id="f87a2-194">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="f87a2-194">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="f87a2-195">Indica se Wi-Fi ponto de extremidade usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="f87a2-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="f87a2-196">Os valores possíveis são: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="f87a2-196">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="f87a2-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="f87a2-197">Response</span></span>
<span data-ttu-id="f87a2-198">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f87a2-198">If successful, this method returns a `200 OK` response code and an updated [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f87a2-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f87a2-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="f87a2-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f87a2-200">Request</span></span>
<span data-ttu-id="f87a2-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f87a2-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f87a2-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="f87a2-202">Response</span></span>
<span data-ttu-id="f87a2-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f87a2-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




