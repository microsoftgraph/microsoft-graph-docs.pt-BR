---
title: Atualizar macOSWiFiConfiguration
description: Atualiza as propriedades de um objeto macOSWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3de269d43e4f7cf5ce907a27bb14abbb64d2cfbd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35946847"
---
# <a name="update-macoswificonfiguration"></a><span data-ttu-id="65f86-103">Atualizar macOSWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="65f86-103">Update macOSWiFiConfiguration</span></span>

> <span data-ttu-id="65f86-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="65f86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65f86-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65f86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65f86-106">Atualiza as propriedades de um objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="65f86-106">Update the properties of a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65f86-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="65f86-107">Prerequisites</span></span>
<span data-ttu-id="65f86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65f86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65f86-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65f86-110">Permission type</span></span>|<span data-ttu-id="65f86-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="65f86-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65f86-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65f86-112">Delegated (work or school account)</span></span>|<span data-ttu-id="65f86-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65f86-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65f86-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65f86-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65f86-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65f86-115">Not supported.</span></span>|
|<span data-ttu-id="65f86-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65f86-116">Application</span></span>|<span data-ttu-id="65f86-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65f86-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65f86-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65f86-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="65f86-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65f86-119">Request headers</span></span>
|<span data-ttu-id="65f86-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="65f86-120">Header</span></span>|<span data-ttu-id="65f86-121">Valor</span><span class="sxs-lookup"><span data-stu-id="65f86-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65f86-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="65f86-122">Authorization</span></span>|<span data-ttu-id="65f86-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65f86-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65f86-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="65f86-124">Accept</span></span>|<span data-ttu-id="65f86-125">application/json</span><span class="sxs-lookup"><span data-stu-id="65f86-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65f86-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65f86-126">Request body</span></span>
<span data-ttu-id="65f86-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="65f86-127">In the request body, supply a JSON representation for the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

<span data-ttu-id="65f86-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65f86-128">The following table shows the properties that are required when you create the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span>

