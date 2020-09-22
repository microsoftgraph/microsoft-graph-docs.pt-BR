---
title: Criar macOSWiFiConfiguration
description: Criar um novo objeto macOSWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0e0de34689030bfd0552d4140b49ad69c6dc63a7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017873"
---
# <a name="create-macoswificonfiguration"></a><span data-ttu-id="f3d42-103">Criar macOSWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="f3d42-103">Create macOSWiFiConfiguration</span></span>

<span data-ttu-id="f3d42-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3d42-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3d42-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3d42-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3d42-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3d42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3d42-107">Criar um novo objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f3d42-107">Create a new [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3d42-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f3d42-108">Prerequisites</span></span>
<span data-ttu-id="f3d42-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3d42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3d42-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3d42-111">Permission type</span></span>|<span data-ttu-id="f3d42-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f3d42-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3d42-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3d42-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3d42-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3d42-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3d42-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3d42-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3d42-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3d42-116">Not supported.</span></span>|
|<span data-ttu-id="f3d42-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3d42-117">Application</span></span>|<span data-ttu-id="f3d42-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3d42-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3d42-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3d42-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f3d42-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3d42-120">Request headers</span></span>
|<span data-ttu-id="f3d42-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f3d42-121">Header</span></span>|<span data-ttu-id="f3d42-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f3d42-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3d42-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3d42-123">Authorization</span></span>|<span data-ttu-id="f3d42-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3d42-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3d42-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f3d42-125">Accept</span></span>|<span data-ttu-id="f3d42-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3d42-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3d42-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3d42-127">Request body</span></span>
<span data-ttu-id="f3d42-128">No corpo da solicitação, forneça uma representação JSON do objeto macOSWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f3d42-128">In the request body, supply a JSON representation for the macOSWiFiConfiguration object.</span></span>

<span data-ttu-id="f3d42-129">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f3d42-129">The following table shows the properties that are required when you create the macOSWiFiConfiguration.</span></span>

