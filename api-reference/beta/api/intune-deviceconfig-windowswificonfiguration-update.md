---
title: Atualizar windowsWifiConfiguration
description: Atualiza as propriedades de um objeto windowsWifiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a7d346e9fc729c148746c229a043391158fadd0d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43332309"
---
# <a name="update-windowswificonfiguration"></a><span data-ttu-id="24a44-103">Atualizar windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="24a44-103">Update windowsWifiConfiguration</span></span>

<span data-ttu-id="24a44-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24a44-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24a44-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="24a44-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24a44-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="24a44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24a44-107">Atualiza as propriedades de um objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="24a44-107">Update the properties of a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24a44-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="24a44-108">Prerequisites</span></span>
<span data-ttu-id="24a44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24a44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24a44-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24a44-111">Permission type</span></span>|<span data-ttu-id="24a44-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="24a44-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24a44-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24a44-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24a44-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24a44-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24a44-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24a44-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24a44-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24a44-116">Not supported.</span></span>|
|<span data-ttu-id="24a44-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24a44-117">Application</span></span>|<span data-ttu-id="24a44-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24a44-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24a44-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24a44-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="24a44-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24a44-120">Request headers</span></span>
|<span data-ttu-id="24a44-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="24a44-121">Header</span></span>|<span data-ttu-id="24a44-122">Valor</span><span class="sxs-lookup"><span data-stu-id="24a44-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24a44-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="24a44-123">Authorization</span></span>|<span data-ttu-id="24a44-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24a44-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24a44-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="24a44-125">Accept</span></span>|<span data-ttu-id="24a44-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24a44-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24a44-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24a44-127">Request body</span></span>
<span data-ttu-id="24a44-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="24a44-128">In the request body, supply a JSON representation for the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

<span data-ttu-id="24a44-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="24a44-129">The following table shows the properties that are required when you create the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span>

