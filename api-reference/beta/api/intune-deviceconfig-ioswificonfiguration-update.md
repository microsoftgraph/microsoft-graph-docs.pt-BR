---
title: Atualizar iosWiFiConfiguration
description: Atualiza as propriedades de um objeto iosWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f13f24fcc58e43020e0d1272b6b5cb54d46cc8e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32519014"
---
# <a name="update-ioswificonfiguration"></a><span data-ttu-id="e98cd-103">Atualizar iosWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="e98cd-103">Update iosWiFiConfiguration</span></span>

> <span data-ttu-id="e98cd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e98cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e98cd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e98cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e98cd-106">Atualiza as propriedades de um objeto [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e98cd-106">Update the properties of a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e98cd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e98cd-107">Prerequisites</span></span>
<span data-ttu-id="e98cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e98cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e98cd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e98cd-110">Permission type</span></span>|<span data-ttu-id="e98cd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e98cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e98cd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e98cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e98cd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e98cd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e98cd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e98cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e98cd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e98cd-115">Not supported.</span></span>|
|<span data-ttu-id="e98cd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e98cd-116">Application</span></span>|<span data-ttu-id="e98cd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e98cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e98cd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e98cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e98cd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e98cd-119">Request headers</span></span>
|<span data-ttu-id="e98cd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e98cd-120">Header</span></span>|<span data-ttu-id="e98cd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e98cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e98cd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e98cd-122">Authorization</span></span>|<span data-ttu-id="e98cd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e98cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e98cd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e98cd-124">Accept</span></span>|<span data-ttu-id="e98cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e98cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e98cd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e98cd-126">Request body</span></span>
<span data-ttu-id="e98cd-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e98cd-127">In the request body, supply a JSON representation for the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

<span data-ttu-id="e98cd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e98cd-128">The following table shows the properties that are required when you create the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span>

|<span data-ttu-id="e98cd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e98cd-129">Property</span></span>|<span data-ttu-id="e98cd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e98cd-130">Type</span></span>|<span data-ttu-id="e98cd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e98cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e98cd-132">id</span><span class="sxs-lookup"><span data-stu-id="e98cd-132">id</span></span>|<span data-ttu-id="e98cd-133">String</span><span class="sxs-lookup"><span data-stu-id="e98cd-133">String</span></span>|<span data-ttu-id="e98cd-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e98cd-134">Key of the entity.</span></span> <span data-ttu-id="e98cd-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e98cd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e98cd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e98cd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e98cd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e98cd-137">DateTimeOffset</span></span>|<span data-ttu-id="e98cd-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e98cd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e98cd-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e98cd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e98cd-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e98cd-140">roleScopeTagIds</span></span>|<span data-ttu-id="e98cd-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e98cd-141">String collection</span></span>|<span data-ttu-id="e98cd-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="e98cd-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e98cd-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e98cd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e98cd-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e98cd-144">supportsScopeTags</span></span>|<span data-ttu-id="e98cd-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="e98cd-145">Boolean</span></span>|<span data-ttu-id="e98cd-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="e98cd-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e98cd-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="e98cd-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e98cd-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="e98cd-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e98cd-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e98cd-149">This property is read-only.</span></span> <span data-ttu-id="e98cd-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e98cd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e98cd-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e98cd-151">createdDateTime</span></span>|<span data-ttu-id="e98cd-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e98cd-152">DateTimeOffset</span></span>|<span data-ttu-id="e98cd-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e98cd-153">DateTime the object was created.</span></span> <span data-ttu-id="e98cd-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e98cd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e98cd-155">description</span><span class="sxs-lookup"><span data-stu-id="e98cd-155">description</span></span>|<span data-ttu-id="e98cd-156">String</span><span class="sxs-lookup"><span data-stu-id="e98cd-156">String</span></span>|<span data-ttu-id="e98cd-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e98cd-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e98cd-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e98cd-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e98cd-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e98cd-159">displayName</span></span>|<span data-ttu-id="e98cd-160">String</span><span class="sxs-lookup"><span data-stu-id="e98cd-160">String</span></span>|<span data-ttu-id="e98cd-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e98cd-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e98cd-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e98cd-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e98cd-163">versão</span><span class="sxs-lookup"><span data-stu-id="e98cd-163">version</span></span>|<span data-ttu-id="e98cd-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e98cd-164">Int32</span></span>|<span data-ttu-id="e98cd-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e98cd-165">Version of the device configuration.</span></span> <span data-ttu-id="e98cd-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e98cd-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e98cd-167">NetworkName</span><span class="sxs-lookup"><span data-stu-id="e98cd-167">networkName</span></span>|<span data-ttu-id="e98cd-168">String</span><span class="sxs-lookup"><span data-stu-id="e98cd-168">String</span></span>|<span data-ttu-id="e98cd-169">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="e98cd-169">Network Name</span></span>|
|<span data-ttu-id="e98cd-170">SSID</span><span class="sxs-lookup"><span data-stu-id="e98cd-170">ssid</span></span>|<span data-ttu-id="e98cd-171">String</span><span class="sxs-lookup"><span data-stu-id="e98cd-171">String</span></span>|<span data-ttu-id="e98cd-172">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e98cd-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="e98cd-173">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="e98cd-173">connectAutomatically</span></span>|<span data-ttu-id="e98cd-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="e98cd-174">Boolean</span></span>|<span data-ttu-id="e98cd-175">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="e98cd-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="e98cd-176">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e98cd-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="e98cd-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="e98cd-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="e98cd-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="e98cd-178">Boolean</span></span>|<span data-ttu-id="e98cd-179">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="e98cd-179">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="e98cd-180">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e98cd-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="e98cd-181">à</span><span class="sxs-lookup"><span data-stu-id="e98cd-181">wiFiSecurityType</span></span>|[<span data-ttu-id="e98cd-182">à</span><span class="sxs-lookup"><span data-stu-id="e98cd-182">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="e98cd-183">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="e98cd-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="e98cd-184">Os valores possíveis são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="e98cd-184">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="e98cd-185">proxySettings</span><span class="sxs-lookup"><span data-stu-id="e98cd-185">proxySettings</span></span>|[<span data-ttu-id="e98cd-186">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="e98cd-186">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="e98cd-187">Tipo de proxy para esta conexão Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e98cd-187">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="e98cd-188">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="e98cd-188">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="e98cd-189">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="e98cd-189">proxyManualAddress</span></span>|<span data-ttu-id="e98cd-190">String</span><span class="sxs-lookup"><span data-stu-id="e98cd-190">String</span></span>|<span data-ttu-id="e98cd-191">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="e98cd-191">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="e98cd-192">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="e98cd-192">proxyManualPort</span></span>|<span data-ttu-id="e98cd-193">Int32</span><span class="sxs-lookup"><span data-stu-id="e98cd-193">Int32</span></span>|<span data-ttu-id="e98cd-194">Porta do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="e98cd-194">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="e98cd-195">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="e98cd-195">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="e98cd-196">String</span><span class="sxs-lookup"><span data-stu-id="e98cd-196">String</span></span>|<span data-ttu-id="e98cd-197">URL do script de configuração automática do servidor proxy quando a configuração automática estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="e98cd-197">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="e98cd-198">Essa URL normalmente é o local do Arquivo PAC (configuração automática de proxy).</span><span class="sxs-lookup"><span data-stu-id="e98cd-198">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="e98cd-199">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="e98cd-199">preSharedKey</span></span>|<span data-ttu-id="e98cd-200">String</span><span class="sxs-lookup"><span data-stu-id="e98cd-200">String</span></span>|<span data-ttu-id="e98cd-201">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="e98cd-201">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="e98cd-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="e98cd-202">Response</span></span>
<span data-ttu-id="e98cd-203">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e98cd-203">If successful, this method returns a `200 OK` response code and an updated [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e98cd-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e98cd-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="e98cd-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e98cd-205">Request</span></span>
<span data-ttu-id="e98cd-206">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e98cd-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 675

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="e98cd-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="e98cd-207">Response</span></span>
<span data-ttu-id="e98cd-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e98cd-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





