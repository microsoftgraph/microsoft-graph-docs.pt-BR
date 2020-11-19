---
title: Criar windowsWifiEnterpriseEAPConfiguration
description: Criar um novo objeto windowsWifiEnterpriseEAPConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4fa446e80725e486fd4e59737c9b7419bba06282
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49311305"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="3b478-103">Criar windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="3b478-103">Create windowsWifiEnterpriseEAPConfiguration</span></span>

<span data-ttu-id="3b478-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b478-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b478-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b478-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b478-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b478-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b478-107">Criar um novo objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3b478-107">Create a new [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b478-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b478-108">Prerequisites</span></span>
<span data-ttu-id="3b478-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b478-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b478-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b478-111">Permission type</span></span>|<span data-ttu-id="3b478-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b478-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b478-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b478-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b478-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b478-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3b478-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b478-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b478-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b478-116">Not supported.</span></span>|
|<span data-ttu-id="3b478-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b478-117">Application</span></span>|<span data-ttu-id="3b478-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b478-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b478-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b478-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3b478-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b478-120">Request headers</span></span>
|<span data-ttu-id="3b478-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b478-121">Header</span></span>|<span data-ttu-id="3b478-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3b478-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b478-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b478-123">Authorization</span></span>|<span data-ttu-id="3b478-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b478-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b478-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b478-125">Accept</span></span>|<span data-ttu-id="3b478-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b478-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b478-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b478-127">Request body</span></span>
<span data-ttu-id="3b478-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsWifiEnterpriseEAPConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3b478-128">In the request body, supply a JSON representation for the windowsWifiEnterpriseEAPConfiguration object.</span></span>

<span data-ttu-id="3b478-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsWifiEnterpriseEAPConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3b478-129">The following table shows the properties that are required when you create the windowsWifiEnterpriseEAPConfiguration.</span></span>

