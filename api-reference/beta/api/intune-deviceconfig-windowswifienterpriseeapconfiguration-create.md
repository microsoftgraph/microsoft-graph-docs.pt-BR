---
title: Criar windowsWifiEnterpriseEAPConfiguration
description: Criar um novo objeto windowsWifiEnterpriseEAPConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f728e6b5c2f20ae39a8f7a58002bc70da02d33b3
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37532138"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="85184-103">Criar windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="85184-103">Create windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="85184-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="85184-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85184-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="85184-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85184-106">Criar um novo objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="85184-106">Create a new [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85184-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="85184-107">Prerequisites</span></span>
<span data-ttu-id="85184-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85184-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85184-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85184-110">Permission type</span></span>|<span data-ttu-id="85184-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="85184-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85184-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85184-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85184-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85184-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85184-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85184-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85184-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85184-115">Not supported.</span></span>|
|<span data-ttu-id="85184-116">Application</span><span class="sxs-lookup"><span data-stu-id="85184-116">Application</span></span>|<span data-ttu-id="85184-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85184-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85184-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85184-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="85184-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85184-119">Request headers</span></span>
|<span data-ttu-id="85184-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85184-120">Header</span></span>|<span data-ttu-id="85184-121">Valor</span><span class="sxs-lookup"><span data-stu-id="85184-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85184-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="85184-122">Authorization</span></span>|<span data-ttu-id="85184-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85184-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85184-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="85184-124">Accept</span></span>|<span data-ttu-id="85184-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85184-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85184-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85184-126">Request body</span></span>
<span data-ttu-id="85184-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsWifiEnterpriseEAPConfiguration.</span><span class="sxs-lookup"><span data-stu-id="85184-127">In the request body, supply a JSON representation for the windowsWifiEnterpriseEAPConfiguration object.</span></span>

<span data-ttu-id="85184-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsWifiEnterpriseEAPConfiguration.</span><span class="sxs-lookup"><span data-stu-id="85184-128">The following table shows the properties that are required when you create the windowsWifiEnterpriseEAPConfiguration.</span></span>

