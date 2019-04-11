---
title: Atualizar windowsWifiConfiguration
description: Atualiza as propriedades de um objeto windowsWifiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 07573055554ac68aea1caa14a774c92bb2ef713f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781565"
---
# <a name="update-windowswificonfiguration"></a><span data-ttu-id="9af7e-103">Atualizar windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="9af7e-103">Update windowsWifiConfiguration</span></span>

> <span data-ttu-id="9af7e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9af7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9af7e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9af7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9af7e-106">Atualiza as propriedades de um objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9af7e-106">Update the properties of a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9af7e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9af7e-107">Prerequisites</span></span>
<span data-ttu-id="9af7e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9af7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9af7e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9af7e-110">Permission type</span></span>|<span data-ttu-id="9af7e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9af7e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9af7e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9af7e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9af7e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9af7e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9af7e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9af7e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9af7e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9af7e-115">Not supported.</span></span>|
|<span data-ttu-id="9af7e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9af7e-116">Application</span></span>|<span data-ttu-id="9af7e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9af7e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9af7e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9af7e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9af7e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9af7e-119">Request headers</span></span>
|<span data-ttu-id="9af7e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9af7e-120">Header</span></span>|<span data-ttu-id="9af7e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9af7e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9af7e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9af7e-122">Authorization</span></span>|<span data-ttu-id="9af7e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9af7e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9af7e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9af7e-124">Accept</span></span>|<span data-ttu-id="9af7e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9af7e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9af7e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9af7e-126">Request body</span></span>
<span data-ttu-id="9af7e-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9af7e-127">In the request body, supply a JSON representation for the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

<span data-ttu-id="9af7e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9af7e-128">The following table shows the properties that are required when you create the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span>

