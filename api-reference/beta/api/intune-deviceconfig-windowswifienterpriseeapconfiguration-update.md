---
title: Atualizar windowsWifiEnterpriseEAPConfiguration
description: Atualiza as propriedades de um objeto windowsWifiEnterpriseEAPConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b0119e99ea7bf14b6177134157d9fd9b9008bb8b
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790347"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="2805b-103">Atualizar windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="2805b-103">Update windowsWifiEnterpriseEAPConfiguration</span></span>

<span data-ttu-id="2805b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2805b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2805b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2805b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2805b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2805b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2805b-107">Atualiza as propriedades de um objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2805b-107">Update the properties of a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2805b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2805b-108">Prerequisites</span></span>
<span data-ttu-id="2805b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2805b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2805b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2805b-111">Permission type</span></span>|<span data-ttu-id="2805b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2805b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2805b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2805b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2805b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2805b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2805b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2805b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2805b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2805b-116">Not supported.</span></span>|
|<span data-ttu-id="2805b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2805b-117">Application</span></span>|<span data-ttu-id="2805b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2805b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2805b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2805b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2805b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2805b-120">Request headers</span></span>
|<span data-ttu-id="2805b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2805b-121">Header</span></span>|<span data-ttu-id="2805b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2805b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2805b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2805b-123">Authorization</span></span>|<span data-ttu-id="2805b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2805b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2805b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2805b-125">Accept</span></span>|<span data-ttu-id="2805b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2805b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2805b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2805b-127">Request body</span></span>
<span data-ttu-id="2805b-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2805b-128">In the request body, supply a JSON representation for the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

<span data-ttu-id="2805b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2805b-129">The following table shows the properties that are required when you create the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

