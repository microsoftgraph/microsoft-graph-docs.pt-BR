---
title: Atualizar iosWiFiConfiguration
description: Atualize as propriedades de um objeto iosWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f65b8f98b12ed3aa8c5caa96afc9b850dd70071f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847534"
---
# <a name="update-ioswificonfiguration"></a><span data-ttu-id="31aba-103">Atualizar iosWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="31aba-103">Update iosWiFiConfiguration</span></span>

> <span data-ttu-id="31aba-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="31aba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31aba-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="31aba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31aba-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="31aba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31aba-107">Atualize as propriedades de um objeto [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="31aba-107">Update the properties of a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="31aba-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="31aba-108">Prerequisites</span></span>
<span data-ttu-id="31aba-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31aba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31aba-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31aba-111">Permission type</span></span>|<span data-ttu-id="31aba-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="31aba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31aba-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31aba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31aba-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31aba-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="31aba-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31aba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31aba-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31aba-116">Not supported.</span></span>|
|<span data-ttu-id="31aba-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31aba-117">Application</span></span>|<span data-ttu-id="31aba-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31aba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31aba-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31aba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="31aba-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31aba-120">Request headers</span></span>
|<span data-ttu-id="31aba-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31aba-121">Header</span></span>|<span data-ttu-id="31aba-122">Valor</span><span class="sxs-lookup"><span data-stu-id="31aba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31aba-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="31aba-123">Authorization</span></span>|<span data-ttu-id="31aba-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31aba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31aba-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="31aba-125">Accept</span></span>|<span data-ttu-id="31aba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31aba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31aba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31aba-127">Request body</span></span>
<span data-ttu-id="31aba-128">No corpo da solicitação, fornece uma representação JSON para o objeto [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="31aba-128">In the request body, supply a JSON representation for the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

<span data-ttu-id="31aba-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31aba-129">The following table shows the properties that are required when you create the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span>

|<span data-ttu-id="31aba-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31aba-130">Property</span></span>|<span data-ttu-id="31aba-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="31aba-131">Type</span></span>|<span data-ttu-id="31aba-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="31aba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31aba-133">id</span><span class="sxs-lookup"><span data-stu-id="31aba-133">id</span></span>|<span data-ttu-id="31aba-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31aba-134">String</span></span>|<span data-ttu-id="31aba-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="31aba-135">Key of the entity.</span></span> <span data-ttu-id="31aba-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31aba-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31aba-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31aba-137">lastModifiedDateTime</span></span>|<span data-ttu-id="31aba-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31aba-138">DateTimeOffset</span></span>|<span data-ttu-id="31aba-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="31aba-139">DateTime the object was last modified.</span></span> <span data-ttu-id="31aba-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31aba-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31aba-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="31aba-141">roleScopeTagIds</span></span>|<span data-ttu-id="31aba-142">String collection</span><span class="sxs-lookup"><span data-stu-id="31aba-142">String collection</span></span>|<span data-ttu-id="31aba-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="31aba-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="31aba-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31aba-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31aba-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="31aba-145">supportsScopeTags</span></span>|<span data-ttu-id="31aba-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="31aba-146">Boolean</span></span>|<span data-ttu-id="31aba-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="31aba-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="31aba-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="31aba-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="31aba-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="31aba-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="31aba-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31aba-150">This property is read-only.</span></span> <span data-ttu-id="31aba-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31aba-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31aba-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31aba-152">createdDateTime</span></span>|<span data-ttu-id="31aba-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31aba-153">DateTimeOffset</span></span>|<span data-ttu-id="31aba-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="31aba-154">DateTime the object was created.</span></span> <span data-ttu-id="31aba-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31aba-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31aba-156">description</span><span class="sxs-lookup"><span data-stu-id="31aba-156">description</span></span>|<span data-ttu-id="31aba-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31aba-157">String</span></span>|<span data-ttu-id="31aba-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31aba-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="31aba-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31aba-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31aba-160">displayName</span><span class="sxs-lookup"><span data-stu-id="31aba-160">displayName</span></span>|<span data-ttu-id="31aba-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31aba-161">String</span></span>|<span data-ttu-id="31aba-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31aba-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="31aba-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31aba-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31aba-164">version</span><span class="sxs-lookup"><span data-stu-id="31aba-164">version</span></span>|<span data-ttu-id="31aba-165">Int32</span><span class="sxs-lookup"><span data-stu-id="31aba-165">Int32</span></span>|<span data-ttu-id="31aba-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31aba-166">Version of the device configuration.</span></span> <span data-ttu-id="31aba-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31aba-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31aba-168">networkName</span><span class="sxs-lookup"><span data-stu-id="31aba-168">networkName</span></span>|<span data-ttu-id="31aba-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31aba-169">String</span></span>|<span data-ttu-id="31aba-170">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="31aba-170">Network Name</span></span>|
|<span data-ttu-id="31aba-171">SSID</span><span class="sxs-lookup"><span data-stu-id="31aba-171">ssid</span></span>|<span data-ttu-id="31aba-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31aba-172">String</span></span>|<span data-ttu-id="31aba-173">Este é o nome da rede Wi-Fi que é difundido para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="31aba-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="31aba-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="31aba-174">connectAutomatically</span></span>|<span data-ttu-id="31aba-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="31aba-175">Boolean</span></span>|<span data-ttu-id="31aba-176">Conecte automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="31aba-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="31aba-177">Essa configuração como true ignorar o prompt do usuário e se conecte automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="31aba-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="31aba-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="31aba-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="31aba-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="31aba-179">Boolean</span></span>|<span data-ttu-id="31aba-180">Conecte-se quando a rede não está transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="31aba-180">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="31aba-181">Quando definido como true, esse perfil força o dispositivo para se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="31aba-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="31aba-182">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="31aba-182">wiFiSecurityType</span></span>|[<span data-ttu-id="31aba-183">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="31aba-183">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="31aba-184">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseada em EAP.</span><span class="sxs-lookup"><span data-stu-id="31aba-184">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="31aba-185">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="31aba-185">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="31aba-186">proxySettings</span><span class="sxs-lookup"><span data-stu-id="31aba-186">proxySettings</span></span>|[<span data-ttu-id="31aba-187">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="31aba-187">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="31aba-188">Tipo de proxy para esta conexão Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="31aba-188">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="31aba-189">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="31aba-189">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="31aba-190">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="31aba-190">proxyManualAddress</span></span>|<span data-ttu-id="31aba-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31aba-191">String</span></span>|<span data-ttu-id="31aba-192">Nome de host DNS ou endereço IP do servidor proxy quando a configuração manual está selecionada.</span><span class="sxs-lookup"><span data-stu-id="31aba-192">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="31aba-193">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="31aba-193">proxyManualPort</span></span>|<span data-ttu-id="31aba-194">Int32</span><span class="sxs-lookup"><span data-stu-id="31aba-194">Int32</span></span>|<span data-ttu-id="31aba-195">Porta do servidor proxy quando a configuração manual está selecionada.</span><span class="sxs-lookup"><span data-stu-id="31aba-195">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="31aba-196">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="31aba-196">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="31aba-197">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31aba-197">String</span></span>|<span data-ttu-id="31aba-198">URL do script de configuração automática do servidor proxy quando a configuração automática é selecionada.</span><span class="sxs-lookup"><span data-stu-id="31aba-198">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="31aba-199">Essa URL normalmente é o local do arquivo PAC (configuração automática de Proxy).</span><span class="sxs-lookup"><span data-stu-id="31aba-199">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="31aba-200">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="31aba-200">preSharedKey</span></span>|<span data-ttu-id="31aba-201">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31aba-201">String</span></span>|<span data-ttu-id="31aba-202">Esta é a chave pré compartilhada para rede Wi-Fi WPA Pessoal.</span><span class="sxs-lookup"><span data-stu-id="31aba-202">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="31aba-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="31aba-203">Response</span></span>
<span data-ttu-id="31aba-204">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31aba-204">If successful, this method returns a `200 OK` response code and an updated [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31aba-205">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31aba-205">Example</span></span>
### <a name="request"></a><span data-ttu-id="31aba-206">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31aba-206">Request</span></span>
<span data-ttu-id="31aba-207">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31aba-207">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 680

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="31aba-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="31aba-208">Response</span></span>
<span data-ttu-id="31aba-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31aba-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 847

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
  "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value"
}
```