|<span data-ttu-id="9af7e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9af7e-129">Property</span></span>|<span data-ttu-id="9af7e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9af7e-130">Type</span></span>|<span data-ttu-id="9af7e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9af7e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9af7e-132">id</span><span class="sxs-lookup"><span data-stu-id="9af7e-132">id</span></span>|<span data-ttu-id="9af7e-133">String</span><span class="sxs-lookup"><span data-stu-id="9af7e-133">String</span></span>|<span data-ttu-id="9af7e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9af7e-134">Key of the entity.</span></span> <span data-ttu-id="9af7e-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9af7e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9af7e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9af7e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9af7e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9af7e-137">DateTimeOffset</span></span>|<span data-ttu-id="9af7e-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9af7e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9af7e-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9af7e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9af7e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9af7e-140">roleScopeTagIds</span></span>|<span data-ttu-id="9af7e-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="9af7e-141">String collection</span></span>|<span data-ttu-id="9af7e-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="9af7e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9af7e-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9af7e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9af7e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9af7e-144">supportsScopeTags</span></span>|<span data-ttu-id="9af7e-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="9af7e-145">Boolean</span></span>|<span data-ttu-id="9af7e-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9af7e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9af7e-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9af7e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9af7e-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9af7e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9af7e-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9af7e-149">This property is read-only.</span></span> <span data-ttu-id="9af7e-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9af7e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9af7e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9af7e-151">createdDateTime</span></span>|<span data-ttu-id="9af7e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9af7e-152">DateTimeOffset</span></span>|<span data-ttu-id="9af7e-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9af7e-153">DateTime the object was created.</span></span> <span data-ttu-id="9af7e-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9af7e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9af7e-155">description</span><span class="sxs-lookup"><span data-stu-id="9af7e-155">description</span></span>|<span data-ttu-id="9af7e-156">String</span><span class="sxs-lookup"><span data-stu-id="9af7e-156">String</span></span>|<span data-ttu-id="9af7e-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9af7e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9af7e-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9af7e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9af7e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9af7e-159">displayName</span></span>|<span data-ttu-id="9af7e-160">String</span><span class="sxs-lookup"><span data-stu-id="9af7e-160">String</span></span>|<span data-ttu-id="9af7e-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9af7e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9af7e-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9af7e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9af7e-163">versão</span><span class="sxs-lookup"><span data-stu-id="9af7e-163">version</span></span>|<span data-ttu-id="9af7e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9af7e-164">Int32</span></span>|<span data-ttu-id="9af7e-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9af7e-165">Version of the device configuration.</span></span> <span data-ttu-id="9af7e-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9af7e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9af7e-167">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="9af7e-167">preSharedKey</span></span>|<span data-ttu-id="9af7e-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9af7e-168">String</span></span>|<span data-ttu-id="9af7e-169">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="9af7e-169">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="9af7e-170">à</span><span class="sxs-lookup"><span data-stu-id="9af7e-170">wifiSecurityType</span></span>|[<span data-ttu-id="9af7e-171">à</span><span class="sxs-lookup"><span data-stu-id="9af7e-171">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="9af7e-172">Especifique o tipo de segurança wifi.</span><span class="sxs-lookup"><span data-stu-id="9af7e-172">Specify the Wifi Security Type.</span></span> <span data-ttu-id="9af7e-173">Os valores possíveis são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="9af7e-173">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="9af7e-174">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="9af7e-174">meteredConnectionLimit</span></span>|[<span data-ttu-id="9af7e-175">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="9af7e-175">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="9af7e-176">Especifique o tipo de limite de conexão limitada para a conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="9af7e-176">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="9af7e-177">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="9af7e-177">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="9af7e-178">SSID</span><span class="sxs-lookup"><span data-stu-id="9af7e-178">ssid</span></span>|<span data-ttu-id="9af7e-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9af7e-179">String</span></span>|<span data-ttu-id="9af7e-180">Especifique o SSID da conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="9af7e-180">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="9af7e-181">NetworkName</span><span class="sxs-lookup"><span data-stu-id="9af7e-181">networkName</span></span>|<span data-ttu-id="9af7e-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9af7e-182">String</span></span>|<span data-ttu-id="9af7e-183">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="9af7e-183">Specify the network configuration name.</span></span>|
|<span data-ttu-id="9af7e-184">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="9af7e-184">connectAutomatically</span></span>|<span data-ttu-id="9af7e-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="9af7e-185">Boolean</span></span>|<span data-ttu-id="9af7e-186">Especifique se a conexão WiFi deve se conectar automaticamente quando estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="9af7e-186">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="9af7e-187">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="9af7e-187">connectToPreferredNetwork</span></span>|<span data-ttu-id="9af7e-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="9af7e-188">Boolean</span></span>|<span data-ttu-id="9af7e-189">Especifique se a conexão WiFi deve se conectar a redes mais preferenciais quando já estiver conectado a ela.</span><span class="sxs-lookup"><span data-stu-id="9af7e-189">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="9af7e-190">Requer que ConnectAutomatically seja true.</span><span class="sxs-lookup"><span data-stu-id="9af7e-190">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="9af7e-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="9af7e-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="9af7e-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="9af7e-192">Boolean</span></span>|<span data-ttu-id="9af7e-193">Especifique se a conexão WiFi deve se conectar automaticamente, mesmo quando o SSID não estiver transmitindo.</span><span class="sxs-lookup"><span data-stu-id="9af7e-193">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="9af7e-194">proxySetting</span><span class="sxs-lookup"><span data-stu-id="9af7e-194">proxySetting</span></span>|[<span data-ttu-id="9af7e-195">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="9af7e-195">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="9af7e-196">Especifique a configuração de proxy para a configuração de Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="9af7e-196">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="9af7e-197">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="9af7e-197">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="9af7e-198">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="9af7e-198">proxyManualAddress</span></span>|<span data-ttu-id="9af7e-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9af7e-199">String</span></span>|<span data-ttu-id="9af7e-200">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="9af7e-200">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="9af7e-201">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="9af7e-201">proxyManualPort</span></span>|<span data-ttu-id="9af7e-202">Int32</span><span class="sxs-lookup"><span data-stu-id="9af7e-202">Int32</span></span>|<span data-ttu-id="9af7e-203">Especifique a porta do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="9af7e-203">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="9af7e-204">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="9af7e-204">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="9af7e-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9af7e-205">String</span></span>|<span data-ttu-id="9af7e-206">Especifique a URL do script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="9af7e-206">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="9af7e-207">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="9af7e-207">forceFIPSCompliance</span></span>|<span data-ttu-id="9af7e-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="9af7e-208">Boolean</span></span>|<span data-ttu-id="9af7e-209">Especifique se a conformidade com FIPS deve ser forçada.</span><span class="sxs-lookup"><span data-stu-id="9af7e-209">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="9af7e-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="9af7e-210">Response</span></span>
<span data-ttu-id="9af7e-211">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9af7e-211">If successful, this method returns a `200 OK` response code and an updated [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9af7e-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9af7e-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="9af7e-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9af7e-213">Request</span></span>
<span data-ttu-id="9af7e-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9af7e-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 786

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="9af7e-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="9af7e-215">Response</span></span>
<span data-ttu-id="9af7e-p114">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9af7e-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 958

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "id": "8a9e790f-790f-8a9e-0f79-9e8a0f799e8a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





