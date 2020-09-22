---
title: Atualizar iosWiFiConfiguration
description: Atualiza as propriedades de um objeto iosWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 017e0ad2f5a0385de971b4ac6e3a9f386a90c058
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994789"
---
# <a name="update-ioswificonfiguration"></a><span data-ttu-id="e2cea-103">Atualizar iosWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2cea-103">Update iosWiFiConfiguration</span></span>

<span data-ttu-id="e2cea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2cea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2cea-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e2cea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2cea-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2cea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2cea-107">Atualiza as propriedades de um objeto [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e2cea-107">Update the properties of a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2cea-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e2cea-108">Prerequisites</span></span>
<span data-ttu-id="e2cea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2cea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2cea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2cea-111">Permission type</span></span>|<span data-ttu-id="e2cea-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e2cea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2cea-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2cea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2cea-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2cea-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2cea-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2cea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2cea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2cea-116">Not supported.</span></span>|
|<span data-ttu-id="e2cea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2cea-117">Application</span></span>|<span data-ttu-id="e2cea-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2cea-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2cea-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2cea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e2cea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2cea-120">Request headers</span></span>
|<span data-ttu-id="e2cea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e2cea-121">Header</span></span>|<span data-ttu-id="e2cea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e2cea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2cea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2cea-123">Authorization</span></span>|<span data-ttu-id="e2cea-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2cea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2cea-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e2cea-125">Accept</span></span>|<span data-ttu-id="e2cea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2cea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2cea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2cea-127">Request body</span></span>
<span data-ttu-id="e2cea-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e2cea-128">In the request body, supply a JSON representation for the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

<span data-ttu-id="e2cea-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2cea-129">The following table shows the properties that are required when you create the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span>

|<span data-ttu-id="e2cea-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2cea-130">Property</span></span>|<span data-ttu-id="e2cea-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2cea-131">Type</span></span>|<span data-ttu-id="e2cea-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2cea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2cea-133">id</span><span class="sxs-lookup"><span data-stu-id="e2cea-133">id</span></span>|<span data-ttu-id="e2cea-134">String</span><span class="sxs-lookup"><span data-stu-id="e2cea-134">String</span></span>|<span data-ttu-id="e2cea-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e2cea-135">Key of the entity.</span></span> <span data-ttu-id="e2cea-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2cea-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cea-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2cea-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e2cea-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2cea-138">DateTimeOffset</span></span>|<span data-ttu-id="e2cea-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e2cea-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e2cea-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2cea-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cea-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e2cea-141">roleScopeTagIds</span></span>|<span data-ttu-id="e2cea-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2cea-142">String collection</span></span>|<span data-ttu-id="e2cea-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="e2cea-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e2cea-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2cea-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cea-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e2cea-145">supportsScopeTags</span></span>|<span data-ttu-id="e2cea-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cea-146">Boolean</span></span>|<span data-ttu-id="e2cea-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="e2cea-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e2cea-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="e2cea-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e2cea-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="e2cea-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e2cea-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e2cea-150">This property is read-only.</span></span> <span data-ttu-id="e2cea-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2cea-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cea-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e2cea-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e2cea-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e2cea-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e2cea-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="e2cea-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e2cea-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2cea-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cea-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e2cea-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e2cea-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e2cea-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e2cea-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="e2cea-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e2cea-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2cea-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cea-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e2cea-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e2cea-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e2cea-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e2cea-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="e2cea-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e2cea-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2cea-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cea-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2cea-164">createdDateTime</span></span>|<span data-ttu-id="e2cea-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2cea-165">DateTimeOffset</span></span>|<span data-ttu-id="e2cea-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e2cea-166">DateTime the object was created.</span></span> <span data-ttu-id="e2cea-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2cea-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cea-168">description</span><span class="sxs-lookup"><span data-stu-id="e2cea-168">description</span></span>|<span data-ttu-id="e2cea-169">String</span><span class="sxs-lookup"><span data-stu-id="e2cea-169">String</span></span>|<span data-ttu-id="e2cea-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e2cea-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e2cea-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2cea-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cea-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e2cea-172">displayName</span></span>|<span data-ttu-id="e2cea-173">String</span><span class="sxs-lookup"><span data-stu-id="e2cea-173">String</span></span>|<span data-ttu-id="e2cea-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e2cea-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e2cea-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2cea-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cea-176">versão</span><span class="sxs-lookup"><span data-stu-id="e2cea-176">version</span></span>|<span data-ttu-id="e2cea-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e2cea-177">Int32</span></span>|<span data-ttu-id="e2cea-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e2cea-178">Version of the device configuration.</span></span> <span data-ttu-id="e2cea-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2cea-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2cea-180">NetworkName</span><span class="sxs-lookup"><span data-stu-id="e2cea-180">networkName</span></span>|<span data-ttu-id="e2cea-181">String</span><span class="sxs-lookup"><span data-stu-id="e2cea-181">String</span></span>|<span data-ttu-id="e2cea-182">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="e2cea-182">Network Name</span></span>|
|<span data-ttu-id="e2cea-183">SSID</span><span class="sxs-lookup"><span data-stu-id="e2cea-183">ssid</span></span>|<span data-ttu-id="e2cea-184">String</span><span class="sxs-lookup"><span data-stu-id="e2cea-184">String</span></span>|<span data-ttu-id="e2cea-185">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e2cea-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="e2cea-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="e2cea-186">connectAutomatically</span></span>|<span data-ttu-id="e2cea-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cea-187">Boolean</span></span>|<span data-ttu-id="e2cea-188">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="e2cea-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="e2cea-189">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e2cea-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="e2cea-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="e2cea-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="e2cea-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cea-191">Boolean</span></span>|<span data-ttu-id="e2cea-192">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="e2cea-192">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="e2cea-193">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e2cea-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="e2cea-194">à</span><span class="sxs-lookup"><span data-stu-id="e2cea-194">wiFiSecurityType</span></span>|[<span data-ttu-id="e2cea-195">à</span><span class="sxs-lookup"><span data-stu-id="e2cea-195">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="e2cea-196">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="e2cea-196">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="e2cea-197">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="e2cea-197">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="e2cea-198">proxySettings</span><span class="sxs-lookup"><span data-stu-id="e2cea-198">proxySettings</span></span>|[<span data-ttu-id="e2cea-199">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="e2cea-199">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="e2cea-200">Tipo de proxy para esta conexão Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e2cea-200">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="e2cea-201">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="e2cea-201">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="e2cea-202">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="e2cea-202">proxyManualAddress</span></span>|<span data-ttu-id="e2cea-203">String</span><span class="sxs-lookup"><span data-stu-id="e2cea-203">String</span></span>|<span data-ttu-id="e2cea-204">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="e2cea-204">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="e2cea-205">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="e2cea-205">proxyManualPort</span></span>|<span data-ttu-id="e2cea-206">Int32</span><span class="sxs-lookup"><span data-stu-id="e2cea-206">Int32</span></span>|<span data-ttu-id="e2cea-207">Porta do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="e2cea-207">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="e2cea-208">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="e2cea-208">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="e2cea-209">String</span><span class="sxs-lookup"><span data-stu-id="e2cea-209">String</span></span>|<span data-ttu-id="e2cea-210">URL do script de configuração automática do servidor proxy quando a configuração automática estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="e2cea-210">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="e2cea-211">Essa URL normalmente é o local do Arquivo PAC (configuração automática de proxy).</span><span class="sxs-lookup"><span data-stu-id="e2cea-211">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="e2cea-212">disableMacAddressRandomization</span><span class="sxs-lookup"><span data-stu-id="e2cea-212">disableMacAddressRandomization</span></span>|<span data-ttu-id="e2cea-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cea-213">Boolean</span></span>|<span data-ttu-id="e2cea-214">Se for definido como true, forçará os dispositivos que se conectam usando esse perfil Wi-Fi a apresentar seu endereço MAC de Wi-Fi real em vez de um endereço MAC aleatório.</span><span class="sxs-lookup"><span data-stu-id="e2cea-214">If set to true, forces devices connecting using this Wi-Fi profile to present their actual Wi-Fi MAC address instead of a random MAC address.</span></span> <span data-ttu-id="e2cea-215">Aplica-se ao iOS 14 e posterior.</span><span class="sxs-lookup"><span data-stu-id="e2cea-215">Applies to iOS 14 and later.</span></span>|
|<span data-ttu-id="e2cea-216">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="e2cea-216">preSharedKey</span></span>|<span data-ttu-id="e2cea-217">String</span><span class="sxs-lookup"><span data-stu-id="e2cea-217">String</span></span>|<span data-ttu-id="e2cea-218">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="e2cea-218">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="e2cea-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2cea-219">Response</span></span>
<span data-ttu-id="e2cea-220">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2cea-220">If successful, this method returns a `200 OK` response code and an updated [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2cea-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2cea-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2cea-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2cea-222">Request</span></span>
<span data-ttu-id="e2cea-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2cea-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1491

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
  "disableMacAddressRandomization": true,
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="e2cea-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2cea-224">Response</span></span>
<span data-ttu-id="e2cea-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2cea-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1663

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
  "disableMacAddressRandomization": true,
  "preSharedKey": "Pre Shared Key value"
}
```






