---
title: Atualizar windowsWifiEnterpriseEAPConfiguration
description: Atualiza as propriedades de um objeto windowsWifiEnterpriseEAPConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ed2afd7f75ebdec5aa334096e0e3e211daab0a94
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49311291"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="992cd-103">Atualizar windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="992cd-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

<span data-ttu-id="992cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="992cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="992cd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="992cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="992cd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="992cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="992cd-107">Atualiza as propriedades de um objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="992cd-107">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="992cd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="992cd-108">Prerequisites</span></span>
<span data-ttu-id="992cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="992cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="992cd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="992cd-111">Permission type</span></span>|<span data-ttu-id="992cd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="992cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="992cd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="992cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="992cd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="992cd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="992cd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="992cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="992cd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="992cd-116">Not supported.</span></span>|
|<span data-ttu-id="992cd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="992cd-117">Application</span></span>|<span data-ttu-id="992cd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="992cd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="992cd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="992cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="992cd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="992cd-120">Request headers</span></span>
|<span data-ttu-id="992cd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="992cd-121">Header</span></span>|<span data-ttu-id="992cd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="992cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="992cd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="992cd-123">Authorization</span></span>|<span data-ttu-id="992cd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="992cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="992cd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="992cd-125">Accept</span></span>|<span data-ttu-id="992cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="992cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="992cd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="992cd-127">Request body</span></span>
<span data-ttu-id="992cd-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="992cd-128">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="992cd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="992cd-129">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="992cd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="992cd-130">Property</span></span>|<span data-ttu-id="992cd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="992cd-131">Type</span></span>|<span data-ttu-id="992cd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="992cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="992cd-133">id</span><span class="sxs-lookup"><span data-stu-id="992cd-133">id</span></span>|<span data-ttu-id="992cd-134">String</span><span class="sxs-lookup"><span data-stu-id="992cd-134">String</span></span>|<span data-ttu-id="992cd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="992cd-135">Key of the entity.</span></span> <span data-ttu-id="992cd-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="992cd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="992cd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="992cd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="992cd-138">DateTimeOffset</span></span>|<span data-ttu-id="992cd-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="992cd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="992cd-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="992cd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="992cd-141">roleScopeTagIds</span></span>|<span data-ttu-id="992cd-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="992cd-142">String collection</span></span>|<span data-ttu-id="992cd-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="992cd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="992cd-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="992cd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="992cd-145">supportsScopeTags</span></span>|<span data-ttu-id="992cd-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="992cd-146">Boolean</span></span>|<span data-ttu-id="992cd-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="992cd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="992cd-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="992cd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="992cd-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="992cd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="992cd-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="992cd-150">This property is read-only.</span></span> <span data-ttu-id="992cd-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="992cd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="992cd-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="992cd-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="992cd-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="992cd-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="992cd-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="992cd-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="992cd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="992cd-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="992cd-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="992cd-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="992cd-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="992cd-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="992cd-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="992cd-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="992cd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="992cd-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="992cd-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="992cd-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="992cd-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="992cd-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="992cd-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="992cd-164">createdDateTime</span></span>|<span data-ttu-id="992cd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="992cd-165">DateTimeOffset</span></span>|<span data-ttu-id="992cd-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="992cd-166">DateTime the object was created.</span></span> <span data-ttu-id="992cd-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="992cd-168">description</span><span class="sxs-lookup"><span data-stu-id="992cd-168">description</span></span>|<span data-ttu-id="992cd-169">String</span><span class="sxs-lookup"><span data-stu-id="992cd-169">String</span></span>|<span data-ttu-id="992cd-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="992cd-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="992cd-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="992cd-172">displayName</span><span class="sxs-lookup"><span data-stu-id="992cd-172">displayName</span></span>|<span data-ttu-id="992cd-173">String</span><span class="sxs-lookup"><span data-stu-id="992cd-173">String</span></span>|<span data-ttu-id="992cd-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="992cd-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="992cd-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="992cd-176">versão</span><span class="sxs-lookup"><span data-stu-id="992cd-176">version</span></span>|<span data-ttu-id="992cd-177">Int32</span><span class="sxs-lookup"><span data-stu-id="992cd-177">Int32</span></span>|<span data-ttu-id="992cd-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="992cd-178">Version of the device configuration.</span></span> <span data-ttu-id="992cd-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="992cd-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="992cd-180">preSharedKey</span></span>|<span data-ttu-id="992cd-181">String</span><span class="sxs-lookup"><span data-stu-id="992cd-181">String</span></span>|<span data-ttu-id="992cd-182">Esta é a chave pré-compartilhada para a rede WPA de Wi-Fi pessoal.</span><span class="sxs-lookup"><span data-stu-id="992cd-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="992cd-183">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-183">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="992cd-184">à</span><span class="sxs-lookup"><span data-stu-id="992cd-184">wifiSecurityType</span></span>|[<span data-ttu-id="992cd-185">à</span><span class="sxs-lookup"><span data-stu-id="992cd-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="992cd-186">Especifique o tipo de segurança wifi.</span><span class="sxs-lookup"><span data-stu-id="992cd-186">Specify the Wifi Security Type.</span></span> <span data-ttu-id="992cd-187">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="992cd-187">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="992cd-188">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="992cd-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="992cd-189">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="992cd-189">meteredConnectionLimit</span></span>|[<span data-ttu-id="992cd-190">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="992cd-190">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="992cd-191">Especifique o tipo de limite de conexão limitada para a conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="992cd-191">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="992cd-192">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="992cd-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="992cd-193">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="992cd-193">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="992cd-194">SSID</span><span class="sxs-lookup"><span data-stu-id="992cd-194">ssid</span></span>|<span data-ttu-id="992cd-195">String</span><span class="sxs-lookup"><span data-stu-id="992cd-195">String</span></span>|<span data-ttu-id="992cd-196">Especifique o SSID da conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="992cd-196">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="992cd-197">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="992cd-198">NetworkName</span><span class="sxs-lookup"><span data-stu-id="992cd-198">networkName</span></span>|<span data-ttu-id="992cd-199">String</span><span class="sxs-lookup"><span data-stu-id="992cd-199">String</span></span>|<span data-ttu-id="992cd-200">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="992cd-200">Specify the network configuration name.</span></span> <span data-ttu-id="992cd-201">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="992cd-202">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="992cd-202">connectAutomatically</span></span>|<span data-ttu-id="992cd-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="992cd-203">Boolean</span></span>|<span data-ttu-id="992cd-204">Especifique se a conexão WiFi deve se conectar automaticamente quando estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="992cd-204">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="992cd-205">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-205">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="992cd-206">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="992cd-206">connectToPreferredNetwork</span></span>|<span data-ttu-id="992cd-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="992cd-207">Boolean</span></span>|<span data-ttu-id="992cd-208">Especifique se a conexão WiFi deve se conectar a redes mais preferenciais quando já estiver conectado a ela.</span><span class="sxs-lookup"><span data-stu-id="992cd-208">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="992cd-209">Requer que ConnectAutomatically seja true.</span><span class="sxs-lookup"><span data-stu-id="992cd-209">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="992cd-210">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="992cd-211">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="992cd-211">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="992cd-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="992cd-212">Boolean</span></span>|<span data-ttu-id="992cd-213">Especifique se a conexão WiFi deve se conectar automaticamente, mesmo quando o SSID não estiver transmitindo.</span><span class="sxs-lookup"><span data-stu-id="992cd-213">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="992cd-214">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="992cd-215">proxySetting</span><span class="sxs-lookup"><span data-stu-id="992cd-215">proxySetting</span></span>|[<span data-ttu-id="992cd-216">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="992cd-216">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="992cd-217">Especifique a configuração de proxy para a configuração de Wi-Fi herdada de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="992cd-217">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="992cd-218">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="992cd-218">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="992cd-219">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="992cd-219">proxyManualAddress</span></span>|<span data-ttu-id="992cd-220">String</span><span class="sxs-lookup"><span data-stu-id="992cd-220">String</span></span>|<span data-ttu-id="992cd-221">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="992cd-221">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="992cd-222">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="992cd-223">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="992cd-223">proxyManualPort</span></span>|<span data-ttu-id="992cd-224">Int32</span><span class="sxs-lookup"><span data-stu-id="992cd-224">Int32</span></span>|<span data-ttu-id="992cd-225">Especifique a porta do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="992cd-225">Specify the port for the proxy server.</span></span> <span data-ttu-id="992cd-226">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-226">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="992cd-227">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="992cd-227">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="992cd-228">String</span><span class="sxs-lookup"><span data-stu-id="992cd-228">String</span></span>|<span data-ttu-id="992cd-229">Especifique a URL do script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="992cd-229">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="992cd-230">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-230">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="992cd-231">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="992cd-231">forceFIPSCompliance</span></span>|<span data-ttu-id="992cd-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="992cd-232">Boolean</span></span>|<span data-ttu-id="992cd-233">Especifique se a conformidade com FIPS deve ser forçada.</span><span class="sxs-lookup"><span data-stu-id="992cd-233">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="992cd-234">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="992cd-234">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="992cd-235">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="992cd-235">networkSingleSignOn</span></span>|[<span data-ttu-id="992cd-236">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="992cd-236">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="992cd-237">Especifique o tipo de logon único na rede.</span><span class="sxs-lookup"><span data-stu-id="992cd-237">Specify the network single sign on type.</span></span> <span data-ttu-id="992cd-238">Os valores possíveis são: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="992cd-238">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="992cd-239">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="992cd-239">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="992cd-240">Int32</span><span class="sxs-lookup"><span data-stu-id="992cd-240">Int32</span></span>|<span data-ttu-id="992cd-241">Especifique o tempo limite máximo de autenticação (em segundos).</span><span class="sxs-lookup"><span data-stu-id="992cd-241">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="992cd-242">Intervalo válido: 1-120</span><span class="sxs-lookup"><span data-stu-id="992cd-242">Valid range: 1-120</span></span>|
|<span data-ttu-id="992cd-243">userBasedVirtualLan</span><span class="sxs-lookup"><span data-stu-id="992cd-243">userBasedVirtualLan</span></span>|<span data-ttu-id="992cd-244">Booliano</span><span class="sxs-lookup"><span data-stu-id="992cd-244">Boolean</span></span>|<span data-ttu-id="992cd-245">Especifique se deseja alterar a LAN virtual usada pelo dispositivo com base nas credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="992cd-245">Specifiy whether to change the virtual LAN used by the device based on the user’s credentials.</span></span> <span data-ttu-id="992cd-246">Não pode ser usado quando NetworkSingleSignOnType está definido como desabilitado.</span><span class="sxs-lookup"><span data-stu-id="992cd-246">Cannot be used when NetworkSingleSignOnType is set to Disabled.</span></span>|
|<span data-ttu-id="992cd-247">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="992cd-247">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="992cd-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="992cd-248">Boolean</span></span>|<span data-ttu-id="992cd-249">Especifique se a conexão WiFi deve solicitar credenciais de autenticação adicionais.</span><span class="sxs-lookup"><span data-stu-id="992cd-249">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="992cd-250">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="992cd-250">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="992cd-251">Booliano</span><span class="sxs-lookup"><span data-stu-id="992cd-251">Boolean</span></span>|<span data-ttu-id="992cd-252">Especifique se a conexão WiFi deve habilitar o cache da chave mestra de par.</span><span class="sxs-lookup"><span data-stu-id="992cd-252">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="992cd-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="992cd-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="992cd-254">Int32</span><span class="sxs-lookup"><span data-stu-id="992cd-254">Int32</span></span>|<span data-ttu-id="992cd-255">Especifique o tempo máximo de cache da chave mestra de paridade (em minutos).</span><span class="sxs-lookup"><span data-stu-id="992cd-255">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="992cd-256">Intervalo válido: 5-1440</span><span class="sxs-lookup"><span data-stu-id="992cd-256">Valid range: 5-1440</span></span>|
|<span data-ttu-id="992cd-257">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="992cd-257">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="992cd-258">Int32</span><span class="sxs-lookup"><span data-stu-id="992cd-258">Int32</span></span>|<span data-ttu-id="992cd-259">Especifique o número máximo de chaves de mestre emparelhadas no cache.</span><span class="sxs-lookup"><span data-stu-id="992cd-259">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="992cd-260">Intervalo válido: 1-255</span><span class="sxs-lookup"><span data-stu-id="992cd-260">Valid range: 1-255</span></span>|
|<span data-ttu-id="992cd-261">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="992cd-261">enablePreAuthentication</span></span>|<span data-ttu-id="992cd-262">Booliano</span><span class="sxs-lookup"><span data-stu-id="992cd-262">Boolean</span></span>|<span data-ttu-id="992cd-263">Especifique se a pré-autenticação deve ser habilitada.</span><span class="sxs-lookup"><span data-stu-id="992cd-263">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="992cd-264">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="992cd-264">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="992cd-265">Int32</span><span class="sxs-lookup"><span data-stu-id="992cd-265">Int32</span></span>|<span data-ttu-id="992cd-266">Especifique as tentativas máximas de pré-autenticação.</span><span class="sxs-lookup"><span data-stu-id="992cd-266">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="992cd-267">Intervalo válido: 1-16</span><span class="sxs-lookup"><span data-stu-id="992cd-267">Valid range: 1-16</span></span>|
|<span data-ttu-id="992cd-268">eapType</span><span class="sxs-lookup"><span data-stu-id="992cd-268">eapType</span></span>|[<span data-ttu-id="992cd-269">eapType</span><span class="sxs-lookup"><span data-stu-id="992cd-269">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="992cd-270">EAP (protocolo de autenticação extensível).</span><span class="sxs-lookup"><span data-stu-id="992cd-270">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="992cd-271">Indica o tipo de protocolo EAP definido no ponto de extremidade de Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="992cd-271">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="992cd-272">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="992cd-272">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="992cd-273">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="992cd-273">trustedServerCertificateNames</span></span>|<span data-ttu-id="992cd-274">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="992cd-274">String collection</span></span>|<span data-ttu-id="992cd-275">Especificar nomes de certificado de servidor confiável.</span><span class="sxs-lookup"><span data-stu-id="992cd-275">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="992cd-276">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="992cd-276">authenticationMethod</span></span>|[<span data-ttu-id="992cd-277">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="992cd-277">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="992cd-278">Especifique o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="992cd-278">Specify the authentication method.</span></span> <span data-ttu-id="992cd-279">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="992cd-279">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="992cd-280">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="992cd-280">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="992cd-281">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="992cd-281">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="992cd-282">Especificar o protocolo de autenticação interna para EAP TTLS.</span><span class="sxs-lookup"><span data-stu-id="992cd-282">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="992cd-283">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="992cd-283">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="992cd-284">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="992cd-284">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="992cd-285">String</span><span class="sxs-lookup"><span data-stu-id="992cd-285">String</span></span>|<span data-ttu-id="992cd-286">Especifique a cadeia de caracteres para substituir os nomes de texto para privacidade ao usar EAP TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="992cd-286">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|
|<span data-ttu-id="992cd-287">requireCryptographicBinding</span><span class="sxs-lookup"><span data-stu-id="992cd-287">requireCryptographicBinding</span></span>|<span data-ttu-id="992cd-288">Booliano</span><span class="sxs-lookup"><span data-stu-id="992cd-288">Boolean</span></span>|<span data-ttu-id="992cd-289">Especifique se deseja habilitar a associação criptográfica quando o tipo EAP for selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="992cd-289">Specify whether to enable cryptographic binding when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="992cd-290">performServerValidation</span><span class="sxs-lookup"><span data-stu-id="992cd-290">performServerValidation</span></span>|<span data-ttu-id="992cd-291">Booliano</span><span class="sxs-lookup"><span data-stu-id="992cd-291">Boolean</span></span>|<span data-ttu-id="992cd-292">Especifique se deseja habilitar a verificação da identidade do servidor, validando o certificado quando o tipo EAP estiver selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="992cd-292">Specify whether to enable verification of server's identity by validating the certificate when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="992cd-293">disableUserPromptForServerValidation</span><span class="sxs-lookup"><span data-stu-id="992cd-293">disableUserPromptForServerValidation</span></span>|<span data-ttu-id="992cd-294">Booliano</span><span class="sxs-lookup"><span data-stu-id="992cd-294">Boolean</span></span>|<span data-ttu-id="992cd-295">Especifique se deseja impedir que o usuário seja solicitado a autorizar novos servidores para autoridades de certificação confiáveis quando o tipo EAP for selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="992cd-295">Specify whether to prevent the user from being prompted to authorize new servers for trusted certification authorities when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="992cd-296">authenticationPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="992cd-296">authenticationPeriodInSeconds</span></span>|<span data-ttu-id="992cd-297">Int32</span><span class="sxs-lookup"><span data-stu-id="992cd-297">Int32</span></span>|<span data-ttu-id="992cd-298">Especifique o número de segundos que o cliente deve aguardar após uma tentativa de autenticação antes de falhar.</span><span class="sxs-lookup"><span data-stu-id="992cd-298">Specify the number of seconds for the client to wait after an authentication attempt before failing.</span></span> <span data-ttu-id="992cd-299">Intervalo válido de 1-3600.</span><span class="sxs-lookup"><span data-stu-id="992cd-299">Valid range 1-3600.</span></span>|
|<span data-ttu-id="992cd-300">authenticationRetryDelayPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="992cd-300">authenticationRetryDelayPeriodInSeconds</span></span>|<span data-ttu-id="992cd-301">Int32</span><span class="sxs-lookup"><span data-stu-id="992cd-301">Int32</span></span>|<span data-ttu-id="992cd-302">Especifique o número de segundos entre uma falha de autenticação e a próxima tentativa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="992cd-302">Specify the number of seconds between a failed authentication and the next authentication attempt.</span></span> <span data-ttu-id="992cd-303">Intervalo válido de 1-3600.</span><span class="sxs-lookup"><span data-stu-id="992cd-303">Valid range 1-3600.</span></span>|
|<span data-ttu-id="992cd-304">eapolStartPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="992cd-304">eapolStartPeriodInSeconds</span></span>|<span data-ttu-id="992cd-305">Int32</span><span class="sxs-lookup"><span data-stu-id="992cd-305">Int32</span></span>|<span data-ttu-id="992cd-306">Especifique o número de segundos de espera antes de enviar uma mensagem de início de EAPOL (protocolo de autenticação extensível via LAN).</span><span class="sxs-lookup"><span data-stu-id="992cd-306">Specify the number of seconds to wait before sending an EAPOL (Extensible Authentication Protocol over LAN) Start message.</span></span> <span data-ttu-id="992cd-307">Intervalo válido de 1-3600.</span><span class="sxs-lookup"><span data-stu-id="992cd-307">Valid range 1-3600.</span></span>|
|<span data-ttu-id="992cd-308">maximumEAPOLStartMessages</span><span class="sxs-lookup"><span data-stu-id="992cd-308">maximumEAPOLStartMessages</span></span>|<span data-ttu-id="992cd-309">Int32</span><span class="sxs-lookup"><span data-stu-id="992cd-309">Int32</span></span>|<span data-ttu-id="992cd-310">Especifique o número máximo de mensagens de início de EAPOL (Extensible Authentication Protocol over LAN) para serem enviadas antes de retornar uma falha.</span><span class="sxs-lookup"><span data-stu-id="992cd-310">Specifiy the maximum number of EAPOL (Extensible Authentication Protocol over LAN) Start messages to be sent before returning failure.</span></span> <span data-ttu-id="992cd-311">Intervalo válido de 1-100.</span><span class="sxs-lookup"><span data-stu-id="992cd-311">Valid range 1-100.</span></span>|
|<span data-ttu-id="992cd-312">maximumAuthenticationFailures</span><span class="sxs-lookup"><span data-stu-id="992cd-312">maximumAuthenticationFailures</span></span>|<span data-ttu-id="992cd-313">Int32</span><span class="sxs-lookup"><span data-stu-id="992cd-313">Int32</span></span>|<span data-ttu-id="992cd-314">Especifique as falhas máximas de autenticação permitidas para um conjunto de credenciais.</span><span class="sxs-lookup"><span data-stu-id="992cd-314">Specify the maximum authentication failures allowed for a set of credentials.</span></span> <span data-ttu-id="992cd-315">Intervalo válido de 1-100.</span><span class="sxs-lookup"><span data-stu-id="992cd-315">Valid range 1-100.</span></span>|
|<span data-ttu-id="992cd-316">cacheCredentials</span><span class="sxs-lookup"><span data-stu-id="992cd-316">cacheCredentials</span></span>|<span data-ttu-id="992cd-317">Booliano</span><span class="sxs-lookup"><span data-stu-id="992cd-317">Boolean</span></span>|<span data-ttu-id="992cd-318">Especifique se deseja armazenar em cache credenciais de usuário no dispositivo para que os usuários não precisem inseri-las sempre que se conectarem.</span><span class="sxs-lookup"><span data-stu-id="992cd-318">Specify whether to cache user credentials on the device so that users don’t need to keep entering them each time they connect.</span></span>|
|<span data-ttu-id="992cd-319">authenticationType</span><span class="sxs-lookup"><span data-stu-id="992cd-319">authenticationType</span></span>|[<span data-ttu-id="992cd-320">wifiAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="992cd-320">wifiAuthenticationType</span></span>](../resources/intune-deviceconfig-wifiauthenticationtype.md)|<span data-ttu-id="992cd-321">Especifique se deseja autenticar o usuário, o dispositivo, ou para usar a autenticação de convidado (nenhuma).</span><span class="sxs-lookup"><span data-stu-id="992cd-321">Specify whether to authenticate the user, the device, either, or to use guest authentication (none).</span></span> <span data-ttu-id="992cd-322">Se você estiver usando a autenticação de certificado, certifique-se de que o tipo de certificado corresponde ao tipo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="992cd-322">If you’re using certificate authentication, make sure the certificate type matches the authentication type.</span></span> <span data-ttu-id="992cd-323">Os valores possíveis são: `none`, `user`, `machine`, `machineOrUser`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="992cd-323">Possible values are: `none`, `user`, `machine`, `machineOrUser`, `guest`.</span></span>|



## <a name="response"></a><span data-ttu-id="992cd-324">Resposta</span><span class="sxs-lookup"><span data-stu-id="992cd-324">Response</span></span>
<span data-ttu-id="992cd-325">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="992cd-325">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="992cd-326">Exemplo</span><span class="sxs-lookup"><span data-stu-id="992cd-326">Example</span></span>

### <a name="request"></a><span data-ttu-id="992cd-327">Solicitação</span><span class="sxs-lookup"><span data-stu-id="992cd-327">Request</span></span>
<span data-ttu-id="992cd-328">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="992cd-328">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2695

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
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
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "userBasedVirtualLan": true,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "requireCryptographicBinding": true,
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "authenticationPeriodInSeconds": 13,
  "authenticationRetryDelayPeriodInSeconds": 7,
  "eapolStartPeriodInSeconds": 9,
  "maximumEAPOLStartMessages": 9,
  "maximumAuthenticationFailures": 13,
  "cacheCredentials": true,
  "authenticationType": "user"
}
```

### <a name="response"></a><span data-ttu-id="992cd-329">Resposta</span><span class="sxs-lookup"><span data-stu-id="992cd-329">Response</span></span>
<span data-ttu-id="992cd-p141">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="992cd-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2867

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
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
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "userBasedVirtualLan": true,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "requireCryptographicBinding": true,
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true,
  "authenticationPeriodInSeconds": 13,
  "authenticationRetryDelayPeriodInSeconds": 7,
  "eapolStartPeriodInSeconds": 9,
  "maximumEAPOLStartMessages": 9,
  "maximumAuthenticationFailures": 13,
  "cacheCredentials": true,
  "authenticationType": "user"
}
```