|<span data-ttu-id="24a44-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24a44-130">Property</span></span>|<span data-ttu-id="24a44-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="24a44-131">Type</span></span>|<span data-ttu-id="24a44-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="24a44-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24a44-133">id</span><span class="sxs-lookup"><span data-stu-id="24a44-133">id</span></span>|<span data-ttu-id="24a44-134">String</span><span class="sxs-lookup"><span data-stu-id="24a44-134">String</span></span>|<span data-ttu-id="24a44-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="24a44-135">Key of the entity.</span></span> <span data-ttu-id="24a44-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24a44-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24a44-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24a44-137">lastModifiedDateTime</span></span>|<span data-ttu-id="24a44-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24a44-138">DateTimeOffset</span></span>|<span data-ttu-id="24a44-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="24a44-139">DateTime the object was last modified.</span></span> <span data-ttu-id="24a44-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24a44-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24a44-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="24a44-141">roleScopeTagIds</span></span>|<span data-ttu-id="24a44-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="24a44-142">String collection</span></span>|<span data-ttu-id="24a44-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="24a44-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="24a44-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24a44-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24a44-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="24a44-145">supportsScopeTags</span></span>|<span data-ttu-id="24a44-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="24a44-146">Boolean</span></span>|<span data-ttu-id="24a44-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="24a44-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="24a44-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="24a44-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="24a44-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="24a44-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="24a44-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="24a44-150">This property is read-only.</span></span> <span data-ttu-id="24a44-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24a44-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24a44-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="24a44-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="24a44-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="24a44-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="24a44-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="24a44-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="24a44-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24a44-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24a44-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="24a44-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="24a44-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="24a44-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="24a44-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="24a44-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="24a44-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24a44-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24a44-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="24a44-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="24a44-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="24a44-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="24a44-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="24a44-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="24a44-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24a44-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24a44-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24a44-164">createdDateTime</span></span>|<span data-ttu-id="24a44-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24a44-165">DateTimeOffset</span></span>|<span data-ttu-id="24a44-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="24a44-166">DateTime the object was created.</span></span> <span data-ttu-id="24a44-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24a44-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24a44-168">description</span><span class="sxs-lookup"><span data-stu-id="24a44-168">description</span></span>|<span data-ttu-id="24a44-169">String</span><span class="sxs-lookup"><span data-stu-id="24a44-169">String</span></span>|<span data-ttu-id="24a44-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="24a44-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="24a44-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24a44-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24a44-172">displayName</span><span class="sxs-lookup"><span data-stu-id="24a44-172">displayName</span></span>|<span data-ttu-id="24a44-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24a44-173">String</span></span>|<span data-ttu-id="24a44-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="24a44-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="24a44-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24a44-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24a44-176">versão</span><span class="sxs-lookup"><span data-stu-id="24a44-176">version</span></span>|<span data-ttu-id="24a44-177">Int32</span><span class="sxs-lookup"><span data-stu-id="24a44-177">Int32</span></span>|<span data-ttu-id="24a44-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="24a44-178">Version of the device configuration.</span></span> <span data-ttu-id="24a44-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24a44-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24a44-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="24a44-180">preSharedKey</span></span>|<span data-ttu-id="24a44-181">String</span><span class="sxs-lookup"><span data-stu-id="24a44-181">String</span></span>|<span data-ttu-id="24a44-182">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="24a44-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="24a44-183">à</span><span class="sxs-lookup"><span data-stu-id="24a44-183">wifiSecurityType</span></span>|[<span data-ttu-id="24a44-184">à</span><span class="sxs-lookup"><span data-stu-id="24a44-184">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="24a44-185">Especifique o tipo de segurança wifi.</span><span class="sxs-lookup"><span data-stu-id="24a44-185">Specify the Wifi Security Type.</span></span> <span data-ttu-id="24a44-186">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="24a44-186">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="24a44-187">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="24a44-187">meteredConnectionLimit</span></span>|[<span data-ttu-id="24a44-188">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="24a44-188">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="24a44-189">Especifique o tipo de limite de conexão limitada para a conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="24a44-189">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="24a44-190">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="24a44-190">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="24a44-191">SSID</span><span class="sxs-lookup"><span data-stu-id="24a44-191">ssid</span></span>|<span data-ttu-id="24a44-192">String</span><span class="sxs-lookup"><span data-stu-id="24a44-192">String</span></span>|<span data-ttu-id="24a44-193">Especifique o SSID da conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="24a44-193">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="24a44-194">NetworkName</span><span class="sxs-lookup"><span data-stu-id="24a44-194">networkName</span></span>|<span data-ttu-id="24a44-195">String</span><span class="sxs-lookup"><span data-stu-id="24a44-195">String</span></span>|<span data-ttu-id="24a44-196">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="24a44-196">Specify the network configuration name.</span></span>|
|<span data-ttu-id="24a44-197">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="24a44-197">connectAutomatically</span></span>|<span data-ttu-id="24a44-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="24a44-198">Boolean</span></span>|<span data-ttu-id="24a44-199">Especifique se a conexão WiFi deve se conectar automaticamente quando estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="24a44-199">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="24a44-200">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="24a44-200">connectToPreferredNetwork</span></span>|<span data-ttu-id="24a44-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="24a44-201">Boolean</span></span>|<span data-ttu-id="24a44-202">Especifique se a conexão WiFi deve se conectar a redes mais preferenciais quando já estiver conectado a ela.</span><span class="sxs-lookup"><span data-stu-id="24a44-202">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="24a44-203">Requer que ConnectAutomatically seja true.</span><span class="sxs-lookup"><span data-stu-id="24a44-203">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="24a44-204">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="24a44-204">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="24a44-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="24a44-205">Boolean</span></span>|<span data-ttu-id="24a44-206">Especifique se a conexão WiFi deve se conectar automaticamente, mesmo quando o SSID não estiver transmitindo.</span><span class="sxs-lookup"><span data-stu-id="24a44-206">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="24a44-207">proxySetting</span><span class="sxs-lookup"><span data-stu-id="24a44-207">proxySetting</span></span>|[<span data-ttu-id="24a44-208">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="24a44-208">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="24a44-209">Especifique a configuração de proxy para a configuração de Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="24a44-209">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="24a44-210">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="24a44-210">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="24a44-211">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="24a44-211">proxyManualAddress</span></span>|<span data-ttu-id="24a44-212">String</span><span class="sxs-lookup"><span data-stu-id="24a44-212">String</span></span>|<span data-ttu-id="24a44-213">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="24a44-213">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="24a44-214">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="24a44-214">proxyManualPort</span></span>|<span data-ttu-id="24a44-215">Int32</span><span class="sxs-lookup"><span data-stu-id="24a44-215">Int32</span></span>|<span data-ttu-id="24a44-216">Especifique a porta do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="24a44-216">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="24a44-217">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="24a44-217">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="24a44-218">String</span><span class="sxs-lookup"><span data-stu-id="24a44-218">String</span></span>|<span data-ttu-id="24a44-219">Especifique a URL do script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="24a44-219">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="24a44-220">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="24a44-220">forceFIPSCompliance</span></span>|<span data-ttu-id="24a44-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="24a44-221">Boolean</span></span>|<span data-ttu-id="24a44-222">Especifique se a conformidade com FIPS deve ser forçada.</span><span class="sxs-lookup"><span data-stu-id="24a44-222">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="24a44-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="24a44-223">Response</span></span>
<span data-ttu-id="24a44-224">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24a44-224">If successful, this method returns a `200 OK` response code and an updated [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24a44-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24a44-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="24a44-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24a44-226">Request</span></span>
<span data-ttu-id="24a44-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24a44-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1559

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
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
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```

### <a name="response"></a><span data-ttu-id="24a44-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="24a44-228">Response</span></span>
<span data-ttu-id="24a44-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24a44-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1731

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "id": "8a9e790f-790f-8a9e-0f79-9e8a0f799e8a",
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
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```



