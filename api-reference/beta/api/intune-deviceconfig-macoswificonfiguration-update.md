---
title: Atualizar macOSWiFiConfiguration
description: Atualiza as propriedades de um objeto macOSWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ba82df6f6f709fa5066e57f5fb107f0f45c4a0c0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518230"
---
# <a name="update-macoswificonfiguration"></a><span data-ttu-id="a97a0-103">Atualizar macOSWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="a97a0-103">Update macOSWiFiConfiguration</span></span>

> <span data-ttu-id="a97a0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a97a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a97a0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a97a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a97a0-106">Atualiza as propriedades de um objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a97a0-106">Update the properties of a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a97a0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a97a0-107">Prerequisites</span></span>
<span data-ttu-id="a97a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a97a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a97a0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a97a0-110">Permission type</span></span>|<span data-ttu-id="a97a0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a97a0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a97a0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a97a0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a97a0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a97a0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a97a0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a97a0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a97a0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a97a0-115">Not supported.</span></span>|
|<span data-ttu-id="a97a0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a97a0-116">Application</span></span>|<span data-ttu-id="a97a0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a97a0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a97a0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a97a0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a97a0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a97a0-119">Request headers</span></span>
|<span data-ttu-id="a97a0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a97a0-120">Header</span></span>|<span data-ttu-id="a97a0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a97a0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a97a0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a97a0-122">Authorization</span></span>|<span data-ttu-id="a97a0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a97a0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a97a0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a97a0-124">Accept</span></span>|<span data-ttu-id="a97a0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a97a0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a97a0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a97a0-126">Request body</span></span>
<span data-ttu-id="a97a0-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a97a0-127">In the request body, supply a JSON representation for the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

<span data-ttu-id="a97a0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a97a0-128">The following table shows the properties that are required when you create the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span>

