---
title: Criar windowsWifiEnterpriseEAPConfiguration
description: Criar um novo objeto windowsWifiEnterpriseEAPConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 64b79f93cfd9cd23617c99529331c6063efe6716
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32510819"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="3eb58-103">Criar windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="3eb58-103">Create windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="3eb58-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3eb58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3eb58-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3eb58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3eb58-106">Criar um novo objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3eb58-106">Create a new [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3eb58-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3eb58-107">Prerequisites</span></span>
<span data-ttu-id="3eb58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eb58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eb58-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3eb58-110">Permission type</span></span>|<span data-ttu-id="3eb58-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3eb58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3eb58-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3eb58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3eb58-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb58-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3eb58-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3eb58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3eb58-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3eb58-115">Not supported.</span></span>|
|<span data-ttu-id="3eb58-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3eb58-116">Application</span></span>|<span data-ttu-id="3eb58-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3eb58-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3eb58-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3eb58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3eb58-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3eb58-119">Request headers</span></span>
|<span data-ttu-id="3eb58-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3eb58-120">Header</span></span>|<span data-ttu-id="3eb58-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3eb58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3eb58-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3eb58-122">Authorization</span></span>|<span data-ttu-id="3eb58-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3eb58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3eb58-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3eb58-124">Accept</span></span>|<span data-ttu-id="3eb58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3eb58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eb58-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3eb58-126">Request body</span></span>
<span data-ttu-id="3eb58-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsWifiEnterpriseEAPConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3eb58-127">In the request body, supply a JSON representation for the windowsWifiEnterpriseEAPConfiguration object.</span></span>

<span data-ttu-id="3eb58-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsWifiEnterpriseEAPConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3eb58-128">The following table shows the properties that are required when you create the windowsWifiEnterpriseEAPConfiguration.</span></span>

|<span data-ttu-id="3eb58-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3eb58-129">Property</span></span>|<span data-ttu-id="3eb58-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3eb58-130">Type</span></span>|<span data-ttu-id="3eb58-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3eb58-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3eb58-132">id</span><span class="sxs-lookup"><span data-stu-id="3eb58-132">id</span></span>|<span data-ttu-id="3eb58-133">String</span><span class="sxs-lookup"><span data-stu-id="3eb58-133">String</span></span>|<span data-ttu-id="3eb58-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3eb58-134">Key of the entity.</span></span> <span data-ttu-id="3eb58-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3eb58-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3eb58-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3eb58-137">DateTimeOffset</span></span>|<span data-ttu-id="3eb58-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3eb58-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3eb58-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3eb58-140">roleScopeTagIds</span></span>|<span data-ttu-id="3eb58-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3eb58-141">String collection</span></span>|<span data-ttu-id="3eb58-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3eb58-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3eb58-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3eb58-144">supportsScopeTags</span></span>|<span data-ttu-id="3eb58-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="3eb58-145">Boolean</span></span>|<span data-ttu-id="3eb58-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="3eb58-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3eb58-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="3eb58-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3eb58-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="3eb58-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3eb58-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3eb58-149">This property is read-only.</span></span> <span data-ttu-id="3eb58-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3eb58-151">createdDateTime</span></span>|<span data-ttu-id="3eb58-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3eb58-152">DateTimeOffset</span></span>|<span data-ttu-id="3eb58-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3eb58-153">DateTime the object was created.</span></span> <span data-ttu-id="3eb58-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-155">description</span><span class="sxs-lookup"><span data-stu-id="3eb58-155">description</span></span>|<span data-ttu-id="3eb58-156">String</span><span class="sxs-lookup"><span data-stu-id="3eb58-156">String</span></span>|<span data-ttu-id="3eb58-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3eb58-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3eb58-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3eb58-159">displayName</span></span>|<span data-ttu-id="3eb58-160">String</span><span class="sxs-lookup"><span data-stu-id="3eb58-160">String</span></span>|<span data-ttu-id="3eb58-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3eb58-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3eb58-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-163">versão</span><span class="sxs-lookup"><span data-stu-id="3eb58-163">version</span></span>|<span data-ttu-id="3eb58-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3eb58-164">Int32</span></span>|<span data-ttu-id="3eb58-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3eb58-165">Version of the device configuration.</span></span> <span data-ttu-id="3eb58-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-167">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="3eb58-167">preSharedKey</span></span>|<span data-ttu-id="3eb58-168">String</span><span class="sxs-lookup"><span data-stu-id="3eb58-168">String</span></span>|<span data-ttu-id="3eb58-169">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="3eb58-169">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="3eb58-170">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-170">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-171">à</span><span class="sxs-lookup"><span data-stu-id="3eb58-171">wifiSecurityType</span></span>|[<span data-ttu-id="3eb58-172">à</span><span class="sxs-lookup"><span data-stu-id="3eb58-172">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="3eb58-173">Especifique o tipo de segurança wifi.</span><span class="sxs-lookup"><span data-stu-id="3eb58-173">Specify the Wifi Security Type.</span></span> <span data-ttu-id="3eb58-174">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3eb58-174">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="3eb58-175">Os valores possíveis são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="3eb58-175">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="3eb58-176">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="3eb58-176">meteredConnectionLimit</span></span>|[<span data-ttu-id="3eb58-177">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="3eb58-177">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="3eb58-178">Especifique o tipo de limite de conexão limitada para a conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="3eb58-178">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="3eb58-179">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3eb58-179">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="3eb58-180">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="3eb58-180">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="3eb58-181">SSID</span><span class="sxs-lookup"><span data-stu-id="3eb58-181">ssid</span></span>|<span data-ttu-id="3eb58-182">String</span><span class="sxs-lookup"><span data-stu-id="3eb58-182">String</span></span>|<span data-ttu-id="3eb58-183">Especifique o SSID da conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="3eb58-183">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="3eb58-184">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-184">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-185">NetworkName</span><span class="sxs-lookup"><span data-stu-id="3eb58-185">networkName</span></span>|<span data-ttu-id="3eb58-186">String</span><span class="sxs-lookup"><span data-stu-id="3eb58-186">String</span></span>|<span data-ttu-id="3eb58-187">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="3eb58-187">Specify the network configuration name.</span></span> <span data-ttu-id="3eb58-188">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-188">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-189">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="3eb58-189">connectAutomatically</span></span>|<span data-ttu-id="3eb58-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="3eb58-190">Boolean</span></span>|<span data-ttu-id="3eb58-191">Especifique se a conexão WiFi deve se conectar automaticamente quando estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="3eb58-191">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="3eb58-192">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-193">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="3eb58-193">connectToPreferredNetwork</span></span>|<span data-ttu-id="3eb58-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="3eb58-194">Boolean</span></span>|<span data-ttu-id="3eb58-195">Especifique se a conexão WiFi deve se conectar a redes mais preferenciais quando já estiver conectado a ela.</span><span class="sxs-lookup"><span data-stu-id="3eb58-195">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="3eb58-196">Requer que ConnectAutomatically seja true.</span><span class="sxs-lookup"><span data-stu-id="3eb58-196">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="3eb58-197">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-198">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="3eb58-198">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="3eb58-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="3eb58-199">Boolean</span></span>|<span data-ttu-id="3eb58-200">Especifique se a conexão WiFi deve se conectar automaticamente, mesmo quando o SSID não estiver transmitindo.</span><span class="sxs-lookup"><span data-stu-id="3eb58-200">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="3eb58-201">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-202">proxySetting</span><span class="sxs-lookup"><span data-stu-id="3eb58-202">proxySetting</span></span>|[<span data-ttu-id="3eb58-203">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="3eb58-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="3eb58-204">Especifique a configuração de proxy para a configuração de Wi-Fi herdada de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3eb58-204">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="3eb58-205">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="3eb58-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="3eb58-206">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="3eb58-206">proxyManualAddress</span></span>|<span data-ttu-id="3eb58-207">String</span><span class="sxs-lookup"><span data-stu-id="3eb58-207">String</span></span>|<span data-ttu-id="3eb58-208">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="3eb58-208">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="3eb58-209">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-209">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-210">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="3eb58-210">proxyManualPort</span></span>|<span data-ttu-id="3eb58-211">Int32</span><span class="sxs-lookup"><span data-stu-id="3eb58-211">Int32</span></span>|<span data-ttu-id="3eb58-212">Especifique a porta do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="3eb58-212">Specify the port for the proxy server.</span></span> <span data-ttu-id="3eb58-213">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-213">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-214">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="3eb58-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="3eb58-215">String</span><span class="sxs-lookup"><span data-stu-id="3eb58-215">String</span></span>|<span data-ttu-id="3eb58-216">Especifique a URL do script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="3eb58-216">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="3eb58-217">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-217">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-218">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="3eb58-218">forceFIPSCompliance</span></span>|<span data-ttu-id="3eb58-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="3eb58-219">Boolean</span></span>|<span data-ttu-id="3eb58-220">Especifique se a conformidade com FIPS deve ser forçada.</span><span class="sxs-lookup"><span data-stu-id="3eb58-220">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="3eb58-221">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3eb58-221">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="3eb58-222">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="3eb58-222">networkSingleSignOn</span></span>|[<span data-ttu-id="3eb58-223">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="3eb58-223">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="3eb58-224">Especifique o tipo de logon único na rede.</span><span class="sxs-lookup"><span data-stu-id="3eb58-224">Specify the network single sign on type.</span></span> <span data-ttu-id="3eb58-225">Os valores possíveis são: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="3eb58-225">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="3eb58-226">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="3eb58-226">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="3eb58-227">Int32</span><span class="sxs-lookup"><span data-stu-id="3eb58-227">Int32</span></span>|<span data-ttu-id="3eb58-228">Especifique o tempo limite máximo de autenticação (em segundos).</span><span class="sxs-lookup"><span data-stu-id="3eb58-228">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="3eb58-229">Intervalo válido: 1-120</span><span class="sxs-lookup"><span data-stu-id="3eb58-229">Valid range: 1-120</span></span>|
|<span data-ttu-id="3eb58-230">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="3eb58-230">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="3eb58-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="3eb58-231">Boolean</span></span>|<span data-ttu-id="3eb58-232">Especifique se a conexão WiFi deve solicitar credenciais de autenticação adicionais.</span><span class="sxs-lookup"><span data-stu-id="3eb58-232">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="3eb58-233">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="3eb58-233">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="3eb58-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="3eb58-234">Boolean</span></span>|<span data-ttu-id="3eb58-235">Especifique se a conexão WiFi deve habilitar o cache da chave mestra de par.</span><span class="sxs-lookup"><span data-stu-id="3eb58-235">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="3eb58-236">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="3eb58-236">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="3eb58-237">Int32</span><span class="sxs-lookup"><span data-stu-id="3eb58-237">Int32</span></span>|<span data-ttu-id="3eb58-238">Especifique o tempo máximo de cache da chave mestra de paridade (em minutos).</span><span class="sxs-lookup"><span data-stu-id="3eb58-238">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="3eb58-239">Intervalo válido: 5-1440</span><span class="sxs-lookup"><span data-stu-id="3eb58-239">Valid range: 5-1440</span></span>|
|<span data-ttu-id="3eb58-240">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="3eb58-240">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="3eb58-241">Int32</span><span class="sxs-lookup"><span data-stu-id="3eb58-241">Int32</span></span>|<span data-ttu-id="3eb58-242">Especifique o número máximo de chaves de mestre emparelhadas no cache.</span><span class="sxs-lookup"><span data-stu-id="3eb58-242">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="3eb58-243">Intervalo válido: 1-255</span><span class="sxs-lookup"><span data-stu-id="3eb58-243">Valid range: 1-255</span></span>|
|<span data-ttu-id="3eb58-244">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="3eb58-244">enablePreAuthentication</span></span>|<span data-ttu-id="3eb58-245">Booliano</span><span class="sxs-lookup"><span data-stu-id="3eb58-245">Boolean</span></span>|<span data-ttu-id="3eb58-246">Especifique se a pré-autenticação deve ser habilitada.</span><span class="sxs-lookup"><span data-stu-id="3eb58-246">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="3eb58-247">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="3eb58-247">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="3eb58-248">Int32</span><span class="sxs-lookup"><span data-stu-id="3eb58-248">Int32</span></span>|<span data-ttu-id="3eb58-249">Especifique as tentativas máximas de pré-autenticação.</span><span class="sxs-lookup"><span data-stu-id="3eb58-249">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="3eb58-250">Intervalo válido: 1-16</span><span class="sxs-lookup"><span data-stu-id="3eb58-250">Valid range: 1-16</span></span>|
|<span data-ttu-id="3eb58-251">eapType</span><span class="sxs-lookup"><span data-stu-id="3eb58-251">eapType</span></span>|[<span data-ttu-id="3eb58-252">eapType</span><span class="sxs-lookup"><span data-stu-id="3eb58-252">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="3eb58-253">EAP (protocolo de autenticação exTensível).</span><span class="sxs-lookup"><span data-stu-id="3eb58-253">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="3eb58-254">Indica o tipo de protocolo EAP definido no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="3eb58-254">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="3eb58-255">Os valores possíveis são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="3eb58-255">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="3eb58-256">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="3eb58-256">trustedServerCertificateNames</span></span>|<span data-ttu-id="3eb58-257">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3eb58-257">String collection</span></span>|<span data-ttu-id="3eb58-258">Especificar nomes de certificado de servidor confiável.</span><span class="sxs-lookup"><span data-stu-id="3eb58-258">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="3eb58-259">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3eb58-259">authenticationMethod</span></span>|[<span data-ttu-id="3eb58-260">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3eb58-260">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="3eb58-261">Especifique o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3eb58-261">Specify the authentication method.</span></span> <span data-ttu-id="3eb58-262">Os valores possíveis são: `certificate` e `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="3eb58-262">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="3eb58-263">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="3eb58-263">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="3eb58-264">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="3eb58-264">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="3eb58-265">Especificar o protocolo de autenticação interna para EAP TTLS.</span><span class="sxs-lookup"><span data-stu-id="3eb58-265">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="3eb58-266">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="3eb58-266">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="3eb58-267">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="3eb58-267">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="3eb58-268">String</span><span class="sxs-lookup"><span data-stu-id="3eb58-268">String</span></span>|<span data-ttu-id="3eb58-269">Especifique a cadeia de caracteres para substituir os nomes de texto para privacidade ao usar EAP TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="3eb58-269">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="3eb58-270">Resposta</span><span class="sxs-lookup"><span data-stu-id="3eb58-270">Response</span></span>
<span data-ttu-id="3eb58-271">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3eb58-271">If successful, this method returns a `201 Created` response code and a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eb58-272">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3eb58-272">Example</span></span>

### <a name="request"></a><span data-ttu-id="3eb58-273">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3eb58-273">Request</span></span>
<span data-ttu-id="3eb58-274">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3eb58-274">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1504

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="3eb58-275">Resposta</span><span class="sxs-lookup"><span data-stu-id="3eb58-275">Response</span></span>
<span data-ttu-id="3eb58-p131">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3eb58-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1676

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