|<span data-ttu-id="85184-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85184-129">Property</span></span>|<span data-ttu-id="85184-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="85184-130">Type</span></span>|<span data-ttu-id="85184-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="85184-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85184-132">id</span><span class="sxs-lookup"><span data-stu-id="85184-132">id</span></span>|<span data-ttu-id="85184-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85184-133">String</span></span>|<span data-ttu-id="85184-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="85184-134">Key of the entity.</span></span> <span data-ttu-id="85184-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85184-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85184-136">lastModifiedDateTime</span></span>|<span data-ttu-id="85184-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85184-137">DateTimeOffset</span></span>|<span data-ttu-id="85184-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="85184-138">DateTime the object was last modified.</span></span> <span data-ttu-id="85184-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85184-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="85184-140">roleScopeTagIds</span></span>|<span data-ttu-id="85184-141">String collection</span><span class="sxs-lookup"><span data-stu-id="85184-141">String collection</span></span>|<span data-ttu-id="85184-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="85184-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="85184-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85184-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="85184-144">supportsScopeTags</span></span>|<span data-ttu-id="85184-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="85184-145">Boolean</span></span>|<span data-ttu-id="85184-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="85184-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="85184-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="85184-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="85184-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="85184-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="85184-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85184-149">This property is read-only.</span></span> <span data-ttu-id="85184-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85184-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="85184-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="85184-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="85184-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="85184-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="85184-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="85184-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85184-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="85184-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="85184-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="85184-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="85184-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="85184-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="85184-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85184-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="85184-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="85184-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="85184-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="85184-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="85184-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="85184-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85184-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85184-163">createdDateTime</span></span>|<span data-ttu-id="85184-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85184-164">DateTimeOffset</span></span>|<span data-ttu-id="85184-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="85184-165">DateTime the object was created.</span></span> <span data-ttu-id="85184-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85184-167">description</span><span class="sxs-lookup"><span data-stu-id="85184-167">description</span></span>|<span data-ttu-id="85184-168">String</span><span class="sxs-lookup"><span data-stu-id="85184-168">String</span></span>|<span data-ttu-id="85184-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="85184-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="85184-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85184-171">displayName</span><span class="sxs-lookup"><span data-stu-id="85184-171">displayName</span></span>|<span data-ttu-id="85184-172">String</span><span class="sxs-lookup"><span data-stu-id="85184-172">String</span></span>|<span data-ttu-id="85184-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="85184-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="85184-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85184-175">versão</span><span class="sxs-lookup"><span data-stu-id="85184-175">version</span></span>|<span data-ttu-id="85184-176">Int32</span><span class="sxs-lookup"><span data-stu-id="85184-176">Int32</span></span>|<span data-ttu-id="85184-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="85184-177">Version of the device configuration.</span></span> <span data-ttu-id="85184-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85184-179">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="85184-179">preSharedKey</span></span>|<span data-ttu-id="85184-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85184-180">String</span></span>|<span data-ttu-id="85184-181">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="85184-181">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="85184-182">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-182">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="85184-183">à</span><span class="sxs-lookup"><span data-stu-id="85184-183">wifiSecurityType</span></span>|[<span data-ttu-id="85184-184">à</span><span class="sxs-lookup"><span data-stu-id="85184-184">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="85184-185">Especifique o tipo de segurança wifi.</span><span class="sxs-lookup"><span data-stu-id="85184-185">Specify the Wifi Security Type.</span></span> <span data-ttu-id="85184-186">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85184-186">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="85184-187">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="85184-187">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="85184-188">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="85184-188">meteredConnectionLimit</span></span>|[<span data-ttu-id="85184-189">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="85184-189">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="85184-190">Especifique o tipo de limite de conexão limitada para a conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="85184-190">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="85184-191">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85184-191">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="85184-192">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="85184-192">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="85184-193">SSID</span><span class="sxs-lookup"><span data-stu-id="85184-193">ssid</span></span>|<span data-ttu-id="85184-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85184-194">String</span></span>|<span data-ttu-id="85184-195">Especifique o SSID da conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="85184-195">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="85184-196">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-196">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="85184-197">NetworkName</span><span class="sxs-lookup"><span data-stu-id="85184-197">networkName</span></span>|<span data-ttu-id="85184-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85184-198">String</span></span>|<span data-ttu-id="85184-199">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="85184-199">Specify the network configuration name.</span></span> <span data-ttu-id="85184-200">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-200">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="85184-201">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="85184-201">connectAutomatically</span></span>|<span data-ttu-id="85184-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="85184-202">Boolean</span></span>|<span data-ttu-id="85184-203">Especifique se a conexão WiFi deve se conectar automaticamente quando estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="85184-203">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="85184-204">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-204">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="85184-205">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="85184-205">connectToPreferredNetwork</span></span>|<span data-ttu-id="85184-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="85184-206">Boolean</span></span>|<span data-ttu-id="85184-207">Especifique se a conexão WiFi deve se conectar a redes mais preferenciais quando já estiver conectado a ela.</span><span class="sxs-lookup"><span data-stu-id="85184-207">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="85184-208">Requer que ConnectAutomatically seja true.</span><span class="sxs-lookup"><span data-stu-id="85184-208">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="85184-209">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-209">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="85184-210">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="85184-210">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="85184-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="85184-211">Boolean</span></span>|<span data-ttu-id="85184-212">Especifique se a conexão WiFi deve se conectar automaticamente, mesmo quando o SSID não estiver transmitindo.</span><span class="sxs-lookup"><span data-stu-id="85184-212">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="85184-213">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-213">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="85184-214">proxySetting</span><span class="sxs-lookup"><span data-stu-id="85184-214">proxySetting</span></span>|[<span data-ttu-id="85184-215">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="85184-215">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="85184-216">Especifique a configuração de proxy para a configuração de Wi-Fi herdada de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85184-216">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="85184-217">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="85184-217">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="85184-218">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="85184-218">proxyManualAddress</span></span>|<span data-ttu-id="85184-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85184-219">String</span></span>|<span data-ttu-id="85184-220">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="85184-220">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="85184-221">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-221">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="85184-222">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="85184-222">proxyManualPort</span></span>|<span data-ttu-id="85184-223">Int32</span><span class="sxs-lookup"><span data-stu-id="85184-223">Int32</span></span>|<span data-ttu-id="85184-224">Especifique a porta do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="85184-224">Specify the port for the proxy server.</span></span> <span data-ttu-id="85184-225">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-225">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="85184-226">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="85184-226">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="85184-227">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85184-227">String</span></span>|<span data-ttu-id="85184-228">Especifique a URL do script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="85184-228">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="85184-229">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-229">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="85184-230">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="85184-230">forceFIPSCompliance</span></span>|<span data-ttu-id="85184-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="85184-231">Boolean</span></span>|<span data-ttu-id="85184-232">Especifique se a conformidade com FIPS deve ser forçada.</span><span class="sxs-lookup"><span data-stu-id="85184-232">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="85184-233">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85184-233">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="85184-234">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="85184-234">networkSingleSignOn</span></span>|[<span data-ttu-id="85184-235">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="85184-235">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="85184-236">Especifique o tipo de logon único na rede.</span><span class="sxs-lookup"><span data-stu-id="85184-236">Specify the network single sign on type.</span></span> <span data-ttu-id="85184-237">Os valores possíveis são: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="85184-237">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="85184-238">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="85184-238">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="85184-239">Int32</span><span class="sxs-lookup"><span data-stu-id="85184-239">Int32</span></span>|<span data-ttu-id="85184-240">Especifique o tempo limite máximo de autenticação (em segundos).</span><span class="sxs-lookup"><span data-stu-id="85184-240">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="85184-241">Intervalo válido: 1-120</span><span class="sxs-lookup"><span data-stu-id="85184-241">Valid range: 1-120</span></span>|
|<span data-ttu-id="85184-242">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="85184-242">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="85184-243">Booliano</span><span class="sxs-lookup"><span data-stu-id="85184-243">Boolean</span></span>|<span data-ttu-id="85184-244">Especifique se a conexão WiFi deve solicitar credenciais de autenticação adicionais.</span><span class="sxs-lookup"><span data-stu-id="85184-244">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="85184-245">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="85184-245">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="85184-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="85184-246">Boolean</span></span>|<span data-ttu-id="85184-247">Especifique se a conexão WiFi deve habilitar o cache da chave mestra de par.</span><span class="sxs-lookup"><span data-stu-id="85184-247">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="85184-248">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="85184-248">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="85184-249">Int32</span><span class="sxs-lookup"><span data-stu-id="85184-249">Int32</span></span>|<span data-ttu-id="85184-250">Especifique o tempo máximo de cache da chave mestra de paridade (em minutos).</span><span class="sxs-lookup"><span data-stu-id="85184-250">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="85184-251">Intervalo válido: 5-1440</span><span class="sxs-lookup"><span data-stu-id="85184-251">Valid range: 5-1440</span></span>|
|<span data-ttu-id="85184-252">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="85184-252">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="85184-253">Int32</span><span class="sxs-lookup"><span data-stu-id="85184-253">Int32</span></span>|<span data-ttu-id="85184-254">Especifique o número máximo de chaves de mestre emparelhadas no cache.</span><span class="sxs-lookup"><span data-stu-id="85184-254">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="85184-255">Intervalo válido: 1-255</span><span class="sxs-lookup"><span data-stu-id="85184-255">Valid range: 1-255</span></span>|
|<span data-ttu-id="85184-256">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="85184-256">enablePreAuthentication</span></span>|<span data-ttu-id="85184-257">Booliano</span><span class="sxs-lookup"><span data-stu-id="85184-257">Boolean</span></span>|<span data-ttu-id="85184-258">Especifique se a pré-autenticação deve ser habilitada.</span><span class="sxs-lookup"><span data-stu-id="85184-258">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="85184-259">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="85184-259">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="85184-260">Int32</span><span class="sxs-lookup"><span data-stu-id="85184-260">Int32</span></span>|<span data-ttu-id="85184-261">Especifique as tentativas máximas de pré-autenticação.</span><span class="sxs-lookup"><span data-stu-id="85184-261">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="85184-262">Intervalo válido: 1-16</span><span class="sxs-lookup"><span data-stu-id="85184-262">Valid range: 1-16</span></span>|
|<span data-ttu-id="85184-263">eapType</span><span class="sxs-lookup"><span data-stu-id="85184-263">eapType</span></span>|[<span data-ttu-id="85184-264">eapType</span><span class="sxs-lookup"><span data-stu-id="85184-264">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="85184-265">EAP (protocolo de autenticação extensível).</span><span class="sxs-lookup"><span data-stu-id="85184-265">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="85184-266">Indica o tipo de protocolo EAP definido no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="85184-266">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="85184-267">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="85184-267">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="85184-268">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="85184-268">trustedServerCertificateNames</span></span>|<span data-ttu-id="85184-269">String collection</span><span class="sxs-lookup"><span data-stu-id="85184-269">String collection</span></span>|<span data-ttu-id="85184-270">Especificar nomes de certificado de servidor confiável.</span><span class="sxs-lookup"><span data-stu-id="85184-270">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="85184-271">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="85184-271">authenticationMethod</span></span>|[<span data-ttu-id="85184-272">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="85184-272">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="85184-273">Especifique o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="85184-273">Specify the authentication method.</span></span> <span data-ttu-id="85184-274">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="85184-274">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="85184-275">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="85184-275">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="85184-276">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="85184-276">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="85184-277">Especificar o protocolo de autenticação interna para EAP TTLS.</span><span class="sxs-lookup"><span data-stu-id="85184-277">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="85184-278">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="85184-278">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="85184-279">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="85184-279">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="85184-280">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85184-280">String</span></span>|<span data-ttu-id="85184-281">Especifique a cadeia de caracteres para substituir os nomes de texto para privacidade ao usar EAP TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="85184-281">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="85184-282">Resposta</span><span class="sxs-lookup"><span data-stu-id="85184-282">Response</span></span>
<span data-ttu-id="85184-283">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85184-283">If successful, this method returns a `201 Created` response code and a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85184-284">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85184-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="85184-285">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85184-285">Request</span></span>
<span data-ttu-id="85184-286">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85184-286">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2277

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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="85184-287">Resposta</span><span class="sxs-lookup"><span data-stu-id="85184-287">Response</span></span>
<span data-ttu-id="85184-p134">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85184-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2449

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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```