|<span data-ttu-id="a97a0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a97a0-129">Property</span></span>|<span data-ttu-id="a97a0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a97a0-130">Type</span></span>|<span data-ttu-id="a97a0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a97a0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a97a0-132">id</span><span class="sxs-lookup"><span data-stu-id="a97a0-132">id</span></span>|<span data-ttu-id="a97a0-133">String</span><span class="sxs-lookup"><span data-stu-id="a97a0-133">String</span></span>|<span data-ttu-id="a97a0-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a97a0-134">Key of the entity.</span></span> <span data-ttu-id="a97a0-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a97a0-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a97a0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a97a0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a97a0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a97a0-137">DateTimeOffset</span></span>|<span data-ttu-id="a97a0-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a97a0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a97a0-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a97a0-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a97a0-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a97a0-140">roleScopeTagIds</span></span>|<span data-ttu-id="a97a0-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a97a0-141">String collection</span></span>|<span data-ttu-id="a97a0-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a97a0-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a97a0-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a97a0-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a97a0-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a97a0-144">supportsScopeTags</span></span>|<span data-ttu-id="a97a0-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="a97a0-145">Boolean</span></span>|<span data-ttu-id="a97a0-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a97a0-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a97a0-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a97a0-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a97a0-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a97a0-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a97a0-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a97a0-149">This property is read-only.</span></span> <span data-ttu-id="a97a0-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a97a0-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a97a0-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a97a0-151">createdDateTime</span></span>|<span data-ttu-id="a97a0-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a97a0-152">DateTimeOffset</span></span>|<span data-ttu-id="a97a0-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a97a0-153">DateTime the object was created.</span></span> <span data-ttu-id="a97a0-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a97a0-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a97a0-155">description</span><span class="sxs-lookup"><span data-stu-id="a97a0-155">description</span></span>|<span data-ttu-id="a97a0-156">String</span><span class="sxs-lookup"><span data-stu-id="a97a0-156">String</span></span>|<span data-ttu-id="a97a0-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a97a0-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a97a0-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a97a0-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a97a0-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a97a0-159">displayName</span></span>|<span data-ttu-id="a97a0-160">String</span><span class="sxs-lookup"><span data-stu-id="a97a0-160">String</span></span>|<span data-ttu-id="a97a0-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a97a0-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a97a0-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a97a0-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a97a0-163">versão</span><span class="sxs-lookup"><span data-stu-id="a97a0-163">version</span></span>|<span data-ttu-id="a97a0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a97a0-164">Int32</span></span>|<span data-ttu-id="a97a0-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a97a0-165">Version of the device configuration.</span></span> <span data-ttu-id="a97a0-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a97a0-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a97a0-167">NetworkName</span><span class="sxs-lookup"><span data-stu-id="a97a0-167">networkName</span></span>|<span data-ttu-id="a97a0-168">String</span><span class="sxs-lookup"><span data-stu-id="a97a0-168">String</span></span>|<span data-ttu-id="a97a0-169">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="a97a0-169">Network Name</span></span>|
|<span data-ttu-id="a97a0-170">SSID</span><span class="sxs-lookup"><span data-stu-id="a97a0-170">ssid</span></span>|<span data-ttu-id="a97a0-171">String</span><span class="sxs-lookup"><span data-stu-id="a97a0-171">String</span></span>|<span data-ttu-id="a97a0-172">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a97a0-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="a97a0-173">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="a97a0-173">connectAutomatically</span></span>|<span data-ttu-id="a97a0-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="a97a0-174">Boolean</span></span>|<span data-ttu-id="a97a0-175">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="a97a0-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="a97a0-176">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="a97a0-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="a97a0-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="a97a0-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="a97a0-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="a97a0-178">Boolean</span></span>|<span data-ttu-id="a97a0-179">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="a97a0-179">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="a97a0-180">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a97a0-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="a97a0-181">à</span><span class="sxs-lookup"><span data-stu-id="a97a0-181">wiFiSecurityType</span></span>|[<span data-ttu-id="a97a0-182">à</span><span class="sxs-lookup"><span data-stu-id="a97a0-182">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="a97a0-183">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="a97a0-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="a97a0-184">Os valores possíveis são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="a97a0-184">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="a97a0-185">proxySettings</span><span class="sxs-lookup"><span data-stu-id="a97a0-185">proxySettings</span></span>|[<span data-ttu-id="a97a0-186">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="a97a0-186">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="a97a0-187">Tipo de proxy para esta conexão Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="a97a0-187">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="a97a0-188">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="a97a0-188">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="a97a0-189">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="a97a0-189">proxyManualAddress</span></span>|<span data-ttu-id="a97a0-190">String</span><span class="sxs-lookup"><span data-stu-id="a97a0-190">String</span></span>|<span data-ttu-id="a97a0-191">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="a97a0-191">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="a97a0-192">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="a97a0-192">proxyManualPort</span></span>|<span data-ttu-id="a97a0-193">Int32</span><span class="sxs-lookup"><span data-stu-id="a97a0-193">Int32</span></span>|<span data-ttu-id="a97a0-194">Porta do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="a97a0-194">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="a97a0-195">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="a97a0-195">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="a97a0-196">String</span><span class="sxs-lookup"><span data-stu-id="a97a0-196">String</span></span>|<span data-ttu-id="a97a0-197">URL do script de configuração automática do servidor proxy quando a configuração automática estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="a97a0-197">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="a97a0-198">Essa URL normalmente é o local do Arquivo PAC (configuração automática de proxy).</span><span class="sxs-lookup"><span data-stu-id="a97a0-198">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="a97a0-199">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="a97a0-199">preSharedKey</span></span>|<span data-ttu-id="a97a0-200">String</span><span class="sxs-lookup"><span data-stu-id="a97a0-200">String</span></span>|<span data-ttu-id="a97a0-201">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="a97a0-201">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="a97a0-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="a97a0-202">Response</span></span>
<span data-ttu-id="a97a0-203">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a97a0-203">If successful, this method returns a `200 OK` response code and an updated [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a97a0-204">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a97a0-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="a97a0-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a97a0-205">Request</span></span>
<span data-ttu-id="a97a0-206">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a97a0-206">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="a97a0-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="a97a0-207">Response</span></span>
<span data-ttu-id="a97a0-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a97a0-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





