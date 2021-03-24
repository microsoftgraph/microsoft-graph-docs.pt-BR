---
title: Criar windowsWifiConfiguration
description: Crie um novo objeto windowsWifiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 82b784c82d66c684ac0afac32e9bf490fc26aaaf
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131033"
---
# <a name="create-windowswificonfiguration"></a><span data-ttu-id="b2d11-103">Criar windowsWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="b2d11-103">Create windowsWifiConfiguration</span></span>

<span data-ttu-id="b2d11-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2d11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2d11-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b2d11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2d11-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b2d11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2d11-107">Crie um novo [objeto windowsWifiConfiguration.](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2d11-107">Create a new [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2d11-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b2d11-108">Prerequisites</span></span>
<span data-ttu-id="b2d11-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2d11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2d11-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b2d11-111">Permission type</span></span>|<span data-ttu-id="b2d11-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b2d11-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2d11-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b2d11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2d11-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2d11-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2d11-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b2d11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2d11-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b2d11-116">Not supported.</span></span>|
|<span data-ttu-id="b2d11-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b2d11-117">Application</span></span>|<span data-ttu-id="b2d11-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2d11-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2d11-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b2d11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b2d11-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d11-120">Request headers</span></span>
|<span data-ttu-id="b2d11-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b2d11-121">Header</span></span>|<span data-ttu-id="b2d11-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b2d11-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2d11-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b2d11-123">Authorization</span></span>|<span data-ttu-id="b2d11-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b2d11-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2d11-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b2d11-125">Accept</span></span>|<span data-ttu-id="b2d11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2d11-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2d11-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d11-127">Request body</span></span>
<span data-ttu-id="b2d11-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b2d11-128">In the request body, supply a JSON representation for the windowsWifiConfiguration object.</span></span>

<span data-ttu-id="b2d11-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o windowsWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b2d11-129">The following table shows the properties that are required when you create the windowsWifiConfiguration.</span></span>

|<span data-ttu-id="b2d11-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b2d11-130">Property</span></span>|<span data-ttu-id="b2d11-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2d11-131">Type</span></span>|<span data-ttu-id="b2d11-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2d11-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2d11-133">id</span><span class="sxs-lookup"><span data-stu-id="b2d11-133">id</span></span>|<span data-ttu-id="b2d11-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2d11-134">String</span></span>|<span data-ttu-id="b2d11-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b2d11-135">Key of the entity.</span></span> <span data-ttu-id="b2d11-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2d11-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2d11-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2d11-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b2d11-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2d11-138">DateTimeOffset</span></span>|<span data-ttu-id="b2d11-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b2d11-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b2d11-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2d11-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2d11-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b2d11-141">roleScopeTagIds</span></span>|<span data-ttu-id="b2d11-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2d11-142">String collection</span></span>|<span data-ttu-id="b2d11-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="b2d11-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b2d11-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2d11-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2d11-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b2d11-145">supportsScopeTags</span></span>|<span data-ttu-id="b2d11-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="b2d11-146">Boolean</span></span>|<span data-ttu-id="b2d11-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b2d11-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b2d11-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b2d11-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b2d11-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b2d11-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b2d11-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b2d11-150">This property is read-only.</span></span> <span data-ttu-id="b2d11-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2d11-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2d11-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b2d11-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b2d11-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b2d11-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b2d11-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="b2d11-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b2d11-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2d11-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2d11-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b2d11-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b2d11-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b2d11-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b2d11-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="b2d11-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b2d11-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2d11-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2d11-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b2d11-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b2d11-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b2d11-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b2d11-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="b2d11-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b2d11-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2d11-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2d11-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2d11-164">createdDateTime</span></span>|<span data-ttu-id="b2d11-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2d11-165">DateTimeOffset</span></span>|<span data-ttu-id="b2d11-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b2d11-166">DateTime the object was created.</span></span> <span data-ttu-id="b2d11-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2d11-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2d11-168">descrição</span><span class="sxs-lookup"><span data-stu-id="b2d11-168">description</span></span>|<span data-ttu-id="b2d11-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2d11-169">String</span></span>|<span data-ttu-id="b2d11-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2d11-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b2d11-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2d11-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2d11-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b2d11-172">displayName</span></span>|<span data-ttu-id="b2d11-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2d11-173">String</span></span>|<span data-ttu-id="b2d11-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2d11-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b2d11-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2d11-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2d11-176">versão</span><span class="sxs-lookup"><span data-stu-id="b2d11-176">version</span></span>|<span data-ttu-id="b2d11-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b2d11-177">Int32</span></span>|<span data-ttu-id="b2d11-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b2d11-178">Version of the device configuration.</span></span> <span data-ttu-id="b2d11-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b2d11-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b2d11-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="b2d11-180">preSharedKey</span></span>|<span data-ttu-id="b2d11-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2d11-181">String</span></span>|<span data-ttu-id="b2d11-182">Esta é a chave pré-compartilhada para a rede WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b2d11-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="b2d11-183">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b2d11-183">wifiSecurityType</span></span>|[<span data-ttu-id="b2d11-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b2d11-184">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="b2d11-185">Especifique o Tipo de Segurança Wifi.</span><span class="sxs-lookup"><span data-stu-id="b2d11-185">Specify the Wifi Security Type.</span></span> <span data-ttu-id="b2d11-186">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="b2d11-186">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="b2d11-187">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="b2d11-187">meteredConnectionLimit</span></span>|[<span data-ttu-id="b2d11-188">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="b2d11-188">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="b2d11-189">Especifique o tipo de limite de conexão limitado para a conexão wifi.</span><span class="sxs-lookup"><span data-stu-id="b2d11-189">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="b2d11-190">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="b2d11-190">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="b2d11-191">ssid</span><span class="sxs-lookup"><span data-stu-id="b2d11-191">ssid</span></span>|<span data-ttu-id="b2d11-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2d11-192">String</span></span>|<span data-ttu-id="b2d11-193">Especifique o SSID da conexão wifi.</span><span class="sxs-lookup"><span data-stu-id="b2d11-193">Specify the SSID of the wifi connection.</span></span>|
|<span data-ttu-id="b2d11-194">networkName</span><span class="sxs-lookup"><span data-stu-id="b2d11-194">networkName</span></span>|<span data-ttu-id="b2d11-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2d11-195">String</span></span>|<span data-ttu-id="b2d11-196">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="b2d11-196">Specify the network configuration name.</span></span>|
|<span data-ttu-id="b2d11-197">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="b2d11-197">connectAutomatically</span></span>|<span data-ttu-id="b2d11-198">Booleano</span><span class="sxs-lookup"><span data-stu-id="b2d11-198">Boolean</span></span>|<span data-ttu-id="b2d11-199">Especifique se a conexão wifi deve se conectar automaticamente quando estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="b2d11-199">Specify whether the wifi connection should connect automatically when in range.</span></span>|
|<span data-ttu-id="b2d11-200">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="b2d11-200">connectToPreferredNetwork</span></span>|<span data-ttu-id="b2d11-201">Booleano</span><span class="sxs-lookup"><span data-stu-id="b2d11-201">Boolean</span></span>|<span data-ttu-id="b2d11-202">Especifique se a conexão wifi deve se conectar a redes mais preferenciais quando já estiver conectada a essa.</span><span class="sxs-lookup"><span data-stu-id="b2d11-202">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="b2d11-203">Requer Que ConnectAutomatically seja verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="b2d11-203">Requires ConnectAutomatically to be true.</span></span>|
|<span data-ttu-id="b2d11-204">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="b2d11-204">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="b2d11-205">Booleano</span><span class="sxs-lookup"><span data-stu-id="b2d11-205">Boolean</span></span>|<span data-ttu-id="b2d11-206">Especifique se a conexão wifi deve se conectar automaticamente mesmo quando o SSID não estiver transmitindo.</span><span class="sxs-lookup"><span data-stu-id="b2d11-206">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span>|
|<span data-ttu-id="b2d11-207">proxySetting</span><span class="sxs-lookup"><span data-stu-id="b2d11-207">proxySetting</span></span>|[<span data-ttu-id="b2d11-208">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="b2d11-208">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="b2d11-209">Especifique a configuração de proxy Wi-Fi configuração.</span><span class="sxs-lookup"><span data-stu-id="b2d11-209">Specify the proxy setting for Wi-Fi configuration.</span></span> <span data-ttu-id="b2d11-210">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="b2d11-210">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="b2d11-211">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="b2d11-211">proxyManualAddress</span></span>|<span data-ttu-id="b2d11-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2d11-212">String</span></span>|<span data-ttu-id="b2d11-213">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="b2d11-213">Specify the IP address for the proxy server.</span></span>|
|<span data-ttu-id="b2d11-214">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="b2d11-214">proxyManualPort</span></span>|<span data-ttu-id="b2d11-215">Int32</span><span class="sxs-lookup"><span data-stu-id="b2d11-215">Int32</span></span>|<span data-ttu-id="b2d11-216">Especifique a porta para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="b2d11-216">Specify the port for the proxy server.</span></span>|
|<span data-ttu-id="b2d11-217">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="b2d11-217">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="b2d11-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b2d11-218">String</span></span>|<span data-ttu-id="b2d11-219">Especifique a URL do script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="b2d11-219">Specify the URL for the proxy server configuration script.</span></span>|
|<span data-ttu-id="b2d11-220">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="b2d11-220">forceFIPSCompliance</span></span>|<span data-ttu-id="b2d11-221">Booleano</span><span class="sxs-lookup"><span data-stu-id="b2d11-221">Boolean</span></span>|<span data-ttu-id="b2d11-222">Especifique se deve forçar a conformidade fips.</span><span class="sxs-lookup"><span data-stu-id="b2d11-222">Specify whether to force FIPS compliance.</span></span>|



## <a name="response"></a><span data-ttu-id="b2d11-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2d11-223">Response</span></span>
<span data-ttu-id="b2d11-224">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b2d11-224">If successful, this method returns a `201 Created` response code and a [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2d11-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b2d11-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2d11-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b2d11-226">Request</span></span>
<span data-ttu-id="b2d11-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2d11-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1559

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
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
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```

### <a name="response"></a><span data-ttu-id="b2d11-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="b2d11-228">Response</span></span>
<span data-ttu-id="b2d11-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b2d11-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1731

{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "id": "8a9e790f-790f-8a9e-0f79-9e8a0f799e8a",
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
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true
}
```




