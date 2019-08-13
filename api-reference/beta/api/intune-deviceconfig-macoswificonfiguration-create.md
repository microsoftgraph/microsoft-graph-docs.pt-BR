---
title: Criar macOSWiFiConfiguration
description: Criar um novo objeto macOSWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: de04b289dd9fe9526890d08be77af14fdb36fdce
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36315075"
---
# <a name="create-macoswificonfiguration"></a><span data-ttu-id="44cc8-103">Criar macOSWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="44cc8-103">Create macOSWiFiConfiguration</span></span>

> <span data-ttu-id="44cc8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="44cc8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44cc8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44cc8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44cc8-106">Criar um novo objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="44cc8-106">Create a new [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44cc8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="44cc8-107">Prerequisites</span></span>
<span data-ttu-id="44cc8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44cc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44cc8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44cc8-110">Permission type</span></span>|<span data-ttu-id="44cc8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="44cc8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44cc8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44cc8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44cc8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44cc8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44cc8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44cc8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44cc8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44cc8-115">Not supported.</span></span>|
|<span data-ttu-id="44cc8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44cc8-116">Application</span></span>|<span data-ttu-id="44cc8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44cc8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44cc8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44cc8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="44cc8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44cc8-119">Request headers</span></span>
|<span data-ttu-id="44cc8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="44cc8-120">Header</span></span>|<span data-ttu-id="44cc8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="44cc8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44cc8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="44cc8-122">Authorization</span></span>|<span data-ttu-id="44cc8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44cc8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44cc8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="44cc8-124">Accept</span></span>|<span data-ttu-id="44cc8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44cc8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44cc8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44cc8-126">Request body</span></span>
<span data-ttu-id="44cc8-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="44cc8-127">In the request body, supply a JSON representation for the macOSWiFiConfiguration object.</span></span>

<span data-ttu-id="44cc8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="44cc8-128">The following table shows the properties that are required when you create the macOSWiFiConfiguration.</span></span>

