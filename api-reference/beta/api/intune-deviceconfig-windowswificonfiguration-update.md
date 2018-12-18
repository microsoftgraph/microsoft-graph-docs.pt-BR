---
title: Atualizar windowsWifiConfiguration
description: Atualize as propriedades de um objeto windowsWifiConfiguration.
author: tfitzmac
ms.openlocfilehash: 0cd1d8ba372daf63561bf94763994fedafb24f46
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310280"
---
# <a name="update-windowswificonfiguration"></a><span data-ttu-id="9ec11-103">Atualizar windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="9ec11-103">Update windowsWifiConfiguration</span></span>

> <span data-ttu-id="9ec11-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9ec11-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ec11-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9ec11-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ec11-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9ec11-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ec11-107">Atualize as propriedades de um objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9ec11-107">Update the properties of a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9ec11-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ec11-108">Prerequisites</span></span>
<span data-ttu-id="9ec11-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ec11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ec11-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ec11-111">Permission type</span></span>|<span data-ttu-id="9ec11-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9ec11-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ec11-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ec11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ec11-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ec11-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ec11-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ec11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ec11-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ec11-116">Not supported.</span></span>|
|<span data-ttu-id="9ec11-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ec11-117">Application</span></span>|<span data-ttu-id="9ec11-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ec11-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ec11-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ec11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9ec11-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ec11-120">Request headers</span></span>
|<span data-ttu-id="9ec11-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ec11-121">Header</span></span>|<span data-ttu-id="9ec11-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9ec11-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ec11-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ec11-123">Authorization</span></span>|<span data-ttu-id="9ec11-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ec11-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ec11-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9ec11-125">Accept</span></span>|<span data-ttu-id="9ec11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ec11-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ec11-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ec11-127">Request body</span></span>
<span data-ttu-id="9ec11-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9ec11-128">In the request body, supply a JSON representation for the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

<span data-ttu-id="9ec11-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ec11-129">The following table shows the properties that are required when you create the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span>

