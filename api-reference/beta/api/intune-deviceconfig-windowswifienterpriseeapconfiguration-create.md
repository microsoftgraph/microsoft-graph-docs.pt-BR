---
title: Criar windowsWifiEnterpriseEAPConfiguration
description: Criar um novo objeto windowsWifiEnterpriseEAPConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 89f3a2ca38fc9b5082f73d8508271f1ff182183b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42731723"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="e18c6-103">Criar windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="e18c6-103">Create windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="e18c6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e18c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e18c6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e18c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e18c6-106">Criar um novo objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e18c6-106">Create a new [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e18c6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e18c6-107">Prerequisites</span></span>
<span data-ttu-id="e18c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e18c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e18c6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e18c6-110">Permission type</span></span>|<span data-ttu-id="e18c6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e18c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e18c6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e18c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e18c6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e18c6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e18c6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e18c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e18c6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e18c6-115">Not supported.</span></span>|
|<span data-ttu-id="e18c6-116">Application</span><span class="sxs-lookup"><span data-stu-id="e18c6-116">Application</span></span>|<span data-ttu-id="e18c6-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e18c6-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e18c6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e18c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e18c6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e18c6-119">Request headers</span></span>
|<span data-ttu-id="e18c6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e18c6-120">Header</span></span>|<span data-ttu-id="e18c6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e18c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e18c6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e18c6-122">Authorization</span></span>|<span data-ttu-id="e18c6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e18c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e18c6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e18c6-124">Accept</span></span>|<span data-ttu-id="e18c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e18c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e18c6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e18c6-126">Request body</span></span>
<span data-ttu-id="e18c6-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsWifiEnterpriseEAPConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e18c6-127">In the request body, supply a JSON representation for the windowsWifiEnterpriseEAPConfiguration object.</span></span>

<span data-ttu-id="e18c6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsWifiEnterpriseEAPConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e18c6-128">The following table shows the properties that are required when you create the windowsWifiEnterpriseEAPConfiguration.</span></span>

|<span data-ttu-id="e18c6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e18c6-129">Property</span></span>|<span data-ttu-id="e18c6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e18c6-130">Type</span></span>|<span data-ttu-id="e18c6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e18c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e18c6-132">id</span><span class="sxs-lookup"><span data-stu-id="e18c6-132">id</span></span>|<span data-ttu-id="e18c6-133">String</span><span class="sxs-lookup"><span data-stu-id="e18c6-133">String</span></span>|<span data-ttu-id="e18c6-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e18c6-134">Key of the entity.</span></span> <span data-ttu-id="e18c6-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e18c6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e18c6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e18c6-137">DateTimeOffset</span></span>|<span data-ttu-id="e18c6-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e18c6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e18c6-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e18c6-140">roleScopeTagIds</span></span>|<span data-ttu-id="e18c6-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e18c6-141">String collection</span></span>|<span data-ttu-id="e18c6-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="e18c6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e18c6-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e18c6-144">supportsScopeTags</span></span>|<span data-ttu-id="e18c6-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e18c6-145">Boolean</span></span>|<span data-ttu-id="e18c6-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="e18c6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e18c6-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="e18c6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e18c6-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="e18c6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e18c6-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e18c6-149">This property is read-only.</span></span> <span data-ttu-id="e18c6-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e18c6-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e18c6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e18c6-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e18c6-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="e18c6-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e18c6-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e18c6-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e18c6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e18c6-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e18c6-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="e18c6-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e18c6-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e18c6-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e18c6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e18c6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e18c6-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="e18c6-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e18c6-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e18c6-163">createdDateTime</span></span>|<span data-ttu-id="e18c6-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e18c6-164">DateTimeOffset</span></span>|<span data-ttu-id="e18c6-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e18c6-165">DateTime the object was created.</span></span> <span data-ttu-id="e18c6-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-167">description</span><span class="sxs-lookup"><span data-stu-id="e18c6-167">description</span></span>|<span data-ttu-id="e18c6-168">String</span><span class="sxs-lookup"><span data-stu-id="e18c6-168">String</span></span>|<span data-ttu-id="e18c6-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e18c6-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e18c6-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-171">displayName</span><span class="sxs-lookup"><span data-stu-id="e18c6-171">displayName</span></span>|<span data-ttu-id="e18c6-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e18c6-172">String</span></span>|<span data-ttu-id="e18c6-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e18c6-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e18c6-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-175">versão</span><span class="sxs-lookup"><span data-stu-id="e18c6-175">version</span></span>|<span data-ttu-id="e18c6-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e18c6-176">Int32</span></span>|<span data-ttu-id="e18c6-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e18c6-177">Version of the device configuration.</span></span> <span data-ttu-id="e18c6-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-179">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="e18c6-179">preSharedKey</span></span>|<span data-ttu-id="e18c6-180">String</span><span class="sxs-lookup"><span data-stu-id="e18c6-180">String</span></span>|<span data-ttu-id="e18c6-181">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="e18c6-181">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="e18c6-182">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-182">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-183">à</span><span class="sxs-lookup"><span data-stu-id="e18c6-183">wifiSecurityType</span></span>|[<span data-ttu-id="e18c6-184">à</span><span class="sxs-lookup"><span data-stu-id="e18c6-184">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="e18c6-185">Especifique o tipo de segurança wifi.</span><span class="sxs-lookup"><span data-stu-id="e18c6-185">Specify the Wifi Security Type.</span></span> <span data-ttu-id="e18c6-186">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e18c6-186">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="e18c6-187">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="e18c6-187">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="e18c6-188">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="e18c6-188">meteredConnectionLimit</span></span>|[<span data-ttu-id="e18c6-189">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="e18c6-189">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="e18c6-190">Especifique o tipo de limite de conexão limitada para a conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="e18c6-190">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="e18c6-191">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e18c6-191">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="e18c6-192">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="e18c6-192">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="e18c6-193">SSID</span><span class="sxs-lookup"><span data-stu-id="e18c6-193">ssid</span></span>|<span data-ttu-id="e18c6-194">String</span><span class="sxs-lookup"><span data-stu-id="e18c6-194">String</span></span>|<span data-ttu-id="e18c6-195">Especifique o SSID da conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="e18c6-195">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="e18c6-196">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-196">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-197">NetworkName</span><span class="sxs-lookup"><span data-stu-id="e18c6-197">networkName</span></span>|<span data-ttu-id="e18c6-198">String</span><span class="sxs-lookup"><span data-stu-id="e18c6-198">String</span></span>|<span data-ttu-id="e18c6-199">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="e18c6-199">Specify the network configuration name.</span></span> <span data-ttu-id="e18c6-200">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-200">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-201">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="e18c6-201">connectAutomatically</span></span>|<span data-ttu-id="e18c6-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="e18c6-202">Boolean</span></span>|<span data-ttu-id="e18c6-203">Especifique se a conexão WiFi deve se conectar automaticamente quando estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="e18c6-203">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="e18c6-204">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-204">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-205">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="e18c6-205">connectToPreferredNetwork</span></span>|<span data-ttu-id="e18c6-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="e18c6-206">Boolean</span></span>|<span data-ttu-id="e18c6-207">Especifique se a conexão WiFi deve se conectar a redes mais preferenciais quando já estiver conectado a ela.</span><span class="sxs-lookup"><span data-stu-id="e18c6-207">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="e18c6-208">Requer que ConnectAutomatically seja true.</span><span class="sxs-lookup"><span data-stu-id="e18c6-208">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="e18c6-209">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-209">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-210">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="e18c6-210">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="e18c6-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="e18c6-211">Boolean</span></span>|<span data-ttu-id="e18c6-212">Especifique se a conexão WiFi deve se conectar automaticamente, mesmo quando o SSID não estiver transmitindo.</span><span class="sxs-lookup"><span data-stu-id="e18c6-212">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="e18c6-213">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-213">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-214">proxySetting</span><span class="sxs-lookup"><span data-stu-id="e18c6-214">proxySetting</span></span>|[<span data-ttu-id="e18c6-215">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="e18c6-215">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="e18c6-216">Especifique a configuração de proxy para a configuração de Wi-Fi herdada de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e18c6-216">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="e18c6-217">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="e18c6-217">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="e18c6-218">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="e18c6-218">proxyManualAddress</span></span>|<span data-ttu-id="e18c6-219">String</span><span class="sxs-lookup"><span data-stu-id="e18c6-219">String</span></span>|<span data-ttu-id="e18c6-220">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="e18c6-220">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="e18c6-221">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-221">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-222">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="e18c6-222">proxyManualPort</span></span>|<span data-ttu-id="e18c6-223">Int32</span><span class="sxs-lookup"><span data-stu-id="e18c6-223">Int32</span></span>|<span data-ttu-id="e18c6-224">Especifique a porta do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="e18c6-224">Specify the port for the proxy server.</span></span> <span data-ttu-id="e18c6-225">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-225">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-226">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="e18c6-226">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="e18c6-227">String</span><span class="sxs-lookup"><span data-stu-id="e18c6-227">String</span></span>|<span data-ttu-id="e18c6-228">Especifique a URL do script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="e18c6-228">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="e18c6-229">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-229">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-230">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="e18c6-230">forceFIPSCompliance</span></span>|<span data-ttu-id="e18c6-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="e18c6-231">Boolean</span></span>|<span data-ttu-id="e18c6-232">Especifique se a conformidade com FIPS deve ser forçada.</span><span class="sxs-lookup"><span data-stu-id="e18c6-232">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="e18c6-233">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e18c6-233">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="e18c6-234">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="e18c6-234">networkSingleSignOn</span></span>|[<span data-ttu-id="e18c6-235">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="e18c6-235">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="e18c6-236">Especifique o tipo de logon único na rede.</span><span class="sxs-lookup"><span data-stu-id="e18c6-236">Specify the network single sign on type.</span></span> <span data-ttu-id="e18c6-237">Os valores possíveis são: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="e18c6-237">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="e18c6-238">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="e18c6-238">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="e18c6-239">Int32</span><span class="sxs-lookup"><span data-stu-id="e18c6-239">Int32</span></span>|<span data-ttu-id="e18c6-240">Especifique o tempo limite máximo de autenticação (em segundos).</span><span class="sxs-lookup"><span data-stu-id="e18c6-240">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="e18c6-241">Intervalo válido: 1-120</span><span class="sxs-lookup"><span data-stu-id="e18c6-241">Valid range: 1-120</span></span>|
|<span data-ttu-id="e18c6-242">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="e18c6-242">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="e18c6-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="e18c6-243">Boolean</span></span>|<span data-ttu-id="e18c6-244">Especifique se a conexão WiFi deve solicitar credenciais de autenticação adicionais.</span><span class="sxs-lookup"><span data-stu-id="e18c6-244">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="e18c6-245">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="e18c6-245">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="e18c6-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="e18c6-246">Boolean</span></span>|<span data-ttu-id="e18c6-247">Especifique se a conexão WiFi deve habilitar o cache da chave mestra de par.</span><span class="sxs-lookup"><span data-stu-id="e18c6-247">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="e18c6-248">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="e18c6-248">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="e18c6-249">Int32</span><span class="sxs-lookup"><span data-stu-id="e18c6-249">Int32</span></span>|<span data-ttu-id="e18c6-250">Especifique o tempo máximo de cache da chave mestra de paridade (em minutos).</span><span class="sxs-lookup"><span data-stu-id="e18c6-250">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="e18c6-251">Intervalo válido: 5-1440</span><span class="sxs-lookup"><span data-stu-id="e18c6-251">Valid range: 5-1440</span></span>|
|<span data-ttu-id="e18c6-252">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="e18c6-252">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="e18c6-253">Int32</span><span class="sxs-lookup"><span data-stu-id="e18c6-253">Int32</span></span>|<span data-ttu-id="e18c6-254">Especifique o número máximo de chaves de mestre emparelhadas no cache.</span><span class="sxs-lookup"><span data-stu-id="e18c6-254">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="e18c6-255">Intervalo válido: 1-255</span><span class="sxs-lookup"><span data-stu-id="e18c6-255">Valid range: 1-255</span></span>|
|<span data-ttu-id="e18c6-256">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="e18c6-256">enablePreAuthentication</span></span>|<span data-ttu-id="e18c6-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="e18c6-257">Boolean</span></span>|<span data-ttu-id="e18c6-258">Especifique se a pré-autenticação deve ser habilitada.</span><span class="sxs-lookup"><span data-stu-id="e18c6-258">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="e18c6-259">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="e18c6-259">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="e18c6-260">Int32</span><span class="sxs-lookup"><span data-stu-id="e18c6-260">Int32</span></span>|<span data-ttu-id="e18c6-261">Especifique as tentativas máximas de pré-autenticação.</span><span class="sxs-lookup"><span data-stu-id="e18c6-261">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="e18c6-262">Intervalo válido: 1-16</span><span class="sxs-lookup"><span data-stu-id="e18c6-262">Valid range: 1-16</span></span>|
|<span data-ttu-id="e18c6-263">eapType</span><span class="sxs-lookup"><span data-stu-id="e18c6-263">eapType</span></span>|[<span data-ttu-id="e18c6-264">eapType</span><span class="sxs-lookup"><span data-stu-id="e18c6-264">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="e18c6-265">EAP (protocolo de autenticação extensível).</span><span class="sxs-lookup"><span data-stu-id="e18c6-265">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="e18c6-266">Indica o tipo de protocolo EAP definido no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="e18c6-266">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="e18c6-267">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="e18c6-267">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="e18c6-268">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="e18c6-268">trustedServerCertificateNames</span></span>|<span data-ttu-id="e18c6-269">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e18c6-269">String collection</span></span>|<span data-ttu-id="e18c6-270">Especificar nomes de certificado de servidor confiável.</span><span class="sxs-lookup"><span data-stu-id="e18c6-270">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="e18c6-271">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e18c6-271">authenticationMethod</span></span>|[<span data-ttu-id="e18c6-272">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e18c6-272">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="e18c6-273">Especifique o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="e18c6-273">Specify the authentication method.</span></span> <span data-ttu-id="e18c6-274">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="e18c6-274">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="e18c6-275">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="e18c6-275">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="e18c6-276">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="e18c6-276">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="e18c6-277">Especificar o protocolo de autenticação interna para EAP TTLS.</span><span class="sxs-lookup"><span data-stu-id="e18c6-277">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="e18c6-278">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="e18c6-278">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="e18c6-279">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="e18c6-279">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="e18c6-280">String</span><span class="sxs-lookup"><span data-stu-id="e18c6-280">String</span></span>|<span data-ttu-id="e18c6-281">Especifique a cadeia de caracteres para substituir os nomes de texto para privacidade ao usar EAP TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="e18c6-281">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="e18c6-282">Resposta</span><span class="sxs-lookup"><span data-stu-id="e18c6-282">Response</span></span>
<span data-ttu-id="e18c6-283">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e18c6-283">If successful, this method returns a `201 Created` response code and a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e18c6-284">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e18c6-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="e18c6-285">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e18c6-285">Request</span></span>
<span data-ttu-id="e18c6-286">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e18c6-286">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e18c6-287">Resposta</span><span class="sxs-lookup"><span data-stu-id="e18c6-287">Response</span></span>
<span data-ttu-id="e18c6-p134">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e18c6-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




