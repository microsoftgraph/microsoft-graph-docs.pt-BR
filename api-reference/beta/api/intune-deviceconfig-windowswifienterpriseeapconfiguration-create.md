---
title: Criar windowsWifiEnterpriseEAPConfiguration
description: Criar um novo objeto windowsWifiEnterpriseEAPConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b47e1ba1fffaf7e194c5ac287903f28d13bfdb57
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990043"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="1ecfb-103">Criar windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ecfb-103">Create windowsWifiEnterpriseEAPConfiguration</span></span>

<span data-ttu-id="1ecfb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ecfb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ecfb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ecfb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ecfb-107">Criar um novo objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1ecfb-107">Create a new [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ecfb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1ecfb-108">Prerequisites</span></span>
<span data-ttu-id="1ecfb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ecfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ecfb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ecfb-111">Permission type</span></span>|<span data-ttu-id="1ecfb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ecfb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ecfb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ecfb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ecfb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ecfb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-116">Not supported.</span></span>|
|<span data-ttu-id="1ecfb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ecfb-117">Application</span></span>|<span data-ttu-id="1ecfb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ecfb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ecfb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ecfb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1ecfb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ecfb-120">Request headers</span></span>
|<span data-ttu-id="1ecfb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ecfb-121">Header</span></span>|<span data-ttu-id="1ecfb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1ecfb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ecfb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ecfb-123">Authorization</span></span>|<span data-ttu-id="1ecfb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ecfb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1ecfb-125">Accept</span></span>|<span data-ttu-id="1ecfb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ecfb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ecfb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ecfb-127">Request body</span></span>
<span data-ttu-id="1ecfb-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsWifiEnterpriseEAPConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-128">In the request body, supply a JSON representation for the windowsWifiEnterpriseEAPConfiguration object.</span></span>

<span data-ttu-id="1ecfb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsWifiEnterpriseEAPConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-129">The following table shows the properties that are required when you create the windowsWifiEnterpriseEAPConfiguration.</span></span>

