---
title: Atualizar macOSWiFiConfiguration
description: Atualiza as propriedades de um objeto macOSWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 613b8833162dc38011674c870a75d1084e3a8dfb
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948034"
---
# <a name="update-macoswificonfiguration"></a><span data-ttu-id="f8294-103">Atualizar macOSWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8294-103">Update macOSWiFiConfiguration</span></span>

> <span data-ttu-id="f8294-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8294-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8294-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8294-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8294-106">Atualiza as propriedades de um objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f8294-106">Update the properties of a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8294-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8294-107">Prerequisites</span></span>
<span data-ttu-id="f8294-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8294-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8294-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8294-110">Permission type</span></span>|<span data-ttu-id="f8294-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8294-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8294-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8294-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f8294-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8294-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8294-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8294-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8294-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8294-115">Not supported.</span></span>|
|<span data-ttu-id="f8294-116">Application</span><span class="sxs-lookup"><span data-stu-id="f8294-116">Application</span></span>|<span data-ttu-id="f8294-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8294-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8294-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8294-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f8294-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8294-119">Request headers</span></span>
|<span data-ttu-id="f8294-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8294-120">Header</span></span>|<span data-ttu-id="f8294-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f8294-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8294-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8294-122">Authorization</span></span>|<span data-ttu-id="f8294-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8294-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8294-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8294-124">Accept</span></span>|<span data-ttu-id="f8294-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f8294-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8294-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8294-126">Request body</span></span>
<span data-ttu-id="f8294-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f8294-127">In the request body, supply a JSON representation for the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

<span data-ttu-id="f8294-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8294-128">The following table shows the properties that are required when you create the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span>

|<span data-ttu-id="f8294-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8294-129">Property</span></span>|<span data-ttu-id="f8294-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8294-130">Type</span></span>|<span data-ttu-id="f8294-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8294-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8294-132">id</span><span class="sxs-lookup"><span data-stu-id="f8294-132">id</span></span>|<span data-ttu-id="f8294-133">String</span><span class="sxs-lookup"><span data-stu-id="f8294-133">String</span></span>|<span data-ttu-id="f8294-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f8294-134">Key of the entity.</span></span> <span data-ttu-id="f8294-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8294-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f8294-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8294-137">DateTimeOffset</span></span>|<span data-ttu-id="f8294-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f8294-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f8294-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f8294-140">roleScopeTagIds</span></span>|<span data-ttu-id="f8294-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8294-141">String collection</span></span>|<span data-ttu-id="f8294-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f8294-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f8294-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f8294-144">supportsScopeTags</span></span>|<span data-ttu-id="f8294-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8294-145">Boolean</span></span>|<span data-ttu-id="f8294-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f8294-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f8294-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f8294-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f8294-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f8294-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f8294-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f8294-149">This property is read-only.</span></span> <span data-ttu-id="f8294-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f8294-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f8294-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f8294-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f8294-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="f8294-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f8294-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f8294-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f8294-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f8294-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f8294-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="f8294-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f8294-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f8294-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f8294-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f8294-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f8294-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="f8294-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f8294-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8294-163">createdDateTime</span></span>|<span data-ttu-id="f8294-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8294-164">DateTimeOffset</span></span>|<span data-ttu-id="f8294-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f8294-165">DateTime the object was created.</span></span> <span data-ttu-id="f8294-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-167">description</span><span class="sxs-lookup"><span data-stu-id="f8294-167">description</span></span>|<span data-ttu-id="f8294-168">String</span><span class="sxs-lookup"><span data-stu-id="f8294-168">String</span></span>|<span data-ttu-id="f8294-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8294-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f8294-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f8294-171">displayName</span></span>|<span data-ttu-id="f8294-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8294-172">String</span></span>|<span data-ttu-id="f8294-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8294-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f8294-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-175">versão</span><span class="sxs-lookup"><span data-stu-id="f8294-175">version</span></span>|<span data-ttu-id="f8294-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f8294-176">Int32</span></span>|<span data-ttu-id="f8294-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8294-177">Version of the device configuration.</span></span> <span data-ttu-id="f8294-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8294-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8294-179">NetworkName</span><span class="sxs-lookup"><span data-stu-id="f8294-179">networkName</span></span>|<span data-ttu-id="f8294-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f8294-180">String</span></span>|<span data-ttu-id="f8294-181">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="f8294-181">Network Name</span></span>|
|<span data-ttu-id="f8294-182">SSID</span><span class="sxs-lookup"><span data-stu-id="f8294-182">ssid</span></span>|<span data-ttu-id="f8294-183">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f8294-183">String</span></span>|<span data-ttu-id="f8294-184">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f8294-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="f8294-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="f8294-185">connectAutomatically</span></span>|<span data-ttu-id="f8294-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8294-186">Boolean</span></span>|<span data-ttu-id="f8294-187">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="f8294-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="f8294-188">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f8294-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="f8294-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="f8294-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="f8294-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8294-190">Boolean</span></span>|<span data-ttu-id="f8294-191">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="f8294-191">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="f8294-192">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f8294-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="f8294-193">à</span><span class="sxs-lookup"><span data-stu-id="f8294-193">wiFiSecurityType</span></span>|[<span data-ttu-id="f8294-194">à</span><span class="sxs-lookup"><span data-stu-id="f8294-194">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="f8294-195">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="f8294-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="f8294-196">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="f8294-196">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="f8294-197">proxySettings</span><span class="sxs-lookup"><span data-stu-id="f8294-197">proxySettings</span></span>|[<span data-ttu-id="f8294-198">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="f8294-198">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="f8294-199">Tipo de proxy para esta conexão Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f8294-199">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="f8294-200">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="f8294-200">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="f8294-201">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="f8294-201">proxyManualAddress</span></span>|<span data-ttu-id="f8294-202">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f8294-202">String</span></span>|<span data-ttu-id="f8294-203">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="f8294-203">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="f8294-204">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="f8294-204">proxyManualPort</span></span>|<span data-ttu-id="f8294-205">Int32</span><span class="sxs-lookup"><span data-stu-id="f8294-205">Int32</span></span>|<span data-ttu-id="f8294-206">Porta do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="f8294-206">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="f8294-207">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="f8294-207">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="f8294-208">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f8294-208">String</span></span>|<span data-ttu-id="f8294-209">URL do script de configuração automática do servidor proxy quando a configuração automática estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="f8294-209">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="f8294-210">Essa URL normalmente é o local do Arquivo PAC (configuração automática de proxy).</span><span class="sxs-lookup"><span data-stu-id="f8294-210">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="f8294-211">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="f8294-211">preSharedKey</span></span>|<span data-ttu-id="f8294-212">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="f8294-212">String</span></span>|<span data-ttu-id="f8294-213">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="f8294-213">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="f8294-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8294-214">Response</span></span>
<span data-ttu-id="f8294-215">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8294-215">If successful, this method returns a `200 OK` response code and an updated [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8294-216">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8294-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8294-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8294-217">Request</span></span>
<span data-ttu-id="f8294-218">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8294-218">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f8294-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8294-219">Response</span></span>
<span data-ttu-id="f8294-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8294-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





