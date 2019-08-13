---
title: Atualizar macOSEnterpriseWiFiConfiguration
description: Atualiza as propriedades de um objeto macOSEnterpriseWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c64cdc632f9af72e6c3ca0b91d86b8052f1b43b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338718"
---
# <a name="update-macosenterprisewificonfiguration"></a><span data-ttu-id="aa8d9-103">Atualizar macOSEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="aa8d9-103">Update macOSEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="aa8d9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa8d9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa8d9-106">Atualiza as propriedades de um objeto [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="aa8d9-106">Update the properties of a [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa8d9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aa8d9-107">Prerequisites</span></span>
<span data-ttu-id="aa8d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa8d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa8d9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa8d9-110">Permission type</span></span>|<span data-ttu-id="aa8d9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa8d9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aa8d9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa8d9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aa8d9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa8d9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-115">Not supported.</span></span>|
|<span data-ttu-id="aa8d9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa8d9-116">Application</span></span>|<span data-ttu-id="aa8d9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa8d9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa8d9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa8d9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="aa8d9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa8d9-119">Request headers</span></span>
|<span data-ttu-id="aa8d9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aa8d9-120">Header</span></span>|<span data-ttu-id="aa8d9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="aa8d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa8d9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa8d9-122">Authorization</span></span>|<span data-ttu-id="aa8d9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa8d9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aa8d9-124">Accept</span></span>|<span data-ttu-id="aa8d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aa8d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa8d9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa8d9-126">Request body</span></span>
<span data-ttu-id="aa8d9-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="aa8d9-127">In the request body, supply a JSON representation for the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="aa8d9-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa8d9-128">The following table shows the properties that are required when you create the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="aa8d9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa8d9-129">Property</span></span>|<span data-ttu-id="aa8d9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa8d9-130">Type</span></span>|<span data-ttu-id="aa8d9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa8d9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa8d9-132">id</span><span class="sxs-lookup"><span data-stu-id="aa8d9-132">id</span></span>|<span data-ttu-id="aa8d9-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa8d9-133">String</span></span>|<span data-ttu-id="aa8d9-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-134">Key of the entity.</span></span> <span data-ttu-id="aa8d9-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa8d9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="aa8d9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa8d9-137">DateTimeOffset</span></span>|<span data-ttu-id="aa8d9-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="aa8d9-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aa8d9-140">roleScopeTagIds</span></span>|<span data-ttu-id="aa8d9-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa8d9-141">String collection</span></span>|<span data-ttu-id="aa8d9-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aa8d9-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="aa8d9-144">supportsScopeTags</span></span>|<span data-ttu-id="aa8d9-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="aa8d9-145">Boolean</span></span>|<span data-ttu-id="aa8d9-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aa8d9-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aa8d9-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aa8d9-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-149">This property is read-only.</span></span> <span data-ttu-id="aa8d9-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="aa8d9-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="aa8d9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="aa8d9-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="aa8d9-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="aa8d9-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="aa8d9-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="aa8d9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="aa8d9-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="aa8d9-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="aa8d9-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="aa8d9-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="aa8d9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="aa8d9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="aa8d9-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="aa8d9-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa8d9-163">createdDateTime</span></span>|<span data-ttu-id="aa8d9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa8d9-164">DateTimeOffset</span></span>|<span data-ttu-id="aa8d9-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-165">DateTime the object was created.</span></span> <span data-ttu-id="aa8d9-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-167">descrição</span><span class="sxs-lookup"><span data-stu-id="aa8d9-167">description</span></span>|<span data-ttu-id="aa8d9-168">String</span><span class="sxs-lookup"><span data-stu-id="aa8d9-168">String</span></span>|<span data-ttu-id="aa8d9-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aa8d9-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-171">displayName</span><span class="sxs-lookup"><span data-stu-id="aa8d9-171">displayName</span></span>|<span data-ttu-id="aa8d9-172">String</span><span class="sxs-lookup"><span data-stu-id="aa8d9-172">String</span></span>|<span data-ttu-id="aa8d9-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aa8d9-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-175">versão</span><span class="sxs-lookup"><span data-stu-id="aa8d9-175">version</span></span>|<span data-ttu-id="aa8d9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="aa8d9-176">Int32</span></span>|<span data-ttu-id="aa8d9-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-177">Version of the device configuration.</span></span> <span data-ttu-id="aa8d9-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-179">NetworkName</span><span class="sxs-lookup"><span data-stu-id="aa8d9-179">networkName</span></span>|<span data-ttu-id="aa8d9-180">String</span><span class="sxs-lookup"><span data-stu-id="aa8d9-180">String</span></span>|<span data-ttu-id="aa8d9-181">Nome da rede herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-181">Network Name Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-182">SSID</span><span class="sxs-lookup"><span data-stu-id="aa8d9-182">ssid</span></span>|<span data-ttu-id="aa8d9-183">String</span><span class="sxs-lookup"><span data-stu-id="aa8d9-183">String</span></span>|<span data-ttu-id="aa8d9-184">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="aa8d9-185">Herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-185">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="aa8d9-186">connectAutomatically</span></span>|<span data-ttu-id="aa8d9-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="aa8d9-187">Boolean</span></span>|<span data-ttu-id="aa8d9-188">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="aa8d9-189">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="aa8d9-190">Herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-190">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="aa8d9-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="aa8d9-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="aa8d9-192">Boolean</span></span>|<span data-ttu-id="aa8d9-193">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="aa8d9-193">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="aa8d9-194">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="aa8d9-195">Herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-195">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-196">à</span><span class="sxs-lookup"><span data-stu-id="aa8d9-196">wiFiSecurityType</span></span>|[<span data-ttu-id="aa8d9-197">à</span><span class="sxs-lookup"><span data-stu-id="aa8d9-197">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="aa8d9-198">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="aa8d9-199">Herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa8d9-199">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="aa8d9-200">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-200">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="aa8d9-201">proxySettings</span><span class="sxs-lookup"><span data-stu-id="aa8d9-201">proxySettings</span></span>|[<span data-ttu-id="aa8d9-202">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="aa8d9-202">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="aa8d9-203">Tipo de proxy para esta conexão Wi-Fi herdada de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa8d9-203">Proxy Type for this Wi-Fi connection Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="aa8d9-204">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-204">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="aa8d9-205">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="aa8d9-205">proxyManualAddress</span></span>|<span data-ttu-id="aa8d9-206">String</span><span class="sxs-lookup"><span data-stu-id="aa8d9-206">String</span></span>|<span data-ttu-id="aa8d9-207">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-207">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="aa8d9-208">Herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-208">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-209">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="aa8d9-209">proxyManualPort</span></span>|<span data-ttu-id="aa8d9-210">Int32</span><span class="sxs-lookup"><span data-stu-id="aa8d9-210">Int32</span></span>|<span data-ttu-id="aa8d9-211">Porta do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-211">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="aa8d9-212">Herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-212">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-213">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="aa8d9-213">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="aa8d9-214">String</span><span class="sxs-lookup"><span data-stu-id="aa8d9-214">String</span></span>|<span data-ttu-id="aa8d9-215">URL do script de configuração automática do servidor proxy quando a configuração automática estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-215">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="aa8d9-216">Essa URL normalmente é o local do Arquivo PAC (configuração automática de proxy).</span><span class="sxs-lookup"><span data-stu-id="aa8d9-216">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="aa8d9-217">Herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-217">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-218">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="aa8d9-218">preSharedKey</span></span>|<span data-ttu-id="aa8d9-219">String</span><span class="sxs-lookup"><span data-stu-id="aa8d9-219">String</span></span>|<span data-ttu-id="aa8d9-220">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-220">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="aa8d9-221">Herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa8d9-221">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="aa8d9-222">eapType</span><span class="sxs-lookup"><span data-stu-id="aa8d9-222">eapType</span></span>|[<span data-ttu-id="aa8d9-223">eapType</span><span class="sxs-lookup"><span data-stu-id="aa8d9-223">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="aa8d9-224">EAP (protocolo de autenticação extensível).</span><span class="sxs-lookup"><span data-stu-id="aa8d9-224">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="aa8d9-225">Indica o tipo de protocolo EAP definido no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="aa8d9-225">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="aa8d9-226">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-226">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="aa8d9-227">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="aa8d9-227">eapFastConfiguration</span></span>|[<span data-ttu-id="aa8d9-228">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="aa8d9-228">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="aa8d9-229">Opção de configuração EAP-FAST quando EAP-FAST for o tipo de EAP selecionado.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-229">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="aa8d9-230">Os valores possíveis são: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-230">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="aa8d9-231">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="aa8d9-231">trustedServerCertificateNames</span></span>|<span data-ttu-id="aa8d9-232">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa8d9-232">String collection</span></span>|<span data-ttu-id="aa8d9-233">Nomes de certificados de servidor confiáveis quando o tipo EAP é configurado como EAP-TLS/TTLS/FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-233">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="aa8d9-234">Este é o nome comum usado nos certificados emitidos pela autoridade de certificação (CA) confiável.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-234">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="aa8d9-235">Se você fornecer essas informações, poderá ignorar a caixa de diálogo de confiança dinâmica exibida em dispositivos de usuários finais quando eles se conectam a esta rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-235">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="aa8d9-236">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="aa8d9-236">authenticationMethod</span></span>|[<span data-ttu-id="aa8d9-237">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="aa8d9-237">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="aa8d9-238">Método de autenticação quando o tipo EAP é configurado como PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-238">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="aa8d9-239">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-239">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="aa8d9-240">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="aa8d9-240">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="aa8d9-241">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="aa8d9-241">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="aa8d9-242">Método não EAP para autenticação (identidade interna) quando o tipo EAP é EAP-TTLS e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-242">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="aa8d9-243">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-243">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="aa8d9-244">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="aa8d9-244">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="aa8d9-245">String</span><span class="sxs-lookup"><span data-stu-id="aa8d9-245">String</span></span>|<span data-ttu-id="aa8d9-246">Habilitar Privacidade de identidade (identidade externa) quando o tipo EAP é configurado como EAP-TTLS, EAP-FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-246">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="aa8d9-247">Essa propriedade mascara os nomes de usernames com o texto inserido.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-247">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="aa8d9-248">Por exemplo, se você usar ' anônimo ', cada usuário que autenticar com essa conexão Wi-Fi usando seu nome de usuário real será exibido como ' anônimo '.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-248">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="aa8d9-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa8d9-249">Response</span></span>
<span data-ttu-id="aa8d9-250">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-250">If successful, this method returns a `200 OK` response code and an updated [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa8d9-251">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa8d9-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa8d9-252">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa8d9-252">Request</span></span>
<span data-ttu-id="aa8d9-253">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-253">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1858

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="aa8d9-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa8d9-254">Response</span></span>
<span data-ttu-id="aa8d9-p128">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa8d9-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2030

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
  "id": "7a6f9a2e-9a2e-7a6f-2e9a-6f7a2e9a6f7a",
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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```






