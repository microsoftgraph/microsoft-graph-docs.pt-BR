---
title: Criar windowsWifiConfiguration
description: Criar um novo objeto windowsWifiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b8cf2c1da53cea38df4e4c184be3863564b0053c
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37181354"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="4ddc0-103">Criar windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ddc0-103">Create windowsWifiConfiguration</span></span>

> <span data-ttu-id="4ddc0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ddc0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ddc0-106">Criar um novo objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4ddc0-106">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ddc0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4ddc0-107">Prerequisites</span></span>
<span data-ttu-id="4ddc0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ddc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ddc0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ddc0-110">Permission type</span></span>|<span data-ttu-id="4ddc0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4ddc0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ddc0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ddc0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ddc0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ddc0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ddc0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ddc0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ddc0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-115">Not supported.</span></span>|
|<span data-ttu-id="4ddc0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ddc0-116">Application</span></span>|<span data-ttu-id="4ddc0-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ddc0-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ddc0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ddc0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4ddc0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ddc0-119">Request headers</span></span>
|<span data-ttu-id="4ddc0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4ddc0-120">Header</span></span>|<span data-ttu-id="4ddc0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4ddc0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ddc0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ddc0-122">Authorization</span></span>|<span data-ttu-id="4ddc0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ddc0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4ddc0-124">Accept</span></span>|<span data-ttu-id="4ddc0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ddc0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ddc0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ddc0-126">Request body</span></span>
<span data-ttu-id="4ddc0-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-127">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="4ddc0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-128">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="4ddc0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ddc0-129">Property</span></span>|<span data-ttu-id="4ddc0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ddc0-130">Type</span></span>|<span data-ttu-id="4ddc0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ddc0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ddc0-132">id</span><span class="sxs-lookup"><span data-stu-id="4ddc0-132">id</span></span>|<span data-ttu-id="4ddc0-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ddc0-133">String</span></span>|<span data-ttu-id="4ddc0-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-134">Key of the entity.</span></span> <span data-ttu-id="4ddc0-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ddc0-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ddc0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ddc0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4ddc0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ddc0-137">DateTimeOffset</span></span>|<span data-ttu-id="4ddc0-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4ddc0-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ddc0-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ddc0-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4ddc0-140">roleScopeTagIds</span></span>|<span data-ttu-id="4ddc0-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ddc0-141">String collection</span></span>|<span data-ttu-id="4ddc0-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4ddc0-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ddc0-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ddc0-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4ddc0-144">supportsScopeTags</span></span>|<span data-ttu-id="4ddc0-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="4ddc0-145">Boolean</span></span>|<span data-ttu-id="4ddc0-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4ddc0-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4ddc0-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4ddc0-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-149">This property is read-only.</span></span> <span data-ttu-id="4ddc0-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ddc0-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ddc0-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4ddc0-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4ddc0-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4ddc0-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4ddc0-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4ddc0-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ddc0-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ddc0-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4ddc0-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4ddc0-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4ddc0-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4ddc0-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4ddc0-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ddc0-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ddc0-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4ddc0-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4ddc0-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4ddc0-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4ddc0-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4ddc0-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ddc0-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ddc0-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ddc0-163">createdDateTime</span></span>|<span data-ttu-id="4ddc0-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ddc0-164">DateTimeOffset</span></span>|<span data-ttu-id="4ddc0-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-165">DateTime the object was created.</span></span> <span data-ttu-id="4ddc0-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ddc0-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ddc0-167">descrição</span><span class="sxs-lookup"><span data-stu-id="4ddc0-167">description</span></span>|<span data-ttu-id="4ddc0-168">String</span><span class="sxs-lookup"><span data-stu-id="4ddc0-168">String</span></span>|<span data-ttu-id="4ddc0-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4ddc0-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ddc0-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ddc0-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4ddc0-171">displayName</span></span>|<span data-ttu-id="4ddc0-172">String</span><span class="sxs-lookup"><span data-stu-id="4ddc0-172">String</span></span>|<span data-ttu-id="4ddc0-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4ddc0-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ddc0-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ddc0-175">versão</span><span class="sxs-lookup"><span data-stu-id="4ddc0-175">version</span></span>|<span data-ttu-id="4ddc0-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4ddc0-176">Int32</span></span>|<span data-ttu-id="4ddc0-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-177">Version of the device configuration.</span></span> <span data-ttu-id="4ddc0-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ddc0-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ddc0-179">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="4ddc0-179">preSharedKey</span></span>|<span data-ttu-id="4ddc0-180">String</span><span class="sxs-lookup"><span data-stu-id="4ddc0-180">String</span></span>|<span data-ttu-id="4ddc0-181">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-181">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="4ddc0-182">à</span><span class="sxs-lookup"><span data-stu-id="4ddc0-182">wifiSecurityType</span></span>|[<span data-ttu-id="4ddc0-183">à</span><span class="sxs-lookup"><span data-stu-id="4ddc0-183">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="4ddc0-184">Especifique o tipo de segurança wifi.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-184">Specify the Wifi Security Type.</span></span> <span data-ttu-id="4ddc0-185">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-185">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="4ddc0-186">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="4ddc0-186">meteredConnectionLimit</span></span>|[<span data-ttu-id="4ddc0-187">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="4ddc0-187">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="4ddc0-188">Especifique o tipo de limite de conexão limitada para a conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-188">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="4ddc0-189">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-189">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="4ddc0-190">SSID</span><span class="sxs-lookup"><span data-stu-id="4ddc0-190">ssid</span></span>|<span data-ttu-id="4ddc0-191">String</span><span class="sxs-lookup"><span data-stu-id="4ddc0-191">String</span></span>|<span data-ttu-id="4ddc0-192">Especifique o SSID da conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-192">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="4ddc0-193">NetworkName</span><span class="sxs-lookup"><span data-stu-id="4ddc0-193">networkName</span></span>|<span data-ttu-id="4ddc0-194">String</span><span class="sxs-lookup"><span data-stu-id="4ddc0-194">String</span></span>|<span data-ttu-id="4ddc0-195">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-195">Specify the network configuration name.</span></span>|
|<span data-ttu-id="4ddc0-196">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="4ddc0-196">connectAutomatically</span></span>|<span data-ttu-id="4ddc0-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="4ddc0-197">Boolean</span></span>|<span data-ttu-id="4ddc0-198">Especifique se a conexão WiFi deve se conectar automaticamente quando estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-198">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="4ddc0-199">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="4ddc0-199">connectToPreferredNetwork</span></span>|<span data-ttu-id="4ddc0-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="4ddc0-200">Boolean</span></span>|<span data-ttu-id="4ddc0-201">Especifique se a conexão WiFi deve se conectar a redes mais preferenciais quando já estiver conectado a ela.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-201">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="4ddc0-202">Requer que ConnectAutomatically seja true.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-202">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="4ddc0-203">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="4ddc0-203">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="4ddc0-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="4ddc0-204">Boolean</span></span>|<span data-ttu-id="4ddc0-205">Especifique se a conexão WiFi deve se conectar automaticamente, mesmo quando o SSID não estiver transmitindo.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-205">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="4ddc0-206">proxySetting</span><span class="sxs-lookup"><span data-stu-id="4ddc0-206">proxySetting</span></span>|[<span data-ttu-id="4ddc0-207">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="4ddc0-207">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="4ddc0-208">Especifique a configuração de proxy para a configuração de Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-208">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="4ddc0-209">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-209">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="4ddc0-210">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="4ddc0-210">proxyManualAddress</span></span>|<span data-ttu-id="4ddc0-211">String</span><span class="sxs-lookup"><span data-stu-id="4ddc0-211">String</span></span>|<span data-ttu-id="4ddc0-212">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-212">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="4ddc0-213">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="4ddc0-213">proxyManualPort</span></span>|<span data-ttu-id="4ddc0-214">Int32</span><span class="sxs-lookup"><span data-stu-id="4ddc0-214">Int32</span></span>|<span data-ttu-id="4ddc0-215">Especifique a porta do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-215">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="4ddc0-216">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="4ddc0-216">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="4ddc0-217">String</span><span class="sxs-lookup"><span data-stu-id="4ddc0-217">String</span></span>|<span data-ttu-id="4ddc0-218">Especifique a URL do script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-218">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="4ddc0-219">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="4ddc0-219">forceFIPSCompliance</span></span>|<span data-ttu-id="4ddc0-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="4ddc0-220">Boolean</span></span>|<span data-ttu-id="4ddc0-221">Especifique se a conformidade com FIPS deve ser forçada.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-221">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="4ddc0-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ddc0-222">Response</span></span>
<span data-ttu-id="4ddc0-223">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-223">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ddc0-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ddc0-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ddc0-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ddc0-225">Request</span></span>
<span data-ttu-id="4ddc0-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-226">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4ddc0-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ddc0-227">Response</span></span>
<span data-ttu-id="4ddc0-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ddc0-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




