---
title: Criar iosEnterpriseWiFiConfiguration
description: Criar um novo objeto iosEnterpriseWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 243fd70da27535d3a19d2e271d0346abeab13742
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442793"
---
# <a name="create-iosenterprisewificonfiguration"></a><span data-ttu-id="6c295-103">Criar iosEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c295-103">Create iosEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="6c295-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6c295-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c295-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c295-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c295-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c295-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c295-107">Criar um novo objeto [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6c295-107">Create a new [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c295-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c295-108">Prerequisites</span></span>
<span data-ttu-id="6c295-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c295-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c295-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c295-111">Permission type</span></span>|<span data-ttu-id="6c295-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c295-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c295-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c295-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c295-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c295-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c295-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c295-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c295-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c295-116">Not supported.</span></span>|
|<span data-ttu-id="6c295-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c295-117">Application</span></span>|<span data-ttu-id="6c295-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c295-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c295-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c295-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6c295-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c295-120">Request headers</span></span>
|<span data-ttu-id="6c295-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c295-121">Header</span></span>|<span data-ttu-id="6c295-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6c295-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c295-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c295-123">Authorization</span></span>|<span data-ttu-id="6c295-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c295-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c295-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c295-125">Accept</span></span>|<span data-ttu-id="6c295-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c295-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c295-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c295-127">Request body</span></span>
<span data-ttu-id="6c295-128">No corpo da solicitação, forneça uma representação JSON do objeto iosEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6c295-128">In the request body, supply a JSON representation for the iosEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="6c295-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6c295-129">The following table shows the properties that are required when you create the iosEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="6c295-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c295-130">Property</span></span>|<span data-ttu-id="6c295-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c295-131">Type</span></span>|<span data-ttu-id="6c295-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c295-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c295-133">id</span><span class="sxs-lookup"><span data-stu-id="6c295-133">id</span></span>|<span data-ttu-id="6c295-134">String</span><span class="sxs-lookup"><span data-stu-id="6c295-134">String</span></span>|<span data-ttu-id="6c295-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6c295-135">Key of the entity.</span></span> <span data-ttu-id="6c295-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c295-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c295-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6c295-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c295-138">DateTimeOffset</span></span>|<span data-ttu-id="6c295-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6c295-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6c295-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c295-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6c295-141">roleScopeTagIds</span></span>|<span data-ttu-id="6c295-142">String collection</span><span class="sxs-lookup"><span data-stu-id="6c295-142">String collection</span></span>|<span data-ttu-id="6c295-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6c295-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6c295-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c295-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6c295-145">supportsScopeTags</span></span>|<span data-ttu-id="6c295-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c295-146">Boolean</span></span>|<span data-ttu-id="6c295-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6c295-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6c295-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6c295-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6c295-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6c295-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6c295-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6c295-150">This property is read-only.</span></span> <span data-ttu-id="6c295-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c295-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6c295-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6c295-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6c295-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6c295-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="6c295-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6c295-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c295-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6c295-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6c295-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6c295-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6c295-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="6c295-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6c295-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c295-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6c295-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6c295-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6c295-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6c295-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="6c295-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6c295-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c295-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c295-164">createdDateTime</span></span>|<span data-ttu-id="6c295-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c295-165">DateTimeOffset</span></span>|<span data-ttu-id="6c295-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6c295-166">DateTime the object was created.</span></span> <span data-ttu-id="6c295-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c295-168">description</span><span class="sxs-lookup"><span data-stu-id="6c295-168">description</span></span>|<span data-ttu-id="6c295-169">String</span><span class="sxs-lookup"><span data-stu-id="6c295-169">String</span></span>|<span data-ttu-id="6c295-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c295-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6c295-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c295-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6c295-172">displayName</span></span>|<span data-ttu-id="6c295-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c295-173">String</span></span>|<span data-ttu-id="6c295-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c295-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6c295-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c295-176">versão</span><span class="sxs-lookup"><span data-stu-id="6c295-176">version</span></span>|<span data-ttu-id="6c295-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6c295-177">Int32</span></span>|<span data-ttu-id="6c295-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c295-178">Version of the device configuration.</span></span> <span data-ttu-id="6c295-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c295-180">NetworkName</span><span class="sxs-lookup"><span data-stu-id="6c295-180">networkName</span></span>|<span data-ttu-id="6c295-181">String</span><span class="sxs-lookup"><span data-stu-id="6c295-181">String</span></span>|<span data-ttu-id="6c295-182">Nome da rede herdado de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-182">Network Name Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6c295-183">SSID</span><span class="sxs-lookup"><span data-stu-id="6c295-183">ssid</span></span>|<span data-ttu-id="6c295-184">String</span><span class="sxs-lookup"><span data-stu-id="6c295-184">String</span></span>|<span data-ttu-id="6c295-185">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6c295-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="6c295-186">Herdado de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-186">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6c295-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="6c295-187">connectAutomatically</span></span>|<span data-ttu-id="6c295-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c295-188">Boolean</span></span>|<span data-ttu-id="6c295-189">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="6c295-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="6c295-190">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="6c295-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="6c295-191">Herdado de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-191">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6c295-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="6c295-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="6c295-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c295-193">Boolean</span></span>|<span data-ttu-id="6c295-194">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="6c295-194">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="6c295-195">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6c295-195">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="6c295-196">Herdado de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-196">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6c295-197">à</span><span class="sxs-lookup"><span data-stu-id="6c295-197">wiFiSecurityType</span></span>|[<span data-ttu-id="6c295-198">à</span><span class="sxs-lookup"><span data-stu-id="6c295-198">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="6c295-199">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="6c295-199">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="6c295-200">Herdado de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c295-200">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="6c295-201">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="6c295-201">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="6c295-202">proxySettings</span><span class="sxs-lookup"><span data-stu-id="6c295-202">proxySettings</span></span>|[<span data-ttu-id="6c295-203">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="6c295-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="6c295-204">Tipo de proxy para esta conexão Wi-Fi herdada de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6c295-204">Proxy Type for this Wi-Fi connection Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="6c295-205">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="6c295-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="6c295-206">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="6c295-206">proxyManualAddress</span></span>|<span data-ttu-id="6c295-207">String</span><span class="sxs-lookup"><span data-stu-id="6c295-207">String</span></span>|<span data-ttu-id="6c295-208">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="6c295-208">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="6c295-209">Herdado de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-209">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6c295-210">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="6c295-210">proxyManualPort</span></span>|<span data-ttu-id="6c295-211">Int32</span><span class="sxs-lookup"><span data-stu-id="6c295-211">Int32</span></span>|<span data-ttu-id="6c295-212">Porta do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="6c295-212">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="6c295-213">Herdado de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-213">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6c295-214">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="6c295-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="6c295-215">String</span><span class="sxs-lookup"><span data-stu-id="6c295-215">String</span></span>|<span data-ttu-id="6c295-216">URL do script de configuração automática do servidor proxy quando a configuração automática estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="6c295-216">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="6c295-217">Essa URL normalmente é o local do Arquivo PAC (configuração automática de proxy).</span><span class="sxs-lookup"><span data-stu-id="6c295-217">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="6c295-218">Herdado de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-218">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6c295-219">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="6c295-219">preSharedKey</span></span>|<span data-ttu-id="6c295-220">String</span><span class="sxs-lookup"><span data-stu-id="6c295-220">String</span></span>|<span data-ttu-id="6c295-221">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="6c295-221">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="6c295-222">Herdado de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c295-222">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6c295-223">eapType</span><span class="sxs-lookup"><span data-stu-id="6c295-223">eapType</span></span>|[<span data-ttu-id="6c295-224">eapType</span><span class="sxs-lookup"><span data-stu-id="6c295-224">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="6c295-225">EAP (protocolo de autenticação extensível).</span><span class="sxs-lookup"><span data-stu-id="6c295-225">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="6c295-226">Indica o tipo de protocolo EAP definido no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="6c295-226">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="6c295-227">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="6c295-227">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="6c295-228">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c295-228">eapFastConfiguration</span></span>|[<span data-ttu-id="6c295-229">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c295-229">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="6c295-230">Opção de configuração EAP-FAST quando EAP-FAST for o tipo de EAP selecionado.</span><span class="sxs-lookup"><span data-stu-id="6c295-230">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="6c295-231">Os valores possíveis são: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="6c295-231">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="6c295-232">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="6c295-232">trustedServerCertificateNames</span></span>|<span data-ttu-id="6c295-233">String collection</span><span class="sxs-lookup"><span data-stu-id="6c295-233">String collection</span></span>|<span data-ttu-id="6c295-234">Nomes de certificados de servidor confiáveis quando o tipo EAP é configurado como EAP-TLS/TTLS/FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="6c295-234">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="6c295-235">Este é o nome comum usado nos certificados emitidos pela autoridade de certificação (CA) confiável.</span><span class="sxs-lookup"><span data-stu-id="6c295-235">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="6c295-236">Se você fornecer essas informações, poderá ignorar a caixa de diálogo de confiança dinâmica exibida nos dispositivos dos usuários finais quando eles se conectam a esta rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="6c295-236">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users' devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="6c295-237">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6c295-237">authenticationMethod</span></span>|[<span data-ttu-id="6c295-238">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6c295-238">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="6c295-239">Método de autenticação quando o tipo EAP é configurado como PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="6c295-239">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="6c295-240">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="6c295-240">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="6c295-241">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="6c295-241">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="6c295-242">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="6c295-242">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="6c295-243">Método não EAP para autenticação quando o tipo EAP é EAP-TTLS e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="6c295-243">Non-EAP Method for Authentication when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="6c295-244">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="6c295-244">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="6c295-245">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="6c295-245">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="6c295-246">String</span><span class="sxs-lookup"><span data-stu-id="6c295-246">String</span></span>|<span data-ttu-id="6c295-247">Habilitar Privacidade de identidade (identidade externa) quando o tipo EAP é configurado como EAP-TTLS, EAP-FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="6c295-247">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP - TTLS, EAP - FAST or PEAP.</span></span> <span data-ttu-id="6c295-248">Essa propriedade mascara os nomes de usernames com o texto inserido.</span><span class="sxs-lookup"><span data-stu-id="6c295-248">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="6c295-249">Por exemplo, se você usar ' anônimo ', cada usuário que autenticar com essa conexão Wi-Fi usando seu nome de usuário real será exibido como ' anônimo '.</span><span class="sxs-lookup"><span data-stu-id="6c295-249">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|
|<span data-ttu-id="6c295-250">usernameFormatString</span><span class="sxs-lookup"><span data-stu-id="6c295-250">usernameFormatString</span></span>|<span data-ttu-id="6c295-251">String</span><span class="sxs-lookup"><span data-stu-id="6c295-251">String</span></span>|<span data-ttu-id="6c295-252">Cadeia de caracteres de formato de nome de usuário usada para criar o nome de usuário para se conectar</span><span class="sxs-lookup"><span data-stu-id="6c295-252">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="6c295-253">passwordFormatString</span><span class="sxs-lookup"><span data-stu-id="6c295-253">passwordFormatString</span></span>|<span data-ttu-id="6c295-254">String</span><span class="sxs-lookup"><span data-stu-id="6c295-254">String</span></span>|<span data-ttu-id="6c295-255">Cadeia de caracteres de formato de senha usada para criar a senha para se conectar ao wifi</span><span class="sxs-lookup"><span data-stu-id="6c295-255">Password format string used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="6c295-256">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c295-256">Response</span></span>
<span data-ttu-id="6c295-257">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c295-257">If successful, this method returns a `201 Created` response code and a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c295-258">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c295-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c295-259">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c295-259">Request</span></span>
<span data-ttu-id="6c295-260">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c295-260">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1974

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
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
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value"
}
```

### <a name="response"></a><span data-ttu-id="6c295-261">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c295-261">Response</span></span>
<span data-ttu-id="6c295-p128">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c295-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2146

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
  "id": "7593f7ba-f7ba-7593-baf7-9375baf79375",
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
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value"
}
```