|<span data-ttu-id="3b478-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b478-130">Property</span></span>|<span data-ttu-id="3b478-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b478-131">Type</span></span>|<span data-ttu-id="3b478-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b478-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b478-133">id</span><span class="sxs-lookup"><span data-stu-id="3b478-133">id</span></span>|<span data-ttu-id="3b478-134">String</span><span class="sxs-lookup"><span data-stu-id="3b478-134">String</span></span>|<span data-ttu-id="3b478-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3b478-135">Key of the entity.</span></span> <span data-ttu-id="3b478-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b478-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b478-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3b478-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b478-138">DateTimeOffset</span></span>|<span data-ttu-id="3b478-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3b478-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3b478-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b478-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3b478-141">roleScopeTagIds</span></span>|<span data-ttu-id="3b478-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b478-142">String collection</span></span>|<span data-ttu-id="3b478-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3b478-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3b478-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b478-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3b478-145">supportsScopeTags</span></span>|<span data-ttu-id="3b478-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b478-146">Boolean</span></span>|<span data-ttu-id="3b478-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="3b478-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3b478-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="3b478-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3b478-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="3b478-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3b478-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3b478-150">This property is read-only.</span></span> <span data-ttu-id="3b478-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b478-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3b478-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3b478-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3b478-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3b478-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="3b478-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3b478-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b478-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3b478-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3b478-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3b478-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3b478-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="3b478-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3b478-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b478-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3b478-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3b478-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3b478-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3b478-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="3b478-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3b478-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b478-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b478-164">createdDateTime</span></span>|<span data-ttu-id="3b478-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b478-165">DateTimeOffset</span></span>|<span data-ttu-id="3b478-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3b478-166">DateTime the object was created.</span></span> <span data-ttu-id="3b478-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b478-168">description</span><span class="sxs-lookup"><span data-stu-id="3b478-168">description</span></span>|<span data-ttu-id="3b478-169">String</span><span class="sxs-lookup"><span data-stu-id="3b478-169">String</span></span>|<span data-ttu-id="3b478-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3b478-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3b478-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b478-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3b478-172">displayName</span></span>|<span data-ttu-id="3b478-173">String</span><span class="sxs-lookup"><span data-stu-id="3b478-173">String</span></span>|<span data-ttu-id="3b478-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3b478-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3b478-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b478-176">versão</span><span class="sxs-lookup"><span data-stu-id="3b478-176">version</span></span>|<span data-ttu-id="3b478-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3b478-177">Int32</span></span>|<span data-ttu-id="3b478-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3b478-178">Version of the device configuration.</span></span> <span data-ttu-id="3b478-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b478-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="3b478-180">preSharedKey</span></span>|<span data-ttu-id="3b478-181">String</span><span class="sxs-lookup"><span data-stu-id="3b478-181">String</span></span>|<span data-ttu-id="3b478-182">Esta é a chave pré-compartilhada para a rede WPA de Wi-Fi pessoal.</span><span class="sxs-lookup"><span data-stu-id="3b478-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="3b478-183">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-183">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3b478-184">à</span><span class="sxs-lookup"><span data-stu-id="3b478-184">wifiSecurityType</span></span>|[<span data-ttu-id="3b478-185">à</span><span class="sxs-lookup"><span data-stu-id="3b478-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="3b478-186">Especifique o tipo de segurança wifi.</span><span class="sxs-lookup"><span data-stu-id="3b478-186">Specify the Wifi Security Type.</span></span> <span data-ttu-id="3b478-187">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3b478-187">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="3b478-188">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="3b478-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="3b478-189">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="3b478-189">meteredConnectionLimit</span></span>|[<span data-ttu-id="3b478-190">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="3b478-190">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="3b478-191">Especifique o tipo de limite de conexão limitada para a conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="3b478-191">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="3b478-192">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3b478-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="3b478-193">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="3b478-193">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="3b478-194">SSID</span><span class="sxs-lookup"><span data-stu-id="3b478-194">ssid</span></span>|<span data-ttu-id="3b478-195">String</span><span class="sxs-lookup"><span data-stu-id="3b478-195">String</span></span>|<span data-ttu-id="3b478-196">Especifique o SSID da conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="3b478-196">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="3b478-197">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3b478-198">NetworkName</span><span class="sxs-lookup"><span data-stu-id="3b478-198">networkName</span></span>|<span data-ttu-id="3b478-199">String</span><span class="sxs-lookup"><span data-stu-id="3b478-199">String</span></span>|<span data-ttu-id="3b478-200">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="3b478-200">Specify the network configuration name.</span></span> <span data-ttu-id="3b478-201">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3b478-202">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="3b478-202">connectAutomatically</span></span>|<span data-ttu-id="3b478-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b478-203">Boolean</span></span>|<span data-ttu-id="3b478-204">Especifique se a conexão WiFi deve se conectar automaticamente quando estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="3b478-204">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="3b478-205">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-205">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3b478-206">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="3b478-206">connectToPreferredNetwork</span></span>|<span data-ttu-id="3b478-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b478-207">Boolean</span></span>|<span data-ttu-id="3b478-208">Especifique se a conexão WiFi deve se conectar a redes mais preferenciais quando já estiver conectado a ela.</span><span class="sxs-lookup"><span data-stu-id="3b478-208">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="3b478-209">Requer que ConnectAutomatically seja true.</span><span class="sxs-lookup"><span data-stu-id="3b478-209">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="3b478-210">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3b478-211">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="3b478-211">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="3b478-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b478-212">Boolean</span></span>|<span data-ttu-id="3b478-213">Especifique se a conexão WiFi deve se conectar automaticamente, mesmo quando o SSID não estiver transmitindo.</span><span class="sxs-lookup"><span data-stu-id="3b478-213">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="3b478-214">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3b478-215">proxySetting</span><span class="sxs-lookup"><span data-stu-id="3b478-215">proxySetting</span></span>|[<span data-ttu-id="3b478-216">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="3b478-216">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="3b478-217">Especifique a configuração de proxy para a configuração de Wi-Fi herdada de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3b478-217">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="3b478-218">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="3b478-218">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="3b478-219">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="3b478-219">proxyManualAddress</span></span>|<span data-ttu-id="3b478-220">String</span><span class="sxs-lookup"><span data-stu-id="3b478-220">String</span></span>|<span data-ttu-id="3b478-221">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="3b478-221">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="3b478-222">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3b478-223">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="3b478-223">proxyManualPort</span></span>|<span data-ttu-id="3b478-224">Int32</span><span class="sxs-lookup"><span data-stu-id="3b478-224">Int32</span></span>|<span data-ttu-id="3b478-225">Especifique a porta do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="3b478-225">Specify the port for the proxy server.</span></span> <span data-ttu-id="3b478-226">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-226">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3b478-227">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="3b478-227">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="3b478-228">String</span><span class="sxs-lookup"><span data-stu-id="3b478-228">String</span></span>|<span data-ttu-id="3b478-229">Especifique a URL do script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="3b478-229">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="3b478-230">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-230">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3b478-231">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="3b478-231">forceFIPSCompliance</span></span>|<span data-ttu-id="3b478-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b478-232">Boolean</span></span>|<span data-ttu-id="3b478-233">Especifique se a conformidade com FIPS deve ser forçada.</span><span class="sxs-lookup"><span data-stu-id="3b478-233">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="3b478-234">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b478-234">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3b478-235">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="3b478-235">networkSingleSignOn</span></span>|[<span data-ttu-id="3b478-236">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="3b478-236">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="3b478-237">Especifique o tipo de logon único na rede.</span><span class="sxs-lookup"><span data-stu-id="3b478-237">Specify the network single sign on type.</span></span> <span data-ttu-id="3b478-238">Os valores possíveis são: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="3b478-238">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="3b478-239">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="3b478-239">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="3b478-240">Int32</span><span class="sxs-lookup"><span data-stu-id="3b478-240">Int32</span></span>|<span data-ttu-id="3b478-241">Especifique o tempo limite máximo de autenticação (em segundos).</span><span class="sxs-lookup"><span data-stu-id="3b478-241">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="3b478-242">Intervalo válido: 1-120</span><span class="sxs-lookup"><span data-stu-id="3b478-242">Valid range: 1-120</span></span>|
|<span data-ttu-id="3b478-243">userBasedVirtualLan</span><span class="sxs-lookup"><span data-stu-id="3b478-243">userBasedVirtualLan</span></span>|<span data-ttu-id="3b478-244">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b478-244">Boolean</span></span>|<span data-ttu-id="3b478-245">Especifique se deseja alterar a LAN virtual usada pelo dispositivo com base nas credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="3b478-245">Specifiy whether to change the virtual LAN used by the device based on the user’s credentials.</span></span> <span data-ttu-id="3b478-246">Não pode ser usado quando NetworkSingleSignOnType está definido como desabilitado.</span><span class="sxs-lookup"><span data-stu-id="3b478-246">Cannot be used when NetworkSingleSignOnType is set to Disabled.</span></span>|
|<span data-ttu-id="3b478-247">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="3b478-247">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="3b478-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b478-248">Boolean</span></span>|<span data-ttu-id="3b478-249">Especifique se a conexão WiFi deve solicitar credenciais de autenticação adicionais.</span><span class="sxs-lookup"><span data-stu-id="3b478-249">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="3b478-250">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="3b478-250">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="3b478-251">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b478-251">Boolean</span></span>|<span data-ttu-id="3b478-252">Especifique se a conexão WiFi deve habilitar o cache da chave mestra de par.</span><span class="sxs-lookup"><span data-stu-id="3b478-252">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="3b478-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="3b478-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="3b478-254">Int32</span><span class="sxs-lookup"><span data-stu-id="3b478-254">Int32</span></span>|<span data-ttu-id="3b478-255">Especifique o tempo máximo de cache da chave mestra de paridade (em minutos).</span><span class="sxs-lookup"><span data-stu-id="3b478-255">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="3b478-256">Intervalo válido: 5-1440</span><span class="sxs-lookup"><span data-stu-id="3b478-256">Valid range: 5-1440</span></span>|
|<span data-ttu-id="3b478-257">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="3b478-257">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="3b478-258">Int32</span><span class="sxs-lookup"><span data-stu-id="3b478-258">Int32</span></span>|<span data-ttu-id="3b478-259">Especifique o número máximo de chaves de mestre emparelhadas no cache.</span><span class="sxs-lookup"><span data-stu-id="3b478-259">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="3b478-260">Intervalo válido: 1-255</span><span class="sxs-lookup"><span data-stu-id="3b478-260">Valid range: 1-255</span></span>|
|<span data-ttu-id="3b478-261">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="3b478-261">enablePreAuthentication</span></span>|<span data-ttu-id="3b478-262">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b478-262">Boolean</span></span>|<span data-ttu-id="3b478-263">Especifique se a pré-autenticação deve ser habilitada.</span><span class="sxs-lookup"><span data-stu-id="3b478-263">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="3b478-264">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="3b478-264">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="3b478-265">Int32</span><span class="sxs-lookup"><span data-stu-id="3b478-265">Int32</span></span>|<span data-ttu-id="3b478-266">Especifique as tentativas máximas de pré-autenticação.</span><span class="sxs-lookup"><span data-stu-id="3b478-266">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="3b478-267">Intervalo válido: 1-16</span><span class="sxs-lookup"><span data-stu-id="3b478-267">Valid range: 1-16</span></span>|
|<span data-ttu-id="3b478-268">eapType</span><span class="sxs-lookup"><span data-stu-id="3b478-268">eapType</span></span>|[<span data-ttu-id="3b478-269">eapType</span><span class="sxs-lookup"><span data-stu-id="3b478-269">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="3b478-270">EAP (protocolo de autenticação extensível).</span><span class="sxs-lookup"><span data-stu-id="3b478-270">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="3b478-271">Indica o tipo de protocolo EAP definido no ponto de extremidade de Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="3b478-271">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="3b478-272">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="3b478-272">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="3b478-273">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="3b478-273">trustedServerCertificateNames</span></span>|<span data-ttu-id="3b478-274">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b478-274">String collection</span></span>|<span data-ttu-id="3b478-275">Especificar nomes de certificado de servidor confiável.</span><span class="sxs-lookup"><span data-stu-id="3b478-275">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="3b478-276">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3b478-276">authenticationMethod</span></span>|[<span data-ttu-id="3b478-277">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3b478-277">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="3b478-278">Especifique o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3b478-278">Specify the authentication method.</span></span> <span data-ttu-id="3b478-279">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="3b478-279">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="3b478-280">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="3b478-280">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="3b478-281">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="3b478-281">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="3b478-282">Especificar o protocolo de autenticação interna para EAP TTLS.</span><span class="sxs-lookup"><span data-stu-id="3b478-282">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="3b478-283">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="3b478-283">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="3b478-284">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="3b478-284">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="3b478-285">String</span><span class="sxs-lookup"><span data-stu-id="3b478-285">String</span></span>|<span data-ttu-id="3b478-286">Especifique a cadeia de caracteres para substituir os nomes de texto para privacidade ao usar EAP TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="3b478-286">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|
|<span data-ttu-id="3b478-287">requireCryptographicBinding</span><span class="sxs-lookup"><span data-stu-id="3b478-287">requireCryptographicBinding</span></span>|<span data-ttu-id="3b478-288">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b478-288">Boolean</span></span>|<span data-ttu-id="3b478-289">Especifique se deseja habilitar a associação criptográfica quando o tipo EAP for selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="3b478-289">Specify whether to enable cryptographic binding when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="3b478-290">performServerValidation</span><span class="sxs-lookup"><span data-stu-id="3b478-290">performServerValidation</span></span>|<span data-ttu-id="3b478-291">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b478-291">Boolean</span></span>|<span data-ttu-id="3b478-292">Especifique se deseja habilitar a verificação da identidade do servidor, validando o certificado quando o tipo EAP estiver selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="3b478-292">Specify whether to enable verification of server's identity by validating the certificate when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="3b478-293">disableUserPromptForServerValidation</span><span class="sxs-lookup"><span data-stu-id="3b478-293">disableUserPromptForServerValidation</span></span>|<span data-ttu-id="3b478-294">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b478-294">Boolean</span></span>|<span data-ttu-id="3b478-295">Especifique se deseja impedir que o usuário seja solicitado a autorizar novos servidores para autoridades de certificação confiáveis quando o tipo EAP for selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="3b478-295">Specify whether to prevent the user from being prompted to authorize new servers for trusted certification authorities when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="3b478-296">authenticationPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="3b478-296">authenticationPeriodInSeconds</span></span>|<span data-ttu-id="3b478-297">Int32</span><span class="sxs-lookup"><span data-stu-id="3b478-297">Int32</span></span>|<span data-ttu-id="3b478-298">Especifique o número de segundos que o cliente deve aguardar após uma tentativa de autenticação antes de falhar.</span><span class="sxs-lookup"><span data-stu-id="3b478-298">Specify the number of seconds for the client to wait after an authentication attempt before failing.</span></span> <span data-ttu-id="3b478-299">Intervalo válido de 1-3600.</span><span class="sxs-lookup"><span data-stu-id="3b478-299">Valid range 1-3600.</span></span>|
|<span data-ttu-id="3b478-300">authenticationRetryDelayPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="3b478-300">authenticationRetryDelayPeriodInSeconds</span></span>|<span data-ttu-id="3b478-301">Int32</span><span class="sxs-lookup"><span data-stu-id="3b478-301">Int32</span></span>|<span data-ttu-id="3b478-302">Especifique o número de segundos entre uma falha de autenticação e a próxima tentativa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3b478-302">Specify the number of seconds between a failed authentication and the next authentication attempt.</span></span> <span data-ttu-id="3b478-303">Intervalo válido de 1-3600.</span><span class="sxs-lookup"><span data-stu-id="3b478-303">Valid range 1-3600.</span></span>|
|<span data-ttu-id="3b478-304">eapolStartPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="3b478-304">eapolStartPeriodInSeconds</span></span>|<span data-ttu-id="3b478-305">Int32</span><span class="sxs-lookup"><span data-stu-id="3b478-305">Int32</span></span>|<span data-ttu-id="3b478-306">Especifique o número de segundos de espera antes de enviar uma mensagem de início de EAPOL (protocolo de autenticação extensível via LAN).</span><span class="sxs-lookup"><span data-stu-id="3b478-306">Specify the number of seconds to wait before sending an EAPOL (Extensible Authentication Protocol over LAN) Start message.</span></span> <span data-ttu-id="3b478-307">Intervalo válido de 1-3600.</span><span class="sxs-lookup"><span data-stu-id="3b478-307">Valid range 1-3600.</span></span>|
|<span data-ttu-id="3b478-308">maximumEAPOLStartMessages</span><span class="sxs-lookup"><span data-stu-id="3b478-308">maximumEAPOLStartMessages</span></span>|<span data-ttu-id="3b478-309">Int32</span><span class="sxs-lookup"><span data-stu-id="3b478-309">Int32</span></span>|<span data-ttu-id="3b478-310">Especifique o número máximo de mensagens de início de EAPOL (Extensible Authentication Protocol over LAN) para serem enviadas antes de retornar uma falha.</span><span class="sxs-lookup"><span data-stu-id="3b478-310">Specifiy the maximum number of EAPOL (Extensible Authentication Protocol over LAN) Start messages to be sent before returning failure.</span></span> <span data-ttu-id="3b478-311">Intervalo válido de 1-100.</span><span class="sxs-lookup"><span data-stu-id="3b478-311">Valid range 1-100.</span></span>|
|<span data-ttu-id="3b478-312">maximumAuthenticationFailures</span><span class="sxs-lookup"><span data-stu-id="3b478-312">maximumAuthenticationFailures</span></span>|<span data-ttu-id="3b478-313">Int32</span><span class="sxs-lookup"><span data-stu-id="3b478-313">Int32</span></span>|<span data-ttu-id="3b478-314">Especifique as falhas máximas de autenticação permitidas para um conjunto de credenciais.</span><span class="sxs-lookup"><span data-stu-id="3b478-314">Specify the maximum authentication failures allowed for a set of credentials.</span></span> <span data-ttu-id="3b478-315">Intervalo válido de 1-100.</span><span class="sxs-lookup"><span data-stu-id="3b478-315">Valid range 1-100.</span></span>|
|<span data-ttu-id="3b478-316">cacheCredentials</span><span class="sxs-lookup"><span data-stu-id="3b478-316">cacheCredentials</span></span>|<span data-ttu-id="3b478-317">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b478-317">Boolean</span></span>|<span data-ttu-id="3b478-318">Especifique se deseja armazenar em cache credenciais de usuário no dispositivo para que os usuários não precisem inseri-las sempre que se conectarem.</span><span class="sxs-lookup"><span data-stu-id="3b478-318">Specify whether to cache user credentials on the device so that users don’t need to keep entering them each time they connect.</span></span>|
|<span data-ttu-id="3b478-319">authenticationType</span><span class="sxs-lookup"><span data-stu-id="3b478-319">authenticationType</span></span>|[<span data-ttu-id="3b478-320">wifiAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="3b478-320">wifiAuthenticationType</span></span>](../resources/intune-deviceconfig-wifiauthenticationtype.md)|<span data-ttu-id="3b478-321">Especifique se deseja autenticar o usuário, o dispositivo, ou para usar a autenticação de convidado (nenhuma).</span><span class="sxs-lookup"><span data-stu-id="3b478-321">Specify whether to authenticate the user, the device, either, or to use guest authentication (none).</span></span> <span data-ttu-id="3b478-322">Se você estiver usando a autenticação de certificado, certifique-se de que o tipo de certificado corresponde ao tipo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3b478-322">If you’re using certificate authentication, make sure the certificate type matches the authentication type.</span></span> <span data-ttu-id="3b478-323">Os valores possíveis são: `none`, `user`, `machine`, `machineOrUser`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="3b478-323">Possible values are: `none`, `user`, `machine`, `machineOrUser`, `guest`.</span></span>|



## <a name="response"></a><span data-ttu-id="3b478-324">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b478-324">Response</span></span>
<span data-ttu-id="3b478-325">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b478-325">If successful, this method returns a `201 Created` response code and a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b478-326">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b478-326">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b478-327">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b478-327">Request</span></span>
<span data-ttu-id="3b478-328">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b478-328">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="3b478-329">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b478-329">Response</span></span>
<span data-ttu-id="3b478-p141">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b478-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




