---
title: Criar windowsWifiConfiguration
description: Crie um novo objeto de windowsWifiConfiguration.
author: tfitzmac
ms.openlocfilehash: 0d09897844acd0e0ea52103a371ff6825df10379
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305009"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="01533-103">Criar windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="01533-103">Create windowsWifiConfiguration</span></span>

> <span data-ttu-id="01533-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="01533-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01533-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="01533-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01533-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="01533-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01533-107">Crie um novo objeto de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="01533-107">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01533-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01533-108">Prerequisites</span></span>
<span data-ttu-id="01533-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01533-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01533-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01533-111">Permission type</span></span>|<span data-ttu-id="01533-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="01533-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01533-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01533-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01533-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01533-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01533-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01533-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01533-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01533-116">Not supported.</span></span>|
|<span data-ttu-id="01533-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01533-117">Application</span></span>|<span data-ttu-id="01533-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01533-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01533-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01533-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="01533-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01533-120">Request headers</span></span>
|<span data-ttu-id="01533-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01533-121">Header</span></span>|<span data-ttu-id="01533-122">Valor</span><span class="sxs-lookup"><span data-stu-id="01533-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01533-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="01533-123">Authorization</span></span>|<span data-ttu-id="01533-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01533-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01533-125">Accept</span><span class="sxs-lookup"><span data-stu-id="01533-125">Accept</span></span>|<span data-ttu-id="01533-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01533-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01533-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01533-127">Request body</span></span>
<span data-ttu-id="01533-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="01533-128">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="01533-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="01533-129">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="01533-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01533-130">Property</span></span>|<span data-ttu-id="01533-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="01533-131">Type</span></span>|<span data-ttu-id="01533-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="01533-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01533-133">id</span><span class="sxs-lookup"><span data-stu-id="01533-133">id</span></span>|<span data-ttu-id="01533-134">String</span><span class="sxs-lookup"><span data-stu-id="01533-134">String</span></span>|<span data-ttu-id="01533-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="01533-135">Key of the entity.</span></span> <span data-ttu-id="01533-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01533-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01533-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01533-137">lastModifiedDateTime</span></span>|<span data-ttu-id="01533-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01533-138">DateTimeOffset</span></span>|<span data-ttu-id="01533-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="01533-139">DateTime the object was last modified.</span></span> <span data-ttu-id="01533-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01533-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01533-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="01533-141">roleScopeTagIds</span></span>|<span data-ttu-id="01533-142">String collection</span><span class="sxs-lookup"><span data-stu-id="01533-142">String collection</span></span>|<span data-ttu-id="01533-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="01533-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="01533-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01533-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01533-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="01533-145">supportsScopeTags</span></span>|<span data-ttu-id="01533-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="01533-146">Boolean</span></span>|<span data-ttu-id="01533-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="01533-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="01533-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="01533-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="01533-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="01533-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="01533-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="01533-150">This property is read-only.</span></span> <span data-ttu-id="01533-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01533-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01533-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01533-152">createdDateTime</span></span>|<span data-ttu-id="01533-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01533-153">DateTimeOffset</span></span>|<span data-ttu-id="01533-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="01533-154">DateTime the object was created.</span></span> <span data-ttu-id="01533-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01533-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01533-156">description</span><span class="sxs-lookup"><span data-stu-id="01533-156">description</span></span>|<span data-ttu-id="01533-157">String</span><span class="sxs-lookup"><span data-stu-id="01533-157">String</span></span>|<span data-ttu-id="01533-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="01533-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="01533-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01533-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01533-160">displayName</span><span class="sxs-lookup"><span data-stu-id="01533-160">displayName</span></span>|<span data-ttu-id="01533-161">String</span><span class="sxs-lookup"><span data-stu-id="01533-161">String</span></span>|<span data-ttu-id="01533-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="01533-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="01533-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01533-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01533-164">version</span><span class="sxs-lookup"><span data-stu-id="01533-164">version</span></span>|<span data-ttu-id="01533-165">Int32</span><span class="sxs-lookup"><span data-stu-id="01533-165">Int32</span></span>|<span data-ttu-id="01533-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="01533-166">Version of the device configuration.</span></span> <span data-ttu-id="01533-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01533-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01533-168">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="01533-168">preSharedKey</span></span>|<span data-ttu-id="01533-169">String</span><span class="sxs-lookup"><span data-stu-id="01533-169">String</span></span>|<span data-ttu-id="01533-170">Esta é a chave pré compartilhada para rede Wi-Fi WPA Pessoal.</span><span class="sxs-lookup"><span data-stu-id="01533-170">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="01533-171">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="01533-171">wifiSecurityType</span></span>|[<span data-ttu-id="01533-172">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="01533-172">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="01533-173">Especifica o tipo de segurança Wifi.</span><span class="sxs-lookup"><span data-stu-id="01533-173">Specify the Wifi Security Type.</span></span> <span data-ttu-id="01533-174">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="01533-174">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="01533-175">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="01533-175">meteredConnectionLimit</span></span>|[<span data-ttu-id="01533-176">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="01533-176">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="01533-177">Especifica o tipo de limite de conexão monitorados para a conexão wifi.</span><span class="sxs-lookup"><span data-stu-id="01533-177">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="01533-178">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="01533-178">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="01533-179">SSID</span><span class="sxs-lookup"><span data-stu-id="01533-179">ssid</span></span>|<span data-ttu-id="01533-180">String</span><span class="sxs-lookup"><span data-stu-id="01533-180">String</span></span>|<span data-ttu-id="01533-181">Especifique o SSID da conexão wifi.</span><span class="sxs-lookup"><span data-stu-id="01533-181">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="01533-182">networkName</span><span class="sxs-lookup"><span data-stu-id="01533-182">networkName</span></span>|<span data-ttu-id="01533-183">String</span><span class="sxs-lookup"><span data-stu-id="01533-183">String</span></span>|<span data-ttu-id="01533-184">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="01533-184">Specify the network configuration name.</span></span>|
|<span data-ttu-id="01533-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="01533-185">connectAutomatically</span></span>|<span data-ttu-id="01533-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="01533-186">Boolean</span></span>|<span data-ttu-id="01533-187">Especifique se a conexão wifi deve conectar automaticamente quando estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="01533-187">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="01533-188">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="01533-188">connectToPreferredNetwork</span></span>|<span data-ttu-id="01533-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="01533-189">Boolean</span></span>|<span data-ttu-id="01533-190">Especifique se a conexão wifi deve se conectar às redes mais preferenciais quando já conectado a este.</span><span class="sxs-lookup"><span data-stu-id="01533-190">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="01533-191">Requer ConnectAutomatically seja true.</span><span class="sxs-lookup"><span data-stu-id="01533-191">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="01533-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="01533-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="01533-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="01533-193">Boolean</span></span>|<span data-ttu-id="01533-194">Especifique se a conexão wifi deve conectar automaticamente mesmo quando o SSID não está transmitindo.</span><span class="sxs-lookup"><span data-stu-id="01533-194">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="01533-195">proxySetting</span><span class="sxs-lookup"><span data-stu-id="01533-195">proxySetting</span></span>|[<span data-ttu-id="01533-196">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="01533-196">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="01533-197">Especifica a configuração para configuração de Wi-Fi do proxy.</span><span class="sxs-lookup"><span data-stu-id="01533-197">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="01533-198">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="01533-198">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="01533-199">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="01533-199">proxyManualAddress</span></span>|<span data-ttu-id="01533-200">String</span><span class="sxs-lookup"><span data-stu-id="01533-200">String</span></span>|<span data-ttu-id="01533-201">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="01533-201">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="01533-202">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="01533-202">proxyManualPort</span></span>|<span data-ttu-id="01533-203">Int32</span><span class="sxs-lookup"><span data-stu-id="01533-203">Int32</span></span>|<span data-ttu-id="01533-204">Especifique a porta para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="01533-204">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="01533-205">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="01533-205">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="01533-206">String</span><span class="sxs-lookup"><span data-stu-id="01533-206">String</span></span>|<span data-ttu-id="01533-207">Especifique a URL para o script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="01533-207">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="01533-208">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="01533-208">forceFIPSCompliance</span></span>|<span data-ttu-id="01533-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="01533-209">Boolean</span></span>|<span data-ttu-id="01533-210">Especifique se deseja forçar a conformidade FIPS.</span><span class="sxs-lookup"><span data-stu-id="01533-210">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="01533-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="01533-211">Response</span></span>
<span data-ttu-id="01533-212">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01533-212">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01533-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01533-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="01533-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01533-214">Request</span></span>
<span data-ttu-id="01533-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01533-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 850

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="01533-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="01533-216">Response</span></span>
<span data-ttu-id="01533-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01533-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