|<span data-ttu-id="44cc8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44cc8-129">Property</span></span>|<span data-ttu-id="44cc8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="44cc8-130">Type</span></span>|<span data-ttu-id="44cc8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="44cc8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44cc8-132">id</span><span class="sxs-lookup"><span data-stu-id="44cc8-132">id</span></span>|<span data-ttu-id="44cc8-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44cc8-133">String</span></span>|<span data-ttu-id="44cc8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="44cc8-134">Key of the entity.</span></span> <span data-ttu-id="44cc8-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44cc8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44cc8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44cc8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="44cc8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44cc8-137">DateTimeOffset</span></span>|<span data-ttu-id="44cc8-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="44cc8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="44cc8-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44cc8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44cc8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="44cc8-140">roleScopeTagIds</span></span>|<span data-ttu-id="44cc8-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="44cc8-141">String collection</span></span>|<span data-ttu-id="44cc8-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="44cc8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="44cc8-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44cc8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44cc8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="44cc8-144">supportsScopeTags</span></span>|<span data-ttu-id="44cc8-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="44cc8-145">Boolean</span></span>|<span data-ttu-id="44cc8-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="44cc8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="44cc8-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="44cc8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="44cc8-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="44cc8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="44cc8-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44cc8-149">This property is read-only.</span></span> <span data-ttu-id="44cc8-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44cc8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44cc8-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="44cc8-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="44cc8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="44cc8-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="44cc8-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="44cc8-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="44cc8-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44cc8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44cc8-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="44cc8-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="44cc8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="44cc8-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="44cc8-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="44cc8-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="44cc8-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44cc8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44cc8-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="44cc8-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="44cc8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="44cc8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="44cc8-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="44cc8-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="44cc8-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44cc8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44cc8-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44cc8-163">createdDateTime</span></span>|<span data-ttu-id="44cc8-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44cc8-164">DateTimeOffset</span></span>|<span data-ttu-id="44cc8-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="44cc8-165">DateTime the object was created.</span></span> <span data-ttu-id="44cc8-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44cc8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44cc8-167">descrição</span><span class="sxs-lookup"><span data-stu-id="44cc8-167">description</span></span>|<span data-ttu-id="44cc8-168">String</span><span class="sxs-lookup"><span data-stu-id="44cc8-168">String</span></span>|<span data-ttu-id="44cc8-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44cc8-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="44cc8-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44cc8-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44cc8-171">displayName</span><span class="sxs-lookup"><span data-stu-id="44cc8-171">displayName</span></span>|<span data-ttu-id="44cc8-172">String</span><span class="sxs-lookup"><span data-stu-id="44cc8-172">String</span></span>|<span data-ttu-id="44cc8-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44cc8-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="44cc8-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44cc8-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44cc8-175">versão</span><span class="sxs-lookup"><span data-stu-id="44cc8-175">version</span></span>|<span data-ttu-id="44cc8-176">Int32</span><span class="sxs-lookup"><span data-stu-id="44cc8-176">Int32</span></span>|<span data-ttu-id="44cc8-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="44cc8-177">Version of the device configuration.</span></span> <span data-ttu-id="44cc8-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="44cc8-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="44cc8-179">NetworkName</span><span class="sxs-lookup"><span data-stu-id="44cc8-179">networkName</span></span>|<span data-ttu-id="44cc8-180">String</span><span class="sxs-lookup"><span data-stu-id="44cc8-180">String</span></span>|<span data-ttu-id="44cc8-181">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="44cc8-181">Network Name</span></span>|
|<span data-ttu-id="44cc8-182">SSID</span><span class="sxs-lookup"><span data-stu-id="44cc8-182">ssid</span></span>|<span data-ttu-id="44cc8-183">String</span><span class="sxs-lookup"><span data-stu-id="44cc8-183">String</span></span>|<span data-ttu-id="44cc8-184">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="44cc8-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="44cc8-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="44cc8-185">connectAutomatically</span></span>|<span data-ttu-id="44cc8-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="44cc8-186">Boolean</span></span>|<span data-ttu-id="44cc8-187">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="44cc8-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="44cc8-188">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="44cc8-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="44cc8-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="44cc8-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="44cc8-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="44cc8-190">Boolean</span></span>|<span data-ttu-id="44cc8-191">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="44cc8-191">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="44cc8-192">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="44cc8-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="44cc8-193">à</span><span class="sxs-lookup"><span data-stu-id="44cc8-193">wiFiSecurityType</span></span>|[<span data-ttu-id="44cc8-194">à</span><span class="sxs-lookup"><span data-stu-id="44cc8-194">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="44cc8-195">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="44cc8-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="44cc8-196">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="44cc8-196">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="44cc8-197">proxySettings</span><span class="sxs-lookup"><span data-stu-id="44cc8-197">proxySettings</span></span>|[<span data-ttu-id="44cc8-198">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="44cc8-198">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="44cc8-199">Tipo de proxy para esta conexão Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="44cc8-199">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="44cc8-200">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="44cc8-200">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="44cc8-201">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="44cc8-201">proxyManualAddress</span></span>|<span data-ttu-id="44cc8-202">String</span><span class="sxs-lookup"><span data-stu-id="44cc8-202">String</span></span>|<span data-ttu-id="44cc8-203">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="44cc8-203">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="44cc8-204">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="44cc8-204">proxyManualPort</span></span>|<span data-ttu-id="44cc8-205">Int32</span><span class="sxs-lookup"><span data-stu-id="44cc8-205">Int32</span></span>|<span data-ttu-id="44cc8-206">Porta do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="44cc8-206">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="44cc8-207">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="44cc8-207">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="44cc8-208">String</span><span class="sxs-lookup"><span data-stu-id="44cc8-208">String</span></span>|<span data-ttu-id="44cc8-209">URL do script de configuração automática do servidor proxy quando a configuração automática estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="44cc8-209">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="44cc8-210">Essa URL normalmente é o local do Arquivo PAC (configuração automática de proxy).</span><span class="sxs-lookup"><span data-stu-id="44cc8-210">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="44cc8-211">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="44cc8-211">preSharedKey</span></span>|<span data-ttu-id="44cc8-212">String</span><span class="sxs-lookup"><span data-stu-id="44cc8-212">String</span></span>|<span data-ttu-id="44cc8-213">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="44cc8-213">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="44cc8-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="44cc8-214">Response</span></span>
<span data-ttu-id="44cc8-215">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44cc8-215">If successful, this method returns a `201 Created` response code and a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44cc8-216">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44cc8-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="44cc8-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44cc8-217">Request</span></span>
<span data-ttu-id="44cc8-218">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44cc8-218">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1450

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="44cc8-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="44cc8-219">Response</span></span>
<span data-ttu-id="44cc8-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44cc8-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1622

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
  "id": "471203fb-03fb-4712-fb03-1247fb031247",
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