|<span data-ttu-id="1ecfb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ecfb-130">Property</span></span>|<span data-ttu-id="1ecfb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ecfb-131">Type</span></span>|<span data-ttu-id="1ecfb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ecfb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ecfb-133">id</span><span class="sxs-lookup"><span data-stu-id="1ecfb-133">id</span></span>|<span data-ttu-id="1ecfb-134">String</span><span class="sxs-lookup"><span data-stu-id="1ecfb-134">String</span></span>|<span data-ttu-id="1ecfb-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-135">Key of the entity.</span></span> <span data-ttu-id="1ecfb-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ecfb-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1ecfb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ecfb-138">DateTimeOffset</span></span>|<span data-ttu-id="1ecfb-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1ecfb-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1ecfb-141">roleScopeTagIds</span></span>|<span data-ttu-id="1ecfb-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ecfb-142">String collection</span></span>|<span data-ttu-id="1ecfb-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1ecfb-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1ecfb-145">supportsScopeTags</span></span>|<span data-ttu-id="1ecfb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ecfb-146">Boolean</span></span>|<span data-ttu-id="1ecfb-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1ecfb-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1ecfb-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1ecfb-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-150">This property is read-only.</span></span> <span data-ttu-id="1ecfb-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1ecfb-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1ecfb-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1ecfb-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1ecfb-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1ecfb-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1ecfb-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1ecfb-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1ecfb-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1ecfb-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1ecfb-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1ecfb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1ecfb-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1ecfb-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1ecfb-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1ecfb-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ecfb-164">createdDateTime</span></span>|<span data-ttu-id="1ecfb-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ecfb-165">DateTimeOffset</span></span>|<span data-ttu-id="1ecfb-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-166">DateTime the object was created.</span></span> <span data-ttu-id="1ecfb-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-168">description</span><span class="sxs-lookup"><span data-stu-id="1ecfb-168">description</span></span>|<span data-ttu-id="1ecfb-169">String</span><span class="sxs-lookup"><span data-stu-id="1ecfb-169">String</span></span>|<span data-ttu-id="1ecfb-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1ecfb-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-172">displayName</span><span class="sxs-lookup"><span data-stu-id="1ecfb-172">displayName</span></span>|<span data-ttu-id="1ecfb-173">String</span><span class="sxs-lookup"><span data-stu-id="1ecfb-173">String</span></span>|<span data-ttu-id="1ecfb-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1ecfb-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-176">versão</span><span class="sxs-lookup"><span data-stu-id="1ecfb-176">version</span></span>|<span data-ttu-id="1ecfb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1ecfb-177">Int32</span></span>|<span data-ttu-id="1ecfb-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-178">Version of the device configuration.</span></span> <span data-ttu-id="1ecfb-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="1ecfb-180">preSharedKey</span></span>|<span data-ttu-id="1ecfb-181">String</span><span class="sxs-lookup"><span data-stu-id="1ecfb-181">String</span></span>|<span data-ttu-id="1ecfb-182">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="1ecfb-183">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-183">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-184">à</span><span class="sxs-lookup"><span data-stu-id="1ecfb-184">wifiSecurityType</span></span>|[<span data-ttu-id="1ecfb-185">à</span><span class="sxs-lookup"><span data-stu-id="1ecfb-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="1ecfb-186">Especifique o tipo de segurança wifi.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-186">Specify the Wifi Security Type.</span></span> <span data-ttu-id="1ecfb-187">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ecfb-187">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="1ecfb-188">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="1ecfb-189">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="1ecfb-189">meteredConnectionLimit</span></span>|[<span data-ttu-id="1ecfb-190">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="1ecfb-190">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="1ecfb-191">Especifique o tipo de limite de conexão limitada para a conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-191">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="1ecfb-192">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ecfb-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="1ecfb-193">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-193">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="1ecfb-194">SSID</span><span class="sxs-lookup"><span data-stu-id="1ecfb-194">ssid</span></span>|<span data-ttu-id="1ecfb-195">String</span><span class="sxs-lookup"><span data-stu-id="1ecfb-195">String</span></span>|<span data-ttu-id="1ecfb-196">Especifique o SSID da conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-196">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="1ecfb-197">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-198">NetworkName</span><span class="sxs-lookup"><span data-stu-id="1ecfb-198">networkName</span></span>|<span data-ttu-id="1ecfb-199">String</span><span class="sxs-lookup"><span data-stu-id="1ecfb-199">String</span></span>|<span data-ttu-id="1ecfb-200">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-200">Specify the network configuration name.</span></span> <span data-ttu-id="1ecfb-201">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-202">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="1ecfb-202">connectAutomatically</span></span>|<span data-ttu-id="1ecfb-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ecfb-203">Boolean</span></span>|<span data-ttu-id="1ecfb-204">Especifique se a conexão WiFi deve se conectar automaticamente quando estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-204">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="1ecfb-205">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-205">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-206">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="1ecfb-206">connectToPreferredNetwork</span></span>|<span data-ttu-id="1ecfb-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ecfb-207">Boolean</span></span>|<span data-ttu-id="1ecfb-208">Especifique se a conexão WiFi deve se conectar a redes mais preferenciais quando já estiver conectado a ela.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-208">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="1ecfb-209">Requer que ConnectAutomatically seja true.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-209">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="1ecfb-210">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-211">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="1ecfb-211">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="1ecfb-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ecfb-212">Boolean</span></span>|<span data-ttu-id="1ecfb-213">Especifique se a conexão WiFi deve se conectar automaticamente, mesmo quando o SSID não estiver transmitindo.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-213">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="1ecfb-214">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-215">proxySetting</span><span class="sxs-lookup"><span data-stu-id="1ecfb-215">proxySetting</span></span>|[<span data-ttu-id="1ecfb-216">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="1ecfb-216">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="1ecfb-217">Especifique a configuração de proxy para a configuração de Wi-Fi herdada de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1ecfb-217">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="1ecfb-218">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-218">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="1ecfb-219">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="1ecfb-219">proxyManualAddress</span></span>|<span data-ttu-id="1ecfb-220">String</span><span class="sxs-lookup"><span data-stu-id="1ecfb-220">String</span></span>|<span data-ttu-id="1ecfb-221">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-221">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="1ecfb-222">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-223">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="1ecfb-223">proxyManualPort</span></span>|<span data-ttu-id="1ecfb-224">Int32</span><span class="sxs-lookup"><span data-stu-id="1ecfb-224">Int32</span></span>|<span data-ttu-id="1ecfb-225">Especifique a porta do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-225">Specify the port for the proxy server.</span></span> <span data-ttu-id="1ecfb-226">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-226">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-227">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="1ecfb-227">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="1ecfb-228">String</span><span class="sxs-lookup"><span data-stu-id="1ecfb-228">String</span></span>|<span data-ttu-id="1ecfb-229">Especifique a URL do script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-229">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="1ecfb-230">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-230">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-231">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="1ecfb-231">forceFIPSCompliance</span></span>|<span data-ttu-id="1ecfb-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ecfb-232">Boolean</span></span>|<span data-ttu-id="1ecfb-233">Especifique se a conformidade com FIPS deve ser forçada.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-233">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="1ecfb-234">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1ecfb-234">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="1ecfb-235">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="1ecfb-235">networkSingleSignOn</span></span>|[<span data-ttu-id="1ecfb-236">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="1ecfb-236">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="1ecfb-237">Especifique o tipo de logon único na rede.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-237">Specify the network single sign on type.</span></span> <span data-ttu-id="1ecfb-238">Os valores possíveis são: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-238">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="1ecfb-239">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="1ecfb-239">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="1ecfb-240">Int32</span><span class="sxs-lookup"><span data-stu-id="1ecfb-240">Int32</span></span>|<span data-ttu-id="1ecfb-241">Especifique o tempo limite máximo de autenticação (em segundos).</span><span class="sxs-lookup"><span data-stu-id="1ecfb-241">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="1ecfb-242">Intervalo válido: 1-120</span><span class="sxs-lookup"><span data-stu-id="1ecfb-242">Valid range: 1-120</span></span>|
|<span data-ttu-id="1ecfb-243">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="1ecfb-243">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="1ecfb-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ecfb-244">Boolean</span></span>|<span data-ttu-id="1ecfb-245">Especifique se a conexão WiFi deve solicitar credenciais de autenticação adicionais.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-245">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="1ecfb-246">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="1ecfb-246">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="1ecfb-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ecfb-247">Boolean</span></span>|<span data-ttu-id="1ecfb-248">Especifique se a conexão WiFi deve habilitar o cache da chave mestra de par.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-248">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="1ecfb-249">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="1ecfb-249">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="1ecfb-250">Int32</span><span class="sxs-lookup"><span data-stu-id="1ecfb-250">Int32</span></span>|<span data-ttu-id="1ecfb-251">Especifique o tempo máximo de cache da chave mestra de paridade (em minutos).</span><span class="sxs-lookup"><span data-stu-id="1ecfb-251">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="1ecfb-252">Intervalo válido: 5-1440</span><span class="sxs-lookup"><span data-stu-id="1ecfb-252">Valid range: 5-1440</span></span>|
|<span data-ttu-id="1ecfb-253">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="1ecfb-253">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="1ecfb-254">Int32</span><span class="sxs-lookup"><span data-stu-id="1ecfb-254">Int32</span></span>|<span data-ttu-id="1ecfb-255">Especifique o número máximo de chaves de mestre emparelhadas no cache.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-255">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="1ecfb-256">Intervalo válido: 1-255</span><span class="sxs-lookup"><span data-stu-id="1ecfb-256">Valid range: 1-255</span></span>|
|<span data-ttu-id="1ecfb-257">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="1ecfb-257">enablePreAuthentication</span></span>|<span data-ttu-id="1ecfb-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ecfb-258">Boolean</span></span>|<span data-ttu-id="1ecfb-259">Especifique se a pré-autenticação deve ser habilitada.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-259">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="1ecfb-260">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="1ecfb-260">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="1ecfb-261">Int32</span><span class="sxs-lookup"><span data-stu-id="1ecfb-261">Int32</span></span>|<span data-ttu-id="1ecfb-262">Especifique as tentativas máximas de pré-autenticação.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-262">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="1ecfb-263">Intervalo válido: 1-16</span><span class="sxs-lookup"><span data-stu-id="1ecfb-263">Valid range: 1-16</span></span>|
|<span data-ttu-id="1ecfb-264">eapType</span><span class="sxs-lookup"><span data-stu-id="1ecfb-264">eapType</span></span>|[<span data-ttu-id="1ecfb-265">eapType</span><span class="sxs-lookup"><span data-stu-id="1ecfb-265">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="1ecfb-266">EAP (protocolo de autenticação extensível).</span><span class="sxs-lookup"><span data-stu-id="1ecfb-266">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="1ecfb-267">Indica o tipo de protocolo EAP definido no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="1ecfb-267">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="1ecfb-268">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-268">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="1ecfb-269">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="1ecfb-269">trustedServerCertificateNames</span></span>|<span data-ttu-id="1ecfb-270">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ecfb-270">String collection</span></span>|<span data-ttu-id="1ecfb-271">Especificar nomes de certificado de servidor confiável.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-271">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="1ecfb-272">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1ecfb-272">authenticationMethod</span></span>|[<span data-ttu-id="1ecfb-273">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1ecfb-273">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="1ecfb-274">Especifique o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-274">Specify the authentication method.</span></span> <span data-ttu-id="1ecfb-275">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-275">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="1ecfb-276">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="1ecfb-276">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="1ecfb-277">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="1ecfb-277">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="1ecfb-278">Especificar o protocolo de autenticação interna para EAP TTLS.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-278">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="1ecfb-279">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-279">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="1ecfb-280">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="1ecfb-280">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="1ecfb-281">String</span><span class="sxs-lookup"><span data-stu-id="1ecfb-281">String</span></span>|<span data-ttu-id="1ecfb-282">Especifique a cadeia de caracteres para substituir os nomes de texto para privacidade ao usar EAP TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-282">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|
|<span data-ttu-id="1ecfb-283">requireCryptographicBinding</span><span class="sxs-lookup"><span data-stu-id="1ecfb-283">requireCryptographicBinding</span></span>|<span data-ttu-id="1ecfb-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ecfb-284">Boolean</span></span>|<span data-ttu-id="1ecfb-285">Especifique se deseja habilitar a associação criptográfica quando o tipo EAP for selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-285">Specify whether to enable cryptographic binding when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="1ecfb-286">performServerValidation</span><span class="sxs-lookup"><span data-stu-id="1ecfb-286">performServerValidation</span></span>|<span data-ttu-id="1ecfb-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ecfb-287">Boolean</span></span>|<span data-ttu-id="1ecfb-288">Especifique se deseja habilitar a verificação da identidade do servidor, validando o certificado quando o tipo EAP estiver selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-288">Specify whether to enable verification of server's identity by validating the certificate when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="1ecfb-289">disableUserPromptForServerValidation</span><span class="sxs-lookup"><span data-stu-id="1ecfb-289">disableUserPromptForServerValidation</span></span>|<span data-ttu-id="1ecfb-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ecfb-290">Boolean</span></span>|<span data-ttu-id="1ecfb-291">Especifique se deseja impedir que o usuário seja solicitado a autorizar novos servidores para autoridades de certificação confiáveis quando o tipo EAP for selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-291">Specify whether to prevent the user from being prompted to authorize new servers for trusted certification authorities when EAP type is selected as PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="1ecfb-292">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ecfb-292">Response</span></span>
<span data-ttu-id="1ecfb-293">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-293">If successful, this method returns a `201 Created` response code and a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ecfb-294">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ecfb-294">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ecfb-295">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ecfb-295">Request</span></span>
<span data-ttu-id="1ecfb-296">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-296">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2402

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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "requireCryptographicBinding": true,
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true
}
```

### <a name="response"></a><span data-ttu-id="1ecfb-297">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ecfb-297">Response</span></span>
<span data-ttu-id="1ecfb-p134">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ecfb-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2574

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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "requireCryptographicBinding": true,
  "performServerValidation": true,
  "disableUserPromptForServerValidation": true
}
```






