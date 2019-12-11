---
title: Criar windowsWifiConfiguration
description: Criar um novo objeto windowsWifiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 307a04bf60faa9f4287436d7255fdc6c5e30137a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946319"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="aa890-103">Criar windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="aa890-103">Create windowsWifiConfiguration</span></span>

> <span data-ttu-id="aa890-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aa890-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa890-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa890-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa890-106">Criar um novo objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="aa890-106">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa890-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aa890-107">Prerequisites</span></span>
<span data-ttu-id="aa890-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa890-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa890-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa890-110">Permission type</span></span>|<span data-ttu-id="aa890-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aa890-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa890-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa890-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aa890-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa890-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aa890-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa890-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa890-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa890-115">Not supported.</span></span>|
|<span data-ttu-id="aa890-116">Application</span><span class="sxs-lookup"><span data-stu-id="aa890-116">Application</span></span>|<span data-ttu-id="aa890-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa890-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa890-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa890-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="aa890-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa890-119">Request headers</span></span>
|<span data-ttu-id="aa890-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aa890-120">Header</span></span>|<span data-ttu-id="aa890-121">Valor</span><span class="sxs-lookup"><span data-stu-id="aa890-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa890-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa890-122">Authorization</span></span>|<span data-ttu-id="aa890-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa890-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa890-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aa890-124">Accept</span></span>|<span data-ttu-id="aa890-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aa890-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa890-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa890-126">Request body</span></span>
<span data-ttu-id="aa890-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="aa890-127">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="aa890-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="aa890-128">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="aa890-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa890-129">Property</span></span>|<span data-ttu-id="aa890-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa890-130">Type</span></span>|<span data-ttu-id="aa890-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa890-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa890-132">id</span><span class="sxs-lookup"><span data-stu-id="aa890-132">id</span></span>|<span data-ttu-id="aa890-133">String</span><span class="sxs-lookup"><span data-stu-id="aa890-133">String</span></span>|<span data-ttu-id="aa890-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aa890-134">Key of the entity.</span></span> <span data-ttu-id="aa890-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa890-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa890-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa890-136">lastModifiedDateTime</span></span>|<span data-ttu-id="aa890-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa890-137">DateTimeOffset</span></span>|<span data-ttu-id="aa890-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="aa890-138">DateTime the object was last modified.</span></span> <span data-ttu-id="aa890-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa890-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa890-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aa890-140">roleScopeTagIds</span></span>|<span data-ttu-id="aa890-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa890-141">String collection</span></span>|<span data-ttu-id="aa890-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="aa890-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aa890-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa890-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa890-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="aa890-144">supportsScopeTags</span></span>|<span data-ttu-id="aa890-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa890-145">Boolean</span></span>|<span data-ttu-id="aa890-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="aa890-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aa890-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="aa890-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aa890-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="aa890-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aa890-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aa890-149">This property is read-only.</span></span> <span data-ttu-id="aa890-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa890-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa890-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="aa890-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="aa890-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="aa890-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="aa890-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="aa890-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="aa890-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa890-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa890-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="aa890-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="aa890-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="aa890-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="aa890-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="aa890-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="aa890-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa890-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa890-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="aa890-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="aa890-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="aa890-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="aa890-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="aa890-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="aa890-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa890-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa890-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa890-163">createdDateTime</span></span>|<span data-ttu-id="aa890-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa890-164">DateTimeOffset</span></span>|<span data-ttu-id="aa890-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="aa890-165">DateTime the object was created.</span></span> <span data-ttu-id="aa890-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa890-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa890-167">description</span><span class="sxs-lookup"><span data-stu-id="aa890-167">description</span></span>|<span data-ttu-id="aa890-168">String</span><span class="sxs-lookup"><span data-stu-id="aa890-168">String</span></span>|<span data-ttu-id="aa890-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aa890-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aa890-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa890-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa890-171">displayName</span><span class="sxs-lookup"><span data-stu-id="aa890-171">displayName</span></span>|<span data-ttu-id="aa890-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa890-172">String</span></span>|<span data-ttu-id="aa890-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aa890-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aa890-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa890-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa890-175">versão</span><span class="sxs-lookup"><span data-stu-id="aa890-175">version</span></span>|<span data-ttu-id="aa890-176">Int32</span><span class="sxs-lookup"><span data-stu-id="aa890-176">Int32</span></span>|<span data-ttu-id="aa890-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aa890-177">Version of the device configuration.</span></span> <span data-ttu-id="aa890-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa890-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa890-179">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="aa890-179">preSharedKey</span></span>|<span data-ttu-id="aa890-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="aa890-180">String</span></span>|<span data-ttu-id="aa890-181">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="aa890-181">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="aa890-182">à</span><span class="sxs-lookup"><span data-stu-id="aa890-182">wifiSecurityType</span></span>|[<span data-ttu-id="aa890-183">à</span><span class="sxs-lookup"><span data-stu-id="aa890-183">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="aa890-184">Especifique o tipo de segurança wifi.</span><span class="sxs-lookup"><span data-stu-id="aa890-184">Specify the Wifi Security Type.</span></span> <span data-ttu-id="aa890-185">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="aa890-185">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="aa890-186">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="aa890-186">meteredConnectionLimit</span></span>|[<span data-ttu-id="aa890-187">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="aa890-187">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="aa890-188">Especifique o tipo de limite de conexão limitada para a conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="aa890-188">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="aa890-189">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="aa890-189">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="aa890-190">SSID</span><span class="sxs-lookup"><span data-stu-id="aa890-190">ssid</span></span>|<span data-ttu-id="aa890-191">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="aa890-191">String</span></span>|<span data-ttu-id="aa890-192">Especifique o SSID da conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="aa890-192">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="aa890-193">NetworkName</span><span class="sxs-lookup"><span data-stu-id="aa890-193">networkName</span></span>|<span data-ttu-id="aa890-194">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="aa890-194">String</span></span>|<span data-ttu-id="aa890-195">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="aa890-195">Specify the network configuration name.</span></span>|
|<span data-ttu-id="aa890-196">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="aa890-196">connectAutomatically</span></span>|<span data-ttu-id="aa890-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa890-197">Boolean</span></span>|<span data-ttu-id="aa890-198">Especifique se a conexão WiFi deve se conectar automaticamente quando estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="aa890-198">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="aa890-199">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="aa890-199">connectToPreferredNetwork</span></span>|<span data-ttu-id="aa890-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa890-200">Boolean</span></span>|<span data-ttu-id="aa890-201">Especifique se a conexão WiFi deve se conectar a redes mais preferenciais quando já estiver conectado a ela.</span><span class="sxs-lookup"><span data-stu-id="aa890-201">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="aa890-202">Requer que ConnectAutomatically seja true.</span><span class="sxs-lookup"><span data-stu-id="aa890-202">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="aa890-203">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="aa890-203">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="aa890-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa890-204">Boolean</span></span>|<span data-ttu-id="aa890-205">Especifique se a conexão WiFi deve se conectar automaticamente, mesmo quando o SSID não estiver transmitindo.</span><span class="sxs-lookup"><span data-stu-id="aa890-205">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="aa890-206">proxySetting</span><span class="sxs-lookup"><span data-stu-id="aa890-206">proxySetting</span></span>|[<span data-ttu-id="aa890-207">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="aa890-207">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="aa890-208">Especifique a configuração de proxy para a configuração de Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="aa890-208">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="aa890-209">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="aa890-209">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="aa890-210">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="aa890-210">proxyManualAddress</span></span>|<span data-ttu-id="aa890-211">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="aa890-211">String</span></span>|<span data-ttu-id="aa890-212">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="aa890-212">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="aa890-213">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="aa890-213">proxyManualPort</span></span>|<span data-ttu-id="aa890-214">Int32</span><span class="sxs-lookup"><span data-stu-id="aa890-214">Int32</span></span>|<span data-ttu-id="aa890-215">Especifique a porta do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="aa890-215">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="aa890-216">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="aa890-216">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="aa890-217">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="aa890-217">String</span></span>|<span data-ttu-id="aa890-218">Especifique a URL do script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="aa890-218">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="aa890-219">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="aa890-219">forceFIPSCompliance</span></span>|<span data-ttu-id="aa890-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa890-220">Boolean</span></span>|<span data-ttu-id="aa890-221">Especifique se a conformidade com FIPS deve ser forçada.</span><span class="sxs-lookup"><span data-stu-id="aa890-221">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="aa890-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa890-222">Response</span></span>
<span data-ttu-id="aa890-223">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa890-223">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa890-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa890-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa890-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa890-225">Request</span></span>
<span data-ttu-id="aa890-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa890-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="aa890-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa890-227">Response</span></span>
<span data-ttu-id="aa890-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa890-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