|<span data-ttu-id="2805b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2805b-130">Property</span></span>|<span data-ttu-id="2805b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2805b-131">Type</span></span>|<span data-ttu-id="2805b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2805b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2805b-133">id</span><span class="sxs-lookup"><span data-stu-id="2805b-133">id</span></span>|<span data-ttu-id="2805b-134">String</span><span class="sxs-lookup"><span data-stu-id="2805b-134">String</span></span>|<span data-ttu-id="2805b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2805b-135">Key of the entity.</span></span> <span data-ttu-id="2805b-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2805b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2805b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2805b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2805b-138">DateTimeOffset</span></span>|<span data-ttu-id="2805b-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2805b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2805b-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2805b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2805b-141">roleScopeTagIds</span></span>|<span data-ttu-id="2805b-142">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2805b-142">String collection</span></span>|<span data-ttu-id="2805b-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="2805b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2805b-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2805b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2805b-145">supportsScopeTags</span></span>|<span data-ttu-id="2805b-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="2805b-146">Boolean</span></span>|<span data-ttu-id="2805b-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="2805b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2805b-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="2805b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2805b-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="2805b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2805b-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2805b-150">This property is read-only.</span></span> <span data-ttu-id="2805b-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2805b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2805b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2805b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2805b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2805b-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="2805b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2805b-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2805b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2805b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2805b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2805b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2805b-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="2805b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2805b-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2805b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2805b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2805b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2805b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2805b-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="2805b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2805b-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2805b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2805b-164">createdDateTime</span></span>|<span data-ttu-id="2805b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2805b-165">DateTimeOffset</span></span>|<span data-ttu-id="2805b-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2805b-166">DateTime the object was created.</span></span> <span data-ttu-id="2805b-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2805b-168">description</span><span class="sxs-lookup"><span data-stu-id="2805b-168">description</span></span>|<span data-ttu-id="2805b-169">String</span><span class="sxs-lookup"><span data-stu-id="2805b-169">String</span></span>|<span data-ttu-id="2805b-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2805b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2805b-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2805b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="2805b-172">displayName</span></span>|<span data-ttu-id="2805b-173">String</span><span class="sxs-lookup"><span data-stu-id="2805b-173">String</span></span>|<span data-ttu-id="2805b-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2805b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2805b-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2805b-176">versão</span><span class="sxs-lookup"><span data-stu-id="2805b-176">version</span></span>|<span data-ttu-id="2805b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2805b-177">Int32</span></span>|<span data-ttu-id="2805b-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2805b-178">Version of the device configuration.</span></span> <span data-ttu-id="2805b-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2805b-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="2805b-180">preSharedKey</span></span>|<span data-ttu-id="2805b-181">String</span><span class="sxs-lookup"><span data-stu-id="2805b-181">String</span></span>|<span data-ttu-id="2805b-182">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="2805b-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="2805b-183">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-183">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2805b-184">à</span><span class="sxs-lookup"><span data-stu-id="2805b-184">wifiSecurityType</span></span>|[<span data-ttu-id="2805b-185">à</span><span class="sxs-lookup"><span data-stu-id="2805b-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="2805b-186">Especifique o tipo de segurança wifi.</span><span class="sxs-lookup"><span data-stu-id="2805b-186">Specify the Wifi Security Type.</span></span> <span data-ttu-id="2805b-187">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2805b-187">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="2805b-188">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="2805b-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="2805b-189">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="2805b-189">meteredConnectionLimit</span></span>|[<span data-ttu-id="2805b-190">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="2805b-190">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="2805b-191">Especifique o tipo de limite de conexão limitada para a conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="2805b-191">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="2805b-192">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2805b-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="2805b-193">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="2805b-193">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="2805b-194">SSID</span><span class="sxs-lookup"><span data-stu-id="2805b-194">ssid</span></span>|<span data-ttu-id="2805b-195">String</span><span class="sxs-lookup"><span data-stu-id="2805b-195">String</span></span>|<span data-ttu-id="2805b-196">Especifique o SSID da conexão WiFi.</span><span class="sxs-lookup"><span data-stu-id="2805b-196">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="2805b-197">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2805b-198">NetworkName</span><span class="sxs-lookup"><span data-stu-id="2805b-198">networkName</span></span>|<span data-ttu-id="2805b-199">String</span><span class="sxs-lookup"><span data-stu-id="2805b-199">String</span></span>|<span data-ttu-id="2805b-200">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="2805b-200">Specify the network configuration name.</span></span> <span data-ttu-id="2805b-201">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2805b-202">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="2805b-202">connectAutomatically</span></span>|<span data-ttu-id="2805b-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="2805b-203">Boolean</span></span>|<span data-ttu-id="2805b-204">Especifique se a conexão WiFi deve se conectar automaticamente quando estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="2805b-204">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="2805b-205">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-205">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2805b-206">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="2805b-206">connectToPreferredNetwork</span></span>|<span data-ttu-id="2805b-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="2805b-207">Boolean</span></span>|<span data-ttu-id="2805b-208">Especifique se a conexão WiFi deve se conectar a redes mais preferenciais quando já estiver conectado a ela.</span><span class="sxs-lookup"><span data-stu-id="2805b-208">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="2805b-209">Requer que ConnectAutomatically seja true.</span><span class="sxs-lookup"><span data-stu-id="2805b-209">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="2805b-210">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2805b-211">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="2805b-211">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="2805b-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="2805b-212">Boolean</span></span>|<span data-ttu-id="2805b-213">Especifique se a conexão WiFi deve se conectar automaticamente, mesmo quando o SSID não estiver transmitindo.</span><span class="sxs-lookup"><span data-stu-id="2805b-213">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="2805b-214">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2805b-215">proxySetting</span><span class="sxs-lookup"><span data-stu-id="2805b-215">proxySetting</span></span>|[<span data-ttu-id="2805b-216">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="2805b-216">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="2805b-217">Especifique a configuração de proxy para a configuração de Wi-Fi herdada de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2805b-217">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="2805b-218">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="2805b-218">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="2805b-219">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="2805b-219">proxyManualAddress</span></span>|<span data-ttu-id="2805b-220">String</span><span class="sxs-lookup"><span data-stu-id="2805b-220">String</span></span>|<span data-ttu-id="2805b-221">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="2805b-221">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="2805b-222">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2805b-223">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="2805b-223">proxyManualPort</span></span>|<span data-ttu-id="2805b-224">Int32</span><span class="sxs-lookup"><span data-stu-id="2805b-224">Int32</span></span>|<span data-ttu-id="2805b-225">Especifique a porta do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="2805b-225">Specify the port for the proxy server.</span></span> <span data-ttu-id="2805b-226">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-226">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2805b-227">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="2805b-227">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="2805b-228">String</span><span class="sxs-lookup"><span data-stu-id="2805b-228">String</span></span>|<span data-ttu-id="2805b-229">Especifique a URL do script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="2805b-229">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="2805b-230">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-230">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2805b-231">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="2805b-231">forceFIPSCompliance</span></span>|<span data-ttu-id="2805b-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="2805b-232">Boolean</span></span>|<span data-ttu-id="2805b-233">Especifique se a conformidade com FIPS deve ser forçada.</span><span class="sxs-lookup"><span data-stu-id="2805b-233">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="2805b-234">Herdado de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2805b-234">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="2805b-235">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="2805b-235">networkSingleSignOn</span></span>|[<span data-ttu-id="2805b-236">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="2805b-236">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="2805b-237">Especifique o tipo de logon único na rede.</span><span class="sxs-lookup"><span data-stu-id="2805b-237">Specify the network single sign on type.</span></span> <span data-ttu-id="2805b-238">Os valores possíveis são: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="2805b-238">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="2805b-239">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="2805b-239">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="2805b-240">Int32</span><span class="sxs-lookup"><span data-stu-id="2805b-240">Int32</span></span>|<span data-ttu-id="2805b-241">Especifique o tempo limite máximo de autenticação (em segundos).</span><span class="sxs-lookup"><span data-stu-id="2805b-241">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="2805b-242">Intervalo válido: 1-120</span><span class="sxs-lookup"><span data-stu-id="2805b-242">Valid range: 1-120</span></span>|
|<span data-ttu-id="2805b-243">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="2805b-243">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="2805b-244">Booliano</span><span class="sxs-lookup"><span data-stu-id="2805b-244">Boolean</span></span>|<span data-ttu-id="2805b-245">Especifique se a conexão WiFi deve solicitar credenciais de autenticação adicionais.</span><span class="sxs-lookup"><span data-stu-id="2805b-245">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="2805b-246">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="2805b-246">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="2805b-247">Booliano</span><span class="sxs-lookup"><span data-stu-id="2805b-247">Boolean</span></span>|<span data-ttu-id="2805b-248">Especifique se a conexão WiFi deve habilitar o cache da chave mestra de par.</span><span class="sxs-lookup"><span data-stu-id="2805b-248">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="2805b-249">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="2805b-249">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="2805b-250">Int32</span><span class="sxs-lookup"><span data-stu-id="2805b-250">Int32</span></span>|<span data-ttu-id="2805b-251">Especifique o tempo máximo de cache da chave mestra de paridade (em minutos).</span><span class="sxs-lookup"><span data-stu-id="2805b-251">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="2805b-252">Intervalo válido: 5-1440</span><span class="sxs-lookup"><span data-stu-id="2805b-252">Valid range: 5-1440</span></span>|
|<span data-ttu-id="2805b-253">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="2805b-253">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="2805b-254">Int32</span><span class="sxs-lookup"><span data-stu-id="2805b-254">Int32</span></span>|<span data-ttu-id="2805b-255">Especifique o número máximo de chaves de mestre emparelhadas no cache.</span><span class="sxs-lookup"><span data-stu-id="2805b-255">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="2805b-256">Intervalo válido: 1-255</span><span class="sxs-lookup"><span data-stu-id="2805b-256">Valid range: 1-255</span></span>|
|<span data-ttu-id="2805b-257">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="2805b-257">enablePreAuthentication</span></span>|<span data-ttu-id="2805b-258">Booliano</span><span class="sxs-lookup"><span data-stu-id="2805b-258">Boolean</span></span>|<span data-ttu-id="2805b-259">Especifique se a pré-autenticação deve ser habilitada.</span><span class="sxs-lookup"><span data-stu-id="2805b-259">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="2805b-260">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="2805b-260">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="2805b-261">Int32</span><span class="sxs-lookup"><span data-stu-id="2805b-261">Int32</span></span>|<span data-ttu-id="2805b-262">Especifique as tentativas máximas de pré-autenticação.</span><span class="sxs-lookup"><span data-stu-id="2805b-262">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="2805b-263">Intervalo válido: 1-16</span><span class="sxs-lookup"><span data-stu-id="2805b-263">Valid range: 1-16</span></span>|
|<span data-ttu-id="2805b-264">eapType</span><span class="sxs-lookup"><span data-stu-id="2805b-264">eapType</span></span>|[<span data-ttu-id="2805b-265">eapType</span><span class="sxs-lookup"><span data-stu-id="2805b-265">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="2805b-266">EAP (protocolo de autenticação extensível).</span><span class="sxs-lookup"><span data-stu-id="2805b-266">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="2805b-267">Indica o tipo de protocolo EAP definido no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="2805b-267">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="2805b-268">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="2805b-268">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="2805b-269">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="2805b-269">trustedServerCertificateNames</span></span>|<span data-ttu-id="2805b-270">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2805b-270">String collection</span></span>|<span data-ttu-id="2805b-271">Especificar nomes de certificado de servidor confiável.</span><span class="sxs-lookup"><span data-stu-id="2805b-271">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="2805b-272">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2805b-272">authenticationMethod</span></span>|[<span data-ttu-id="2805b-273">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2805b-273">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="2805b-274">Especifique o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="2805b-274">Specify the authentication method.</span></span> <span data-ttu-id="2805b-275">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="2805b-275">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="2805b-276">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="2805b-276">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="2805b-277">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="2805b-277">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="2805b-278">Especificar o protocolo de autenticação interna para EAP TTLS.</span><span class="sxs-lookup"><span data-stu-id="2805b-278">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="2805b-279">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="2805b-279">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="2805b-280">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="2805b-280">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="2805b-281">String</span><span class="sxs-lookup"><span data-stu-id="2805b-281">String</span></span>|<span data-ttu-id="2805b-282">Especifique a cadeia de caracteres para substituir os nomes de texto para privacidade ao usar EAP TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="2805b-282">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|
|<span data-ttu-id="2805b-283">requireCryptographicBinding</span><span class="sxs-lookup"><span data-stu-id="2805b-283">requireCryptographicBinding</span></span>|<span data-ttu-id="2805b-284">Booliano</span><span class="sxs-lookup"><span data-stu-id="2805b-284">Boolean</span></span>|<span data-ttu-id="2805b-285">Especifique se deseja habilitar a associação criptográfica quando o tipo EAP for selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="2805b-285">Specify whether to enable cryptographic binding when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="2805b-286">performServerValidation</span><span class="sxs-lookup"><span data-stu-id="2805b-286">performServerValidation</span></span>|<span data-ttu-id="2805b-287">Booliano</span><span class="sxs-lookup"><span data-stu-id="2805b-287">Boolean</span></span>|<span data-ttu-id="2805b-288">Especifique se deseja habilitar a verificação da identidade do servidor, validando o certificado quando o tipo EAP estiver selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="2805b-288">Specify whether to enable verification of server's identity by validating the certificate when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="2805b-289">disableUserPromptForServerValidation</span><span class="sxs-lookup"><span data-stu-id="2805b-289">disableUserPromptForServerValidation</span></span>|<span data-ttu-id="2805b-290">Booliano</span><span class="sxs-lookup"><span data-stu-id="2805b-290">Boolean</span></span>|<span data-ttu-id="2805b-291">Especifique se deseja impedir que o usuário seja solicitado a autorizar novos servidores para autoridades de certificação confiáveis quando o tipo EAP for selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="2805b-291">Specify whether to prevent the user from being prompted to authorize new servers for trusted certification authorities when EAP type is selected as PEAP.</span></span>|



## <a name="response"></a><span data-ttu-id="2805b-292">Resposta</span><span class="sxs-lookup"><span data-stu-id="2805b-292">Response</span></span>
<span data-ttu-id="2805b-293">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2805b-293">If successful, this method returns a `200 OK` response code and an updated [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2805b-294">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2805b-294">Example</span></span>

### <a name="request"></a><span data-ttu-id="2805b-295">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2805b-295">Request</span></span>
<span data-ttu-id="2805b-296">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2805b-296">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="2805b-297">Resposta</span><span class="sxs-lookup"><span data-stu-id="2805b-297">Response</span></span>
<span data-ttu-id="2805b-p134">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2805b-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