|<span data-ttu-id="65f86-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65f86-129">Property</span></span>|<span data-ttu-id="65f86-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="65f86-130">Type</span></span>|<span data-ttu-id="65f86-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="65f86-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65f86-132">id</span><span class="sxs-lookup"><span data-stu-id="65f86-132">id</span></span>|<span data-ttu-id="65f86-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65f86-133">String</span></span>|<span data-ttu-id="65f86-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="65f86-134">Key of the entity.</span></span> <span data-ttu-id="65f86-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f86-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f86-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65f86-136">lastModifiedDateTime</span></span>|<span data-ttu-id="65f86-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65f86-137">DateTimeOffset</span></span>|<span data-ttu-id="65f86-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="65f86-138">DateTime the object was last modified.</span></span> <span data-ttu-id="65f86-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f86-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f86-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="65f86-140">roleScopeTagIds</span></span>|<span data-ttu-id="65f86-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="65f86-141">String collection</span></span>|<span data-ttu-id="65f86-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="65f86-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="65f86-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f86-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f86-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="65f86-144">supportsScopeTags</span></span>|<span data-ttu-id="65f86-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="65f86-145">Boolean</span></span>|<span data-ttu-id="65f86-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="65f86-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="65f86-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="65f86-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="65f86-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="65f86-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="65f86-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="65f86-149">This property is read-only.</span></span> <span data-ttu-id="65f86-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f86-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f86-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="65f86-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="65f86-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="65f86-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="65f86-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="65f86-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="65f86-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f86-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f86-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="65f86-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="65f86-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="65f86-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="65f86-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="65f86-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="65f86-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f86-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f86-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="65f86-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="65f86-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="65f86-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="65f86-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="65f86-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="65f86-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f86-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f86-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65f86-163">createdDateTime</span></span>|<span data-ttu-id="65f86-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65f86-164">DateTimeOffset</span></span>|<span data-ttu-id="65f86-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="65f86-165">DateTime the object was created.</span></span> <span data-ttu-id="65f86-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f86-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f86-167">descrição</span><span class="sxs-lookup"><span data-stu-id="65f86-167">description</span></span>|<span data-ttu-id="65f86-168">String</span><span class="sxs-lookup"><span data-stu-id="65f86-168">String</span></span>|<span data-ttu-id="65f86-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="65f86-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="65f86-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f86-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f86-171">displayName</span><span class="sxs-lookup"><span data-stu-id="65f86-171">displayName</span></span>|<span data-ttu-id="65f86-172">String</span><span class="sxs-lookup"><span data-stu-id="65f86-172">String</span></span>|<span data-ttu-id="65f86-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="65f86-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="65f86-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f86-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f86-175">versão</span><span class="sxs-lookup"><span data-stu-id="65f86-175">version</span></span>|<span data-ttu-id="65f86-176">Int32</span><span class="sxs-lookup"><span data-stu-id="65f86-176">Int32</span></span>|<span data-ttu-id="65f86-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="65f86-177">Version of the device configuration.</span></span> <span data-ttu-id="65f86-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f86-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f86-179">NetworkName</span><span class="sxs-lookup"><span data-stu-id="65f86-179">networkName</span></span>|<span data-ttu-id="65f86-180">String</span><span class="sxs-lookup"><span data-stu-id="65f86-180">String</span></span>|<span data-ttu-id="65f86-181">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="65f86-181">Network Name</span></span>|
|<span data-ttu-id="65f86-182">SSID</span><span class="sxs-lookup"><span data-stu-id="65f86-182">ssid</span></span>|<span data-ttu-id="65f86-183">String</span><span class="sxs-lookup"><span data-stu-id="65f86-183">String</span></span>|<span data-ttu-id="65f86-184">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="65f86-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="65f86-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="65f86-185">connectAutomatically</span></span>|<span data-ttu-id="65f86-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="65f86-186">Boolean</span></span>|<span data-ttu-id="65f86-187">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="65f86-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="65f86-188">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="65f86-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="65f86-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="65f86-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="65f86-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="65f86-190">Boolean</span></span>|<span data-ttu-id="65f86-191">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="65f86-191">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="65f86-192">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="65f86-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="65f86-193">à</span><span class="sxs-lookup"><span data-stu-id="65f86-193">wiFiSecurityType</span></span>|[<span data-ttu-id="65f86-194">à</span><span class="sxs-lookup"><span data-stu-id="65f86-194">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="65f86-195">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="65f86-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="65f86-196">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="65f86-196">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="65f86-197">proxySettings</span><span class="sxs-lookup"><span data-stu-id="65f86-197">proxySettings</span></span>|[<span data-ttu-id="65f86-198">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="65f86-198">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="65f86-199">Tipo de proxy para esta conexão Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="65f86-199">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="65f86-200">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="65f86-200">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="65f86-201">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="65f86-201">proxyManualAddress</span></span>|<span data-ttu-id="65f86-202">String</span><span class="sxs-lookup"><span data-stu-id="65f86-202">String</span></span>|<span data-ttu-id="65f86-203">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="65f86-203">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="65f86-204">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="65f86-204">proxyManualPort</span></span>|<span data-ttu-id="65f86-205">Int32</span><span class="sxs-lookup"><span data-stu-id="65f86-205">Int32</span></span>|<span data-ttu-id="65f86-206">Porta do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="65f86-206">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="65f86-207">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="65f86-207">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="65f86-208">String</span><span class="sxs-lookup"><span data-stu-id="65f86-208">String</span></span>|<span data-ttu-id="65f86-209">URL do script de configuração automática do servidor proxy quando a configuração automática estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="65f86-209">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="65f86-210">Essa URL normalmente é o local do Arquivo PAC (configuração automática de proxy).</span><span class="sxs-lookup"><span data-stu-id="65f86-210">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="65f86-211">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="65f86-211">preSharedKey</span></span>|<span data-ttu-id="65f86-212">String</span><span class="sxs-lookup"><span data-stu-id="65f86-212">String</span></span>|<span data-ttu-id="65f86-213">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="65f86-213">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="65f86-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="65f86-214">Response</span></span>
<span data-ttu-id="65f86-215">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65f86-215">If successful, this method returns a `200 OK` response code and an updated [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65f86-216">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65f86-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="65f86-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65f86-217">Request</span></span>
<span data-ttu-id="65f86-218">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="65f86-218">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="65f86-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="65f86-219">Response</span></span>
<span data-ttu-id="65f86-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65f86-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





