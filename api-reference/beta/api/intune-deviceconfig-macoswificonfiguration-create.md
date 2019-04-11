---
title: Criar macOSWiFiConfiguration
description: Criar um novo objeto macOSWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37de63ee477e4e72b50ace82aac49c1add1c7613
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804939"
---
# <a name="create-macoswificonfiguration"></a><span data-ttu-id="0b53b-103">Criar macOSWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b53b-103">Create macOSWiFiConfiguration</span></span>

> <span data-ttu-id="0b53b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0b53b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b53b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b53b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b53b-106">Criar um novo objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0b53b-106">Create a new [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b53b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b53b-107">Prerequisites</span></span>
<span data-ttu-id="0b53b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b53b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b53b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b53b-110">Permission type</span></span>|<span data-ttu-id="0b53b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b53b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b53b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b53b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b53b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b53b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b53b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b53b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b53b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b53b-115">Not supported.</span></span>|
|<span data-ttu-id="0b53b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b53b-116">Application</span></span>|<span data-ttu-id="0b53b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b53b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b53b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b53b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0b53b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b53b-119">Request headers</span></span>
|<span data-ttu-id="0b53b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b53b-120">Header</span></span>|<span data-ttu-id="0b53b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0b53b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b53b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b53b-122">Authorization</span></span>|<span data-ttu-id="0b53b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b53b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b53b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0b53b-124">Accept</span></span>|<span data-ttu-id="0b53b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b53b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b53b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b53b-126">Request body</span></span>
<span data-ttu-id="0b53b-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0b53b-127">In the request body, supply a JSON representation for the macOSWiFiConfiguration object.</span></span>

<span data-ttu-id="0b53b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0b53b-128">The following table shows the properties that are required when you create the macOSWiFiConfiguration.</span></span>

|<span data-ttu-id="0b53b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b53b-129">Property</span></span>|<span data-ttu-id="0b53b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b53b-130">Type</span></span>|<span data-ttu-id="0b53b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b53b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b53b-132">id</span><span class="sxs-lookup"><span data-stu-id="0b53b-132">id</span></span>|<span data-ttu-id="0b53b-133">String</span><span class="sxs-lookup"><span data-stu-id="0b53b-133">String</span></span>|<span data-ttu-id="0b53b-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0b53b-134">Key of the entity.</span></span> <span data-ttu-id="0b53b-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b53b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b53b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b53b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0b53b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b53b-137">DateTimeOffset</span></span>|<span data-ttu-id="0b53b-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0b53b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0b53b-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b53b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b53b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0b53b-140">roleScopeTagIds</span></span>|<span data-ttu-id="0b53b-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="0b53b-141">String collection</span></span>|<span data-ttu-id="0b53b-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0b53b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0b53b-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b53b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b53b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0b53b-144">supportsScopeTags</span></span>|<span data-ttu-id="0b53b-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b53b-145">Boolean</span></span>|<span data-ttu-id="0b53b-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0b53b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0b53b-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0b53b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0b53b-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0b53b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0b53b-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b53b-149">This property is read-only.</span></span> <span data-ttu-id="0b53b-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b53b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b53b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b53b-151">createdDateTime</span></span>|<span data-ttu-id="0b53b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b53b-152">DateTimeOffset</span></span>|<span data-ttu-id="0b53b-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0b53b-153">DateTime the object was created.</span></span> <span data-ttu-id="0b53b-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b53b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b53b-155">description</span><span class="sxs-lookup"><span data-stu-id="0b53b-155">description</span></span>|<span data-ttu-id="0b53b-156">String</span><span class="sxs-lookup"><span data-stu-id="0b53b-156">String</span></span>|<span data-ttu-id="0b53b-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b53b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0b53b-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b53b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b53b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0b53b-159">displayName</span></span>|<span data-ttu-id="0b53b-160">String</span><span class="sxs-lookup"><span data-stu-id="0b53b-160">String</span></span>|<span data-ttu-id="0b53b-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b53b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0b53b-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b53b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b53b-163">versão</span><span class="sxs-lookup"><span data-stu-id="0b53b-163">version</span></span>|<span data-ttu-id="0b53b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0b53b-164">Int32</span></span>|<span data-ttu-id="0b53b-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b53b-165">Version of the device configuration.</span></span> <span data-ttu-id="0b53b-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b53b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b53b-167">NetworkName</span><span class="sxs-lookup"><span data-stu-id="0b53b-167">networkName</span></span>|<span data-ttu-id="0b53b-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b53b-168">String</span></span>|<span data-ttu-id="0b53b-169">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="0b53b-169">Network Name</span></span>|
|<span data-ttu-id="0b53b-170">SSID</span><span class="sxs-lookup"><span data-stu-id="0b53b-170">ssid</span></span>|<span data-ttu-id="0b53b-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b53b-171">String</span></span>|<span data-ttu-id="0b53b-172">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0b53b-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="0b53b-173">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="0b53b-173">connectAutomatically</span></span>|<span data-ttu-id="0b53b-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b53b-174">Boolean</span></span>|<span data-ttu-id="0b53b-175">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="0b53b-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="0b53b-176">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="0b53b-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="0b53b-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="0b53b-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="0b53b-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b53b-178">Boolean</span></span>|<span data-ttu-id="0b53b-179">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="0b53b-179">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="0b53b-180">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0b53b-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="0b53b-181">à</span><span class="sxs-lookup"><span data-stu-id="0b53b-181">wiFiSecurityType</span></span>|[<span data-ttu-id="0b53b-182">à</span><span class="sxs-lookup"><span data-stu-id="0b53b-182">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="0b53b-183">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="0b53b-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="0b53b-184">Os valores possíveis são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="0b53b-184">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="0b53b-185">proxySettings</span><span class="sxs-lookup"><span data-stu-id="0b53b-185">proxySettings</span></span>|[<span data-ttu-id="0b53b-186">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="0b53b-186">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="0b53b-187">Tipo de proxy para esta conexão Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="0b53b-187">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="0b53b-188">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="0b53b-188">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="0b53b-189">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="0b53b-189">proxyManualAddress</span></span>|<span data-ttu-id="0b53b-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b53b-190">String</span></span>|<span data-ttu-id="0b53b-191">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="0b53b-191">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="0b53b-192">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="0b53b-192">proxyManualPort</span></span>|<span data-ttu-id="0b53b-193">Int32</span><span class="sxs-lookup"><span data-stu-id="0b53b-193">Int32</span></span>|<span data-ttu-id="0b53b-194">Porta do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="0b53b-194">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="0b53b-195">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="0b53b-195">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="0b53b-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b53b-196">String</span></span>|<span data-ttu-id="0b53b-197">URL do script de configuração automática do servidor proxy quando a configuração automática estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="0b53b-197">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="0b53b-198">Essa URL normalmente é o local do Arquivo PAC (configuração automática de proxy).</span><span class="sxs-lookup"><span data-stu-id="0b53b-198">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="0b53b-199">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="0b53b-199">preSharedKey</span></span>|<span data-ttu-id="0b53b-200">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b53b-200">String</span></span>|<span data-ttu-id="0b53b-201">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="0b53b-201">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="0b53b-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b53b-202">Response</span></span>
<span data-ttu-id="0b53b-203">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b53b-203">If successful, this method returns a `201 Created` response code and a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b53b-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b53b-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b53b-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b53b-205">Request</span></span>
<span data-ttu-id="0b53b-206">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b53b-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 677

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="0b53b-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b53b-207">Response</span></span>
<span data-ttu-id="0b53b-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b53b-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 849

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
  "id": "471203fb-03fb-4712-fb03-1247fb031247",
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





