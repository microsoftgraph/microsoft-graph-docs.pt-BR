---
title: Criar windowsWifiConfiguration
description: Criar um novo objeto windowsWifiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 55e8935c1bc845f770b78b3530a144c55dcb16cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42473427"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="47fe4-103">Criar windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="47fe4-103">Create windowsWifiConfiguration</span></span>

<span data-ttu-id="47fe4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="47fe4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47fe4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="47fe4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47fe4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47fe4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47fe4-107">Criar um novo objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="47fe4-107">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47fe4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47fe4-108">Prerequisites</span></span>
<span data-ttu-id="47fe4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47fe4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47fe4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47fe4-111">Permission type</span></span>|<span data-ttu-id="47fe4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="47fe4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47fe4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47fe4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47fe4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47fe4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47fe4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47fe4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47fe4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47fe4-116">Not supported.</span></span>|
|<span data-ttu-id="47fe4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47fe4-117">Application</span></span>|<span data-ttu-id="47fe4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47fe4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47fe4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47fe4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="47fe4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47fe4-120">Request headers</span></span>
|<span data-ttu-id="47fe4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47fe4-121">Header</span></span>|<span data-ttu-id="47fe4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="47fe4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47fe4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="47fe4-123">Authorization</span></span>|<span data-ttu-id="47fe4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47fe4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47fe4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="47fe4-125">Accept</span></span>|<span data-ttu-id="47fe4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47fe4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47fe4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47fe4-127">Request body</span></span>
<span data-ttu-id="47fe4-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="47fe4-128">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="47fe4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="47fe4-129">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="47fe4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47fe4-130">Property</span></span>|<span data-ttu-id="47fe4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="47fe4-131">Type</span></span>|<span data-ttu-id="47fe4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="47fe4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47fe4-133">id</span><span class="sxs-lookup"><span data-stu-id="47fe4-133">id</span></span>|<span data-ttu-id="47fe4-134">String</span><span class="sxs-lookup"><span data-stu-id="47fe4-134">String</span></span>|<span data-ttu-id="47fe4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="47fe4-135">Key of the entity.</span></span> <span data-ttu-id="47fe4-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47fe4-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47fe4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47fe4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="47fe4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47fe4-138">DateTimeOffset</span></span>|<span data-ttu-id="47fe4-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="47fe4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="47fe4-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47fe4-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47fe4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="47fe4-141">roleScopeTagIds</span></span>|<span data-ttu-id="47fe4-142">String collection</span><span class="sxs-lookup"><span data-stu-id="47fe4-142">String collection</span></span>|<span data-ttu-id="47fe4-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="47fe4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="47fe4-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47fe4-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47fe4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="47fe4-145">supportsScopeTags</span></span>|<span data-ttu-id="47fe4-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="47fe4-146">Boolean</span></span>|<span data-ttu-id="47fe4-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="47fe4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="47fe4-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="47fe4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="47fe4-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="47fe4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="47fe4-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="47fe4-150">This property is read-only.</span></span> <span data-ttu-id="47fe4-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47fe4-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47fe4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="47fe4-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="47fe4-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="47fe4-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="47fe4-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="47fe4-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="47fe4-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47fe4-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47fe4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="47fe4-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="47fe4-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="47fe4-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="47fe4-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="47fe4-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="47fe4-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47fe4-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47fe4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="47fe4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="47fe4-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="47fe4-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="47fe4-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="47fe4-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="47fe4-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47fe4-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47fe4-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47fe4-164">createdDateTime</span></span>|<span data-ttu-id="47fe4-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47fe4-165">DateTimeOffset</span></span>|<span data-ttu-id="47fe4-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="47fe4-166">DateTime the object was created.</span></span> <span data-ttu-id="47fe4-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47fe4-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47fe4-168">description</span><span class="sxs-lookup"><span data-stu-id="47fe4-168">description</span></span>|<span data-ttu-id="47fe4-169">String</span><span class="sxs-lookup"><span data-stu-id="47fe4-169">String</span></span>|<span data-ttu-id="47fe4-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47fe4-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="47fe4-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47fe4-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47fe4-172">displayName</span><span class="sxs-lookup"><span data-stu-id="47fe4-172">displayName</span></span>|<span data-ttu-id="47fe4-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47fe4-173">String</span></span>|<span data-ttu-id="47fe4-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47fe4-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="47fe4-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47fe4-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47fe4-176">versão</span><span class="sxs-lookup"><span data-stu-id="47fe4-176">version</span></span>|<span data-ttu-id="47fe4-177">Int32</span><span class="sxs-lookup"><span data-stu-id="47fe4-177">Int32</span></span>|<span data-ttu-id="47fe4-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47fe4-178">Version of the device configuration.</span></span> <span data-ttu-id="47fe4-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47fe4-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47fe4-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="47fe4-180">preSharedKey</span></span>|<span data-ttu-id="47fe4-181">String</span><span class="sxs-lookup"><span data-stu-id="47fe4-181">String</span></span>|<span data-ttu-id="47fe4-182">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="47fe4-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="47fe4-183">à</span><span class="sxs-lookup"><span data-stu-id="47fe4-183">wifiSecurityType</span></span>|[<span data-ttu-id="47fe4-184">à</span><span class="sxs-lookup"><span data-stu-id="47fe4-184">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="47fe4-185">Especifique o tipo de segurança wifi.</span><span class="sxs-lookup"><span data-stu-id="47fe4-185">Specify the Wifi Security Type.</span></span> <span data-ttu-id="47fe4-186">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="47fe4-186">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="47fe4-187">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="47fe4-187">meteredConnectionLimit</span></span>|[<span data-ttu-id="47fe4-188">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="47fe4-188">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="47fe4-189">Especifique o tipo de limite de conexão limitada para a conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="47fe4-189">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="47fe4-190">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="47fe4-190">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="47fe4-191">SSID</span><span class="sxs-lookup"><span data-stu-id="47fe4-191">ssid</span></span>|<span data-ttu-id="47fe4-192">String</span><span class="sxs-lookup"><span data-stu-id="47fe4-192">String</span></span>|<span data-ttu-id="47fe4-193">Especifique o SSID da conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="47fe4-193">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="47fe4-194">NetworkName</span><span class="sxs-lookup"><span data-stu-id="47fe4-194">networkName</span></span>|<span data-ttu-id="47fe4-195">String</span><span class="sxs-lookup"><span data-stu-id="47fe4-195">String</span></span>|<span data-ttu-id="47fe4-196">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="47fe4-196">Specify the network configuration name.</span></span>|
|<span data-ttu-id="47fe4-197">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="47fe4-197">connectAutomatically</span></span>|<span data-ttu-id="47fe4-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="47fe4-198">Boolean</span></span>|<span data-ttu-id="47fe4-199">Especifique se a conexão WiFi deve se conectar automaticamente quando estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="47fe4-199">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="47fe4-200">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="47fe4-200">connectToPreferredNetwork</span></span>|<span data-ttu-id="47fe4-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="47fe4-201">Boolean</span></span>|<span data-ttu-id="47fe4-202">Especifique se a conexão WiFi deve se conectar a redes mais preferenciais quando já estiver conectado a ela.</span><span class="sxs-lookup"><span data-stu-id="47fe4-202">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="47fe4-203">Requer que ConnectAutomatically seja true.</span><span class="sxs-lookup"><span data-stu-id="47fe4-203">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="47fe4-204">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="47fe4-204">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="47fe4-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="47fe4-205">Boolean</span></span>|<span data-ttu-id="47fe4-206">Especifique se a conexão WiFi deve se conectar automaticamente, mesmo quando o SSID não estiver transmitindo.</span><span class="sxs-lookup"><span data-stu-id="47fe4-206">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="47fe4-207">proxySetting</span><span class="sxs-lookup"><span data-stu-id="47fe4-207">proxySetting</span></span>|[<span data-ttu-id="47fe4-208">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="47fe4-208">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="47fe4-209">Especifique a configuração de proxy para a configuração de Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="47fe4-209">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="47fe4-210">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="47fe4-210">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="47fe4-211">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="47fe4-211">proxyManualAddress</span></span>|<span data-ttu-id="47fe4-212">String</span><span class="sxs-lookup"><span data-stu-id="47fe4-212">String</span></span>|<span data-ttu-id="47fe4-213">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="47fe4-213">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="47fe4-214">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="47fe4-214">proxyManualPort</span></span>|<span data-ttu-id="47fe4-215">Int32</span><span class="sxs-lookup"><span data-stu-id="47fe4-215">Int32</span></span>|<span data-ttu-id="47fe4-216">Especifique a porta do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="47fe4-216">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="47fe4-217">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="47fe4-217">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="47fe4-218">String</span><span class="sxs-lookup"><span data-stu-id="47fe4-218">String</span></span>|<span data-ttu-id="47fe4-219">Especifique a URL do script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="47fe4-219">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="47fe4-220">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="47fe4-220">forceFIPSCompliance</span></span>|<span data-ttu-id="47fe4-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="47fe4-221">Boolean</span></span>|<span data-ttu-id="47fe4-222">Especifique se a conformidade com FIPS deve ser forçada.</span><span class="sxs-lookup"><span data-stu-id="47fe4-222">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="47fe4-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="47fe4-223">Response</span></span>
<span data-ttu-id="47fe4-224">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47fe4-224">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47fe4-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47fe4-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="47fe4-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47fe4-226">Request</span></span>
<span data-ttu-id="47fe4-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47fe4-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="47fe4-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="47fe4-228">Response</span></span>
<span data-ttu-id="47fe4-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47fe4-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





