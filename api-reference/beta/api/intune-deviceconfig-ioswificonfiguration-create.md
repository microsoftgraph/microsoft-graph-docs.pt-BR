---
title: Criar iosWiFiConfiguration
description: Criar um novo objeto iosWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b02a524b6f94731833deef1c1ac69b59e90a208
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977027"
---
# <a name="create-ioswificonfiguration"></a><span data-ttu-id="cc053-103">Criar iosWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="cc053-103">Create iosWiFiConfiguration</span></span>

> <span data-ttu-id="cc053-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cc053-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc053-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cc053-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc053-106">Criar um novo objeto [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="cc053-106">Create a new [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc053-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cc053-107">Prerequisites</span></span>
<span data-ttu-id="cc053-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc053-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc053-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc053-110">Permission type</span></span>|<span data-ttu-id="cc053-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cc053-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc053-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc053-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc053-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc053-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc053-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc053-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc053-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc053-115">Not supported.</span></span>|
|<span data-ttu-id="cc053-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc053-116">Application</span></span>|<span data-ttu-id="cc053-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc053-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc053-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc053-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cc053-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc053-119">Request headers</span></span>
|<span data-ttu-id="cc053-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc053-120">Header</span></span>|<span data-ttu-id="cc053-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cc053-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc053-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc053-122">Authorization</span></span>|<span data-ttu-id="cc053-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc053-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc053-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cc053-124">Accept</span></span>|<span data-ttu-id="cc053-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cc053-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc053-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc053-126">Request body</span></span>
<span data-ttu-id="cc053-127">No corpo da solicitação, forneça uma representação JSON do objeto iosWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cc053-127">In the request body, supply a JSON representation for the iosWiFiConfiguration object.</span></span>

<span data-ttu-id="cc053-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="cc053-128">The following table shows the properties that are required when you create the iosWiFiConfiguration.</span></span>

|<span data-ttu-id="cc053-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc053-129">Property</span></span>|<span data-ttu-id="cc053-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc053-130">Type</span></span>|<span data-ttu-id="cc053-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc053-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc053-132">id</span><span class="sxs-lookup"><span data-stu-id="cc053-132">id</span></span>|<span data-ttu-id="cc053-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc053-133">String</span></span>|<span data-ttu-id="cc053-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cc053-134">Key of the entity.</span></span> <span data-ttu-id="cc053-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc053-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc053-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc053-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cc053-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc053-137">DateTimeOffset</span></span>|<span data-ttu-id="cc053-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="cc053-138">DateTime the object was last modified.</span></span> <span data-ttu-id="cc053-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc053-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc053-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cc053-140">roleScopeTagIds</span></span>|<span data-ttu-id="cc053-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc053-141">String collection</span></span>|<span data-ttu-id="cc053-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="cc053-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cc053-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc053-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc053-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="cc053-144">supportsScopeTags</span></span>|<span data-ttu-id="cc053-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="cc053-145">Boolean</span></span>|<span data-ttu-id="cc053-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="cc053-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cc053-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="cc053-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cc053-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="cc053-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cc053-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc053-149">This property is read-only.</span></span> <span data-ttu-id="cc053-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc053-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc053-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cc053-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="cc053-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cc053-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="cc053-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="cc053-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="cc053-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc053-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc053-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cc053-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="cc053-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cc053-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="cc053-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="cc053-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="cc053-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc053-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc053-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="cc053-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="cc053-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="cc053-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="cc053-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="cc053-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="cc053-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc053-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc053-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc053-163">createdDateTime</span></span>|<span data-ttu-id="cc053-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc053-164">DateTimeOffset</span></span>|<span data-ttu-id="cc053-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="cc053-165">DateTime the object was created.</span></span> <span data-ttu-id="cc053-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc053-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc053-167">descrição</span><span class="sxs-lookup"><span data-stu-id="cc053-167">description</span></span>|<span data-ttu-id="cc053-168">String</span><span class="sxs-lookup"><span data-stu-id="cc053-168">String</span></span>|<span data-ttu-id="cc053-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cc053-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cc053-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc053-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc053-171">displayName</span><span class="sxs-lookup"><span data-stu-id="cc053-171">displayName</span></span>|<span data-ttu-id="cc053-172">String</span><span class="sxs-lookup"><span data-stu-id="cc053-172">String</span></span>|<span data-ttu-id="cc053-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cc053-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cc053-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc053-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc053-175">versão</span><span class="sxs-lookup"><span data-stu-id="cc053-175">version</span></span>|<span data-ttu-id="cc053-176">Int32</span><span class="sxs-lookup"><span data-stu-id="cc053-176">Int32</span></span>|<span data-ttu-id="cc053-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cc053-177">Version of the device configuration.</span></span> <span data-ttu-id="cc053-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc053-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cc053-179">NetworkName</span><span class="sxs-lookup"><span data-stu-id="cc053-179">networkName</span></span>|<span data-ttu-id="cc053-180">String</span><span class="sxs-lookup"><span data-stu-id="cc053-180">String</span></span>|<span data-ttu-id="cc053-181">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="cc053-181">Network Name</span></span>|
|<span data-ttu-id="cc053-182">SSID</span><span class="sxs-lookup"><span data-stu-id="cc053-182">ssid</span></span>|<span data-ttu-id="cc053-183">String</span><span class="sxs-lookup"><span data-stu-id="cc053-183">String</span></span>|<span data-ttu-id="cc053-184">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="cc053-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="cc053-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="cc053-185">connectAutomatically</span></span>|<span data-ttu-id="cc053-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="cc053-186">Boolean</span></span>|<span data-ttu-id="cc053-187">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="cc053-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="cc053-188">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="cc053-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="cc053-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="cc053-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="cc053-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="cc053-190">Boolean</span></span>|<span data-ttu-id="cc053-191">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="cc053-191">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="cc053-192">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="cc053-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="cc053-193">à</span><span class="sxs-lookup"><span data-stu-id="cc053-193">wiFiSecurityType</span></span>|[<span data-ttu-id="cc053-194">à</span><span class="sxs-lookup"><span data-stu-id="cc053-194">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="cc053-195">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="cc053-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="cc053-196">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="cc053-196">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="cc053-197">proxySettings</span><span class="sxs-lookup"><span data-stu-id="cc053-197">proxySettings</span></span>|[<span data-ttu-id="cc053-198">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="cc053-198">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="cc053-199">Tipo de proxy para esta conexão Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="cc053-199">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="cc053-200">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="cc053-200">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="cc053-201">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="cc053-201">proxyManualAddress</span></span>|<span data-ttu-id="cc053-202">String</span><span class="sxs-lookup"><span data-stu-id="cc053-202">String</span></span>|<span data-ttu-id="cc053-203">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="cc053-203">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="cc053-204">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="cc053-204">proxyManualPort</span></span>|<span data-ttu-id="cc053-205">Int32</span><span class="sxs-lookup"><span data-stu-id="cc053-205">Int32</span></span>|<span data-ttu-id="cc053-206">Porta do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="cc053-206">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="cc053-207">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="cc053-207">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="cc053-208">String</span><span class="sxs-lookup"><span data-stu-id="cc053-208">String</span></span>|<span data-ttu-id="cc053-209">URL do script de configuração automática do servidor proxy quando a configuração automática estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="cc053-209">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="cc053-210">Essa URL normalmente é o local do Arquivo PAC (configuração automática de proxy).</span><span class="sxs-lookup"><span data-stu-id="cc053-210">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="cc053-211">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="cc053-211">preSharedKey</span></span>|<span data-ttu-id="cc053-212">String</span><span class="sxs-lookup"><span data-stu-id="cc053-212">String</span></span>|<span data-ttu-id="cc053-213">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="cc053-213">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="cc053-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc053-214">Response</span></span>
<span data-ttu-id="cc053-215">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc053-215">If successful, this method returns a `201 Created` response code and a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc053-216">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc053-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc053-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc053-217">Request</span></span>
<span data-ttu-id="cc053-218">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc053-218">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1448

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="cc053-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc053-219">Response</span></span>
<span data-ttu-id="cc053-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc053-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1620

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
  "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
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





