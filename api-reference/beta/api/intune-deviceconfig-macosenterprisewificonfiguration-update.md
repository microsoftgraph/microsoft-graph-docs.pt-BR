---
title: Atualizar macOSEnterpriseWiFiConfiguration
description: Atualiza as propriedades de um objeto macOSEnterpriseWiFiConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57fa3910f4b3bf9ac65f1968e0803839ed68cc02
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42746327"
---
# <a name="update-macosenterprisewificonfiguration"></a><span data-ttu-id="37bd1-103">Atualizar macOSEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="37bd1-103">Update macOSEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="37bd1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37bd1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37bd1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37bd1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37bd1-106">Atualiza as propriedades de um objeto [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="37bd1-106">Update the properties of a [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37bd1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="37bd1-107">Prerequisites</span></span>
<span data-ttu-id="37bd1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37bd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37bd1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37bd1-110">Permission type</span></span>|<span data-ttu-id="37bd1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="37bd1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37bd1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37bd1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37bd1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37bd1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37bd1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37bd1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37bd1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37bd1-115">Not supported.</span></span>|
|<span data-ttu-id="37bd1-116">Application</span><span class="sxs-lookup"><span data-stu-id="37bd1-116">Application</span></span>|<span data-ttu-id="37bd1-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37bd1-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37bd1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37bd1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="37bd1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37bd1-119">Request headers</span></span>
|<span data-ttu-id="37bd1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="37bd1-120">Header</span></span>|<span data-ttu-id="37bd1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="37bd1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37bd1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="37bd1-122">Authorization</span></span>|<span data-ttu-id="37bd1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37bd1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37bd1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="37bd1-124">Accept</span></span>|<span data-ttu-id="37bd1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37bd1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37bd1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37bd1-126">Request body</span></span>
<span data-ttu-id="37bd1-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="37bd1-127">In the request body, supply a JSON representation for the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="37bd1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37bd1-128">The following table shows the properties that are required when you create the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="37bd1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37bd1-129">Property</span></span>|<span data-ttu-id="37bd1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="37bd1-130">Type</span></span>|<span data-ttu-id="37bd1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="37bd1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37bd1-132">id</span><span class="sxs-lookup"><span data-stu-id="37bd1-132">id</span></span>|<span data-ttu-id="37bd1-133">String</span><span class="sxs-lookup"><span data-stu-id="37bd1-133">String</span></span>|<span data-ttu-id="37bd1-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="37bd1-134">Key of the entity.</span></span> <span data-ttu-id="37bd1-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37bd1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="37bd1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37bd1-137">DateTimeOffset</span></span>|<span data-ttu-id="37bd1-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="37bd1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="37bd1-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="37bd1-140">roleScopeTagIds</span></span>|<span data-ttu-id="37bd1-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="37bd1-141">String collection</span></span>|<span data-ttu-id="37bd1-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="37bd1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="37bd1-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="37bd1-144">supportsScopeTags</span></span>|<span data-ttu-id="37bd1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="37bd1-145">Boolean</span></span>|<span data-ttu-id="37bd1-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="37bd1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="37bd1-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="37bd1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="37bd1-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="37bd1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="37bd1-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="37bd1-149">This property is read-only.</span></span> <span data-ttu-id="37bd1-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="37bd1-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="37bd1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="37bd1-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="37bd1-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="37bd1-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="37bd1-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="37bd1-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="37bd1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="37bd1-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="37bd1-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="37bd1-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="37bd1-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="37bd1-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="37bd1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="37bd1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="37bd1-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="37bd1-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="37bd1-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37bd1-163">createdDateTime</span></span>|<span data-ttu-id="37bd1-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37bd1-164">DateTimeOffset</span></span>|<span data-ttu-id="37bd1-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="37bd1-165">DateTime the object was created.</span></span> <span data-ttu-id="37bd1-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-167">description</span><span class="sxs-lookup"><span data-stu-id="37bd1-167">description</span></span>|<span data-ttu-id="37bd1-168">String</span><span class="sxs-lookup"><span data-stu-id="37bd1-168">String</span></span>|<span data-ttu-id="37bd1-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="37bd1-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="37bd1-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-171">displayName</span><span class="sxs-lookup"><span data-stu-id="37bd1-171">displayName</span></span>|<span data-ttu-id="37bd1-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="37bd1-172">String</span></span>|<span data-ttu-id="37bd1-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="37bd1-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="37bd1-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-175">versão</span><span class="sxs-lookup"><span data-stu-id="37bd1-175">version</span></span>|<span data-ttu-id="37bd1-176">Int32</span><span class="sxs-lookup"><span data-stu-id="37bd1-176">Int32</span></span>|<span data-ttu-id="37bd1-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="37bd1-177">Version of the device configuration.</span></span> <span data-ttu-id="37bd1-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-179">NetworkName</span><span class="sxs-lookup"><span data-stu-id="37bd1-179">networkName</span></span>|<span data-ttu-id="37bd1-180">String</span><span class="sxs-lookup"><span data-stu-id="37bd1-180">String</span></span>|<span data-ttu-id="37bd1-181">Nome da rede herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-181">Network Name Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-182">SSID</span><span class="sxs-lookup"><span data-stu-id="37bd1-182">ssid</span></span>|<span data-ttu-id="37bd1-183">String</span><span class="sxs-lookup"><span data-stu-id="37bd1-183">String</span></span>|<span data-ttu-id="37bd1-184">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="37bd1-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="37bd1-185">Herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-185">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="37bd1-186">connectAutomatically</span></span>|<span data-ttu-id="37bd1-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="37bd1-187">Boolean</span></span>|<span data-ttu-id="37bd1-188">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="37bd1-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="37bd1-189">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="37bd1-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="37bd1-190">Herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-190">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="37bd1-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="37bd1-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="37bd1-192">Boolean</span></span>|<span data-ttu-id="37bd1-193">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="37bd1-193">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="37bd1-194">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="37bd1-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="37bd1-195">Herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-195">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-196">à</span><span class="sxs-lookup"><span data-stu-id="37bd1-196">wiFiSecurityType</span></span>|[<span data-ttu-id="37bd1-197">à</span><span class="sxs-lookup"><span data-stu-id="37bd1-197">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="37bd1-198">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="37bd1-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="37bd1-199">Herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37bd1-199">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="37bd1-200">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="37bd1-200">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="37bd1-201">proxySettings</span><span class="sxs-lookup"><span data-stu-id="37bd1-201">proxySettings</span></span>|[<span data-ttu-id="37bd1-202">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="37bd1-202">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="37bd1-203">Tipo de proxy para esta conexão Wi-Fi herdada de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="37bd1-203">Proxy Type for this Wi-Fi connection Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="37bd1-204">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="37bd1-204">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="37bd1-205">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="37bd1-205">proxyManualAddress</span></span>|<span data-ttu-id="37bd1-206">String</span><span class="sxs-lookup"><span data-stu-id="37bd1-206">String</span></span>|<span data-ttu-id="37bd1-207">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="37bd1-207">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="37bd1-208">Herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-208">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-209">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="37bd1-209">proxyManualPort</span></span>|<span data-ttu-id="37bd1-210">Int32</span><span class="sxs-lookup"><span data-stu-id="37bd1-210">Int32</span></span>|<span data-ttu-id="37bd1-211">Porta do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="37bd1-211">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="37bd1-212">Herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-212">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-213">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="37bd1-213">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="37bd1-214">String</span><span class="sxs-lookup"><span data-stu-id="37bd1-214">String</span></span>|<span data-ttu-id="37bd1-215">URL do script de configuração automática do servidor proxy quando a configuração automática estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="37bd1-215">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="37bd1-216">Essa URL normalmente é o local do Arquivo PAC (configuração automática de proxy).</span><span class="sxs-lookup"><span data-stu-id="37bd1-216">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="37bd1-217">Herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-217">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-218">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="37bd1-218">preSharedKey</span></span>|<span data-ttu-id="37bd1-219">String</span><span class="sxs-lookup"><span data-stu-id="37bd1-219">String</span></span>|<span data-ttu-id="37bd1-220">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="37bd1-220">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="37bd1-221">Herdado de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37bd1-221">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="37bd1-222">eapType</span><span class="sxs-lookup"><span data-stu-id="37bd1-222">eapType</span></span>|[<span data-ttu-id="37bd1-223">eapType</span><span class="sxs-lookup"><span data-stu-id="37bd1-223">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="37bd1-224">EAP (protocolo de autenticação extensível).</span><span class="sxs-lookup"><span data-stu-id="37bd1-224">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="37bd1-225">Indica o tipo de protocolo EAP definido no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="37bd1-225">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="37bd1-226">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="37bd1-226">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="37bd1-227">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="37bd1-227">eapFastConfiguration</span></span>|[<span data-ttu-id="37bd1-228">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="37bd1-228">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="37bd1-229">Opção de configuração EAP-FAST quando EAP-FAST for o tipo de EAP selecionado.</span><span class="sxs-lookup"><span data-stu-id="37bd1-229">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="37bd1-230">Os valores possíveis são: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="37bd1-230">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="37bd1-231">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="37bd1-231">trustedServerCertificateNames</span></span>|<span data-ttu-id="37bd1-232">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="37bd1-232">String collection</span></span>|<span data-ttu-id="37bd1-233">Nomes de certificados de servidor confiáveis quando o tipo EAP é configurado como EAP-TLS/TTLS/FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="37bd1-233">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="37bd1-234">Este é o nome comum usado nos certificados emitidos pela autoridade de certificação (CA) confiável.</span><span class="sxs-lookup"><span data-stu-id="37bd1-234">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="37bd1-235">Se você fornecer essas informações, poderá ignorar a caixa de diálogo de confiança dinâmica exibida em dispositivos de usuários finais quando eles se conectam a esta rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="37bd1-235">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="37bd1-236">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="37bd1-236">authenticationMethod</span></span>|[<span data-ttu-id="37bd1-237">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="37bd1-237">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="37bd1-238">Método de autenticação quando o tipo EAP é configurado como PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="37bd1-238">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="37bd1-239">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="37bd1-239">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="37bd1-240">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="37bd1-240">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="37bd1-241">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="37bd1-241">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="37bd1-242">Método não EAP para autenticação (identidade interna) quando o tipo EAP é EAP-TTLS e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="37bd1-242">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="37bd1-243">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="37bd1-243">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="37bd1-244">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="37bd1-244">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="37bd1-245">String</span><span class="sxs-lookup"><span data-stu-id="37bd1-245">String</span></span>|<span data-ttu-id="37bd1-246">Habilitar Privacidade de identidade (identidade externa) quando o tipo EAP é configurado como EAP-TTLS, EAP-FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="37bd1-246">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="37bd1-247">Essa propriedade mascara os nomes de usernames com o texto inserido.</span><span class="sxs-lookup"><span data-stu-id="37bd1-247">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="37bd1-248">Por exemplo, se você usar ' anônimo ', cada usuário que autenticar com essa conexão Wi-Fi usando seu nome de usuário real será exibido como ' anônimo '.</span><span class="sxs-lookup"><span data-stu-id="37bd1-248">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="37bd1-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="37bd1-249">Response</span></span>
<span data-ttu-id="37bd1-250">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37bd1-250">If successful, this method returns a `200 OK` response code and an updated [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37bd1-251">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37bd1-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="37bd1-252">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37bd1-252">Request</span></span>
<span data-ttu-id="37bd1-253">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37bd1-253">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37bd1-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="37bd1-254">Response</span></span>
<span data-ttu-id="37bd1-p128">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37bd1-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