|<span data-ttu-id="f3d42-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3d42-130">Property</span></span>|<span data-ttu-id="f3d42-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3d42-131">Type</span></span>|<span data-ttu-id="f3d42-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3d42-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3d42-133">id</span><span class="sxs-lookup"><span data-stu-id="f3d42-133">id</span></span>|<span data-ttu-id="f3d42-134">String</span><span class="sxs-lookup"><span data-stu-id="f3d42-134">String</span></span>|<span data-ttu-id="f3d42-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f3d42-135">Key of the entity.</span></span> <span data-ttu-id="f3d42-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3d42-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d42-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3d42-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f3d42-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3d42-138">DateTimeOffset</span></span>|<span data-ttu-id="f3d42-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f3d42-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f3d42-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3d42-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d42-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f3d42-141">roleScopeTagIds</span></span>|<span data-ttu-id="f3d42-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f3d42-142">String collection</span></span>|<span data-ttu-id="f3d42-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f3d42-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f3d42-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3d42-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d42-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f3d42-145">supportsScopeTags</span></span>|<span data-ttu-id="f3d42-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3d42-146">Boolean</span></span>|<span data-ttu-id="f3d42-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f3d42-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f3d42-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f3d42-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f3d42-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f3d42-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f3d42-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f3d42-150">This property is read-only.</span></span> <span data-ttu-id="f3d42-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3d42-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d42-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f3d42-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f3d42-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f3d42-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f3d42-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="f3d42-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f3d42-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3d42-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d42-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f3d42-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f3d42-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f3d42-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f3d42-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="f3d42-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f3d42-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3d42-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d42-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f3d42-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f3d42-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f3d42-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f3d42-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="f3d42-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f3d42-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3d42-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d42-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3d42-164">createdDateTime</span></span>|<span data-ttu-id="f3d42-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3d42-165">DateTimeOffset</span></span>|<span data-ttu-id="f3d42-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f3d42-166">DateTime the object was created.</span></span> <span data-ttu-id="f3d42-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3d42-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d42-168">description</span><span class="sxs-lookup"><span data-stu-id="f3d42-168">description</span></span>|<span data-ttu-id="f3d42-169">String</span><span class="sxs-lookup"><span data-stu-id="f3d42-169">String</span></span>|<span data-ttu-id="f3d42-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3d42-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f3d42-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3d42-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d42-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f3d42-172">displayName</span></span>|<span data-ttu-id="f3d42-173">String</span><span class="sxs-lookup"><span data-stu-id="f3d42-173">String</span></span>|<span data-ttu-id="f3d42-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3d42-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f3d42-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3d42-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d42-176">versão</span><span class="sxs-lookup"><span data-stu-id="f3d42-176">version</span></span>|<span data-ttu-id="f3d42-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f3d42-177">Int32</span></span>|<span data-ttu-id="f3d42-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3d42-178">Version of the device configuration.</span></span> <span data-ttu-id="f3d42-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3d42-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d42-180">NetworkName</span><span class="sxs-lookup"><span data-stu-id="f3d42-180">networkName</span></span>|<span data-ttu-id="f3d42-181">String</span><span class="sxs-lookup"><span data-stu-id="f3d42-181">String</span></span>|<span data-ttu-id="f3d42-182">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="f3d42-182">Network Name</span></span>|
|<span data-ttu-id="f3d42-183">SSID</span><span class="sxs-lookup"><span data-stu-id="f3d42-183">ssid</span></span>|<span data-ttu-id="f3d42-184">String</span><span class="sxs-lookup"><span data-stu-id="f3d42-184">String</span></span>|<span data-ttu-id="f3d42-185">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f3d42-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="f3d42-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="f3d42-186">connectAutomatically</span></span>|<span data-ttu-id="f3d42-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3d42-187">Boolean</span></span>|<span data-ttu-id="f3d42-188">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="f3d42-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="f3d42-189">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f3d42-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="f3d42-190">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="f3d42-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="f3d42-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3d42-191">Boolean</span></span>|<span data-ttu-id="f3d42-192">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="f3d42-192">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="f3d42-193">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f3d42-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="f3d42-194">à</span><span class="sxs-lookup"><span data-stu-id="f3d42-194">wiFiSecurityType</span></span>|[<span data-ttu-id="f3d42-195">à</span><span class="sxs-lookup"><span data-stu-id="f3d42-195">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="f3d42-196">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="f3d42-196">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="f3d42-197">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="f3d42-197">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="f3d42-198">proxySettings</span><span class="sxs-lookup"><span data-stu-id="f3d42-198">proxySettings</span></span>|[<span data-ttu-id="f3d42-199">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="f3d42-199">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="f3d42-200">Tipo de proxy para esta conexão Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f3d42-200">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="f3d42-201">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="f3d42-201">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="f3d42-202">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="f3d42-202">proxyManualAddress</span></span>|<span data-ttu-id="f3d42-203">String</span><span class="sxs-lookup"><span data-stu-id="f3d42-203">String</span></span>|<span data-ttu-id="f3d42-204">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="f3d42-204">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="f3d42-205">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="f3d42-205">proxyManualPort</span></span>|<span data-ttu-id="f3d42-206">Int32</span><span class="sxs-lookup"><span data-stu-id="f3d42-206">Int32</span></span>|<span data-ttu-id="f3d42-207">Porta do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="f3d42-207">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="f3d42-208">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="f3d42-208">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="f3d42-209">String</span><span class="sxs-lookup"><span data-stu-id="f3d42-209">String</span></span>|<span data-ttu-id="f3d42-210">URL do script de configuração automática do servidor proxy quando a configuração automática estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="f3d42-210">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="f3d42-211">Essa URL normalmente é o local do Arquivo PAC (configuração automática de proxy).</span><span class="sxs-lookup"><span data-stu-id="f3d42-211">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="f3d42-212">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="f3d42-212">preSharedKey</span></span>|<span data-ttu-id="f3d42-213">String</span><span class="sxs-lookup"><span data-stu-id="f3d42-213">String</span></span>|<span data-ttu-id="f3d42-214">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="f3d42-214">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="f3d42-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3d42-215">Response</span></span>
<span data-ttu-id="f3d42-216">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3d42-216">If successful, this method returns a `201 Created` response code and a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3d42-217">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3d42-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3d42-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3d42-218">Request</span></span>
<span data-ttu-id="f3d42-219">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3d42-219">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f3d42-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3d42-220">Response</span></span>
<span data-ttu-id="f3d42-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3d42-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






