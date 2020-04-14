---
title: Criar macOSWiFiConfiguration
description: Criar um novo objeto macOSWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0bd592f91f25637493e295919cc0bf477518bf5d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432230"
---
# <a name="create-macoswificonfiguration"></a><span data-ttu-id="08d19-103">Criar macOSWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="08d19-103">Create macOSWiFiConfiguration</span></span>

<span data-ttu-id="08d19-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08d19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08d19-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="08d19-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08d19-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08d19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08d19-107">Criar um novo objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="08d19-107">Create a new [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08d19-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="08d19-108">Prerequisites</span></span>
<span data-ttu-id="08d19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08d19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08d19-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08d19-111">Permission type</span></span>|<span data-ttu-id="08d19-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="08d19-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08d19-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08d19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08d19-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08d19-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08d19-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08d19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08d19-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08d19-116">Not supported.</span></span>|
|<span data-ttu-id="08d19-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08d19-117">Application</span></span>|<span data-ttu-id="08d19-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08d19-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08d19-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08d19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="08d19-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08d19-120">Request headers</span></span>
|<span data-ttu-id="08d19-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="08d19-121">Header</span></span>|<span data-ttu-id="08d19-122">Valor</span><span class="sxs-lookup"><span data-stu-id="08d19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08d19-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="08d19-123">Authorization</span></span>|<span data-ttu-id="08d19-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08d19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08d19-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="08d19-125">Accept</span></span>|<span data-ttu-id="08d19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08d19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08d19-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08d19-127">Request body</span></span>
<span data-ttu-id="08d19-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="08d19-128">In the request body, supply a JSON representation for the macOSWiFiConfiguration object.</span></span>

<span data-ttu-id="08d19-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="08d19-129">The following table shows the properties that are required when you create the macOSWiFiConfiguration.</span></span>