|<span data-ttu-id="9ec11-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ec11-130">Property</span></span>|<span data-ttu-id="9ec11-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ec11-131">Type</span></span>|<span data-ttu-id="9ec11-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ec11-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ec11-133">id</span><span class="sxs-lookup"><span data-stu-id="9ec11-133">id</span></span>|<span data-ttu-id="9ec11-134">String</span><span class="sxs-lookup"><span data-stu-id="9ec11-134">String</span></span>|<span data-ttu-id="9ec11-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9ec11-135">Key of the entity.</span></span> <span data-ttu-id="9ec11-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ec11-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ec11-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ec11-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9ec11-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ec11-138">DateTimeOffset</span></span>|<span data-ttu-id="9ec11-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9ec11-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9ec11-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ec11-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ec11-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ec11-141">roleScopeTagIds</span></span>|<span data-ttu-id="9ec11-142">String collection</span><span class="sxs-lookup"><span data-stu-id="9ec11-142">String collection</span></span>|<span data-ttu-id="9ec11-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="9ec11-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9ec11-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ec11-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ec11-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9ec11-145">supportsScopeTags</span></span>|<span data-ttu-id="9ec11-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ec11-146">Boolean</span></span>|<span data-ttu-id="9ec11-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9ec11-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9ec11-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9ec11-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9ec11-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="9ec11-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9ec11-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ec11-150">This property is read-only.</span></span> <span data-ttu-id="9ec11-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ec11-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ec11-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ec11-152">createdDateTime</span></span>|<span data-ttu-id="9ec11-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ec11-153">DateTimeOffset</span></span>|<span data-ttu-id="9ec11-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9ec11-154">DateTime the object was created.</span></span> <span data-ttu-id="9ec11-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ec11-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ec11-156">description</span><span class="sxs-lookup"><span data-stu-id="9ec11-156">description</span></span>|<span data-ttu-id="9ec11-157">String</span><span class="sxs-lookup"><span data-stu-id="9ec11-157">String</span></span>|<span data-ttu-id="9ec11-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ec11-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9ec11-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ec11-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ec11-160">displayName</span><span class="sxs-lookup"><span data-stu-id="9ec11-160">displayName</span></span>|<span data-ttu-id="9ec11-161">String</span><span class="sxs-lookup"><span data-stu-id="9ec11-161">String</span></span>|<span data-ttu-id="9ec11-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ec11-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9ec11-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ec11-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ec11-164">version</span><span class="sxs-lookup"><span data-stu-id="9ec11-164">version</span></span>|<span data-ttu-id="9ec11-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9ec11-165">Int32</span></span>|<span data-ttu-id="9ec11-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ec11-166">Version of the device configuration.</span></span> <span data-ttu-id="9ec11-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ec11-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ec11-168">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="9ec11-168">preSharedKey</span></span>|<span data-ttu-id="9ec11-169">String</span><span class="sxs-lookup"><span data-stu-id="9ec11-169">String</span></span>|<span data-ttu-id="9ec11-170">Esta é a chave pré compartilhada para rede Wi-Fi WPA Pessoal.</span><span class="sxs-lookup"><span data-stu-id="9ec11-170">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="9ec11-171">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="9ec11-171">wifiSecurityType</span></span>|[<span data-ttu-id="9ec11-172">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="9ec11-172">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="9ec11-173">Especifica o tipo de segurança Wifi.</span><span class="sxs-lookup"><span data-stu-id="9ec11-173">Specify the Wifi Security Type.</span></span> <span data-ttu-id="9ec11-174">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="9ec11-174">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="9ec11-175">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="9ec11-175">meteredConnectionLimit</span></span>|[<span data-ttu-id="9ec11-176">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="9ec11-176">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="9ec11-177">Especifica o tipo de limite de conexão monitorados para a conexão wifi.</span><span class="sxs-lookup"><span data-stu-id="9ec11-177">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="9ec11-178">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="9ec11-178">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="9ec11-179">SSID</span><span class="sxs-lookup"><span data-stu-id="9ec11-179">ssid</span></span>|<span data-ttu-id="9ec11-180">String</span><span class="sxs-lookup"><span data-stu-id="9ec11-180">String</span></span>|<span data-ttu-id="9ec11-181">Especifique o SSID da conexão wifi.</span><span class="sxs-lookup"><span data-stu-id="9ec11-181">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="9ec11-182">networkName</span><span class="sxs-lookup"><span data-stu-id="9ec11-182">networkName</span></span>|<span data-ttu-id="9ec11-183">String</span><span class="sxs-lookup"><span data-stu-id="9ec11-183">String</span></span>|<span data-ttu-id="9ec11-184">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="9ec11-184">Specify the network configuration name.</span></span>|
|<span data-ttu-id="9ec11-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="9ec11-185">connectAutomatically</span></span>|<span data-ttu-id="9ec11-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ec11-186">Boolean</span></span>|<span data-ttu-id="9ec11-187">Especifique se a conexão wifi deve conectar automaticamente quando estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="9ec11-187">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="9ec11-188">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="9ec11-188">connectToPreferredNetwork</span></span>|<span data-ttu-id="9ec11-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ec11-189">Boolean</span></span>|<span data-ttu-id="9ec11-190">Especifique se a conexão wifi deve se conectar às redes mais preferenciais quando já conectado a este.</span><span class="sxs-lookup"><span data-stu-id="9ec11-190">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="9ec11-191">Requer ConnectAutomatically seja true.</span><span class="sxs-lookup"><span data-stu-id="9ec11-191">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="9ec11-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="9ec11-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="9ec11-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ec11-193">Boolean</span></span>|<span data-ttu-id="9ec11-194">Especifique se a conexão wifi deve conectar automaticamente mesmo quando o SSID não está transmitindo.</span><span class="sxs-lookup"><span data-stu-id="9ec11-194">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="9ec11-195">proxySetting</span><span class="sxs-lookup"><span data-stu-id="9ec11-195">proxySetting</span></span>|[<span data-ttu-id="9ec11-196">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="9ec11-196">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="9ec11-197">Especifica a configuração para configuração de Wi-Fi do proxy.</span><span class="sxs-lookup"><span data-stu-id="9ec11-197">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="9ec11-198">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="9ec11-198">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="9ec11-199">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="9ec11-199">proxyManualAddress</span></span>|<span data-ttu-id="9ec11-200">String</span><span class="sxs-lookup"><span data-stu-id="9ec11-200">String</span></span>|<span data-ttu-id="9ec11-201">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="9ec11-201">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="9ec11-202">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="9ec11-202">proxyManualPort</span></span>|<span data-ttu-id="9ec11-203">Int32</span><span class="sxs-lookup"><span data-stu-id="9ec11-203">Int32</span></span>|<span data-ttu-id="9ec11-204">Especifique a porta para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="9ec11-204">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="9ec11-205">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="9ec11-205">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="9ec11-206">String</span><span class="sxs-lookup"><span data-stu-id="9ec11-206">String</span></span>|<span data-ttu-id="9ec11-207">Especifique a URL para o script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="9ec11-207">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="9ec11-208">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="9ec11-208">forceFIPSCompliance</span></span>|<span data-ttu-id="9ec11-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ec11-209">Boolean</span></span>|<span data-ttu-id="9ec11-210">Especifique se deseja forçar a conformidade FIPS.</span><span class="sxs-lookup"><span data-stu-id="9ec11-210">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="9ec11-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ec11-211">Response</span></span>
<span data-ttu-id="9ec11-212">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ec11-212">If successful, this method returns a `200 OK` response code and an updated [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ec11-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ec11-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="9ec11-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ec11-214">Request</span></span>
<span data-ttu-id="9ec11-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ec11-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 787

{
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

### <a name="response"></a><span data-ttu-id="9ec11-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ec11-216">Response</span></span>
<span data-ttu-id="9ec11-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ec11-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