|<span data-ttu-id="08d19-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08d19-130">Property</span></span>|<span data-ttu-id="08d19-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="08d19-131">Type</span></span>|<span data-ttu-id="08d19-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="08d19-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08d19-133">id</span><span class="sxs-lookup"><span data-stu-id="08d19-133">id</span></span>|<span data-ttu-id="08d19-134">String</span><span class="sxs-lookup"><span data-stu-id="08d19-134">String</span></span>|<span data-ttu-id="08d19-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="08d19-135">Key of the entity.</span></span> <span data-ttu-id="08d19-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08d19-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08d19-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08d19-137">lastModifiedDateTime</span></span>|<span data-ttu-id="08d19-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08d19-138">DateTimeOffset</span></span>|<span data-ttu-id="08d19-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="08d19-139">DateTime the object was last modified.</span></span> <span data-ttu-id="08d19-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08d19-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08d19-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="08d19-141">roleScopeTagIds</span></span>|<span data-ttu-id="08d19-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="08d19-142">String collection</span></span>|<span data-ttu-id="08d19-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="08d19-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="08d19-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08d19-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08d19-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="08d19-145">supportsScopeTags</span></span>|<span data-ttu-id="08d19-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="08d19-146">Boolean</span></span>|<span data-ttu-id="08d19-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="08d19-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="08d19-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="08d19-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="08d19-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="08d19-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="08d19-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="08d19-150">This property is read-only.</span></span> <span data-ttu-id="08d19-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08d19-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08d19-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="08d19-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="08d19-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="08d19-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="08d19-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="08d19-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="08d19-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08d19-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08d19-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="08d19-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="08d19-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="08d19-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="08d19-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="08d19-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="08d19-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08d19-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08d19-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="08d19-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="08d19-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="08d19-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="08d19-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="08d19-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="08d19-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08d19-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08d19-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08d19-164">createdDateTime</span></span>|<span data-ttu-id="08d19-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08d19-165">DateTimeOffset</span></span>|<span data-ttu-id="08d19-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="08d19-166">DateTime the object was created.</span></span> <span data-ttu-id="08d19-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08d19-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08d19-168">description</span><span class="sxs-lookup"><span data-stu-id="08d19-168">description</span></span>|<span data-ttu-id="08d19-169">String</span><span class="sxs-lookup"><span data-stu-id="08d19-169">String</span></span>|<span data-ttu-id="08d19-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="08d19-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="08d19-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08d19-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08d19-172">displayName</span><span class="sxs-lookup"><span data-stu-id="08d19-172">displayName</span></span>|<span data-ttu-id="08d19-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08d19-173">String</span></span>|<span data-ttu-id="08d19-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="08d19-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="08d19-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08d19-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08d19-176">versão</span><span class="sxs-lookup"><span data-stu-id="08d19-176">version</span></span>|<span data-ttu-id="08d19-177">Int32</span><span class="sxs-lookup"><span data-stu-id="08d19-177">Int32</span></span>|<span data-ttu-id="08d19-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="08d19-178">Version of the device configuration.</span></span> <span data-ttu-id="08d19-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="08d19-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08d19-180">NetworkName</span><span class="sxs-lookup"><span data-stu-id="08d19-180">networkName</span></span>|<span data-ttu-id="08d19-181">String</span><span class="sxs-lookup"><span data-stu-id="08d19-181">String</span></span>|<span data-ttu-id="08d19-182">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="08d19-182">Network Name</span></span>|
|<span data-ttu-id="08d19-183">SSID</span><span class="sxs-lookup"><span data-stu-id="08d19-183">ssid</span></span>|<span data-ttu-id="08d19-184">String</span><span class="sxs-lookup"><span data-stu-id="08d19-184">String</span></span>|<span data-ttu-id="08d19-185">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="08d19-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="08d19-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="08d19-186">connectAutomatically</span></span>|<span data-ttu-id="08d19-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="08d19-187">Boolean</span></span>|<span data-ttu-id="08d19-188">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="08d19-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="08d19-189">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="08d19-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="08d19-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="08d19-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="08d19-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="08d19-191">Boolean</span></span>|<span data-ttu-id="08d19-192">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="08d19-192">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="08d19-193">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="08d19-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="08d19-194">à</span><span class="sxs-lookup"><span data-stu-id="08d19-194">wiFiSecurityType</span></span>|[<span data-ttu-id="08d19-195">à</span><span class="sxs-lookup"><span data-stu-id="08d19-195">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="08d19-196">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="08d19-196">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="08d19-197">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="08d19-197">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="08d19-198">proxySettings</span><span class="sxs-lookup"><span data-stu-id="08d19-198">proxySettings</span></span>|[<span data-ttu-id="08d19-199">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="08d19-199">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="08d19-200">Tipo de proxy para esta conexão Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="08d19-200">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="08d19-201">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="08d19-201">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="08d19-202">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="08d19-202">proxyManualAddress</span></span>|<span data-ttu-id="08d19-203">String</span><span class="sxs-lookup"><span data-stu-id="08d19-203">String</span></span>|<span data-ttu-id="08d19-204">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="08d19-204">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="08d19-205">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="08d19-205">proxyManualPort</span></span>|<span data-ttu-id="08d19-206">Int32</span><span class="sxs-lookup"><span data-stu-id="08d19-206">Int32</span></span>|<span data-ttu-id="08d19-207">Porta do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="08d19-207">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="08d19-208">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="08d19-208">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="08d19-209">String</span><span class="sxs-lookup"><span data-stu-id="08d19-209">String</span></span>|<span data-ttu-id="08d19-210">URL do script de configuração automática do servidor proxy quando a configuração automática estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="08d19-210">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="08d19-211">Essa URL normalmente é o local do Arquivo PAC (configuração automática de proxy).</span><span class="sxs-lookup"><span data-stu-id="08d19-211">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="08d19-212">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="08d19-212">preSharedKey</span></span>|<span data-ttu-id="08d19-213">String</span><span class="sxs-lookup"><span data-stu-id="08d19-213">String</span></span>|<span data-ttu-id="08d19-214">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="08d19-214">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="08d19-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="08d19-215">Response</span></span>
<span data-ttu-id="08d19-216">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08d19-216">If successful, this method returns a `201 Created` response code and a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08d19-217">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08d19-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="08d19-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08d19-218">Request</span></span>
<span data-ttu-id="08d19-219">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08d19-219">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="08d19-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="08d19-220">Response</span></span>
<span data-ttu-id="08d19-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08d19-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



