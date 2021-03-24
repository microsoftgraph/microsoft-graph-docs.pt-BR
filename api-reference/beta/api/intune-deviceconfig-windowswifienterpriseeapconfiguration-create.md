---
title: Criar windowsWifiEnterpriseEAPConfiguration
description: Crie um novo objeto windowsWifiEnterpriseEAPConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e391e1167159d244a5a5ad9ad8a867aaed80bb47
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147074"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="54bd2-103">Criar windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="54bd2-103">Create windowsWifiEnterpriseEAPConfiguration</span></span>

<span data-ttu-id="54bd2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54bd2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54bd2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54bd2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54bd2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54bd2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54bd2-107">Crie um novo [objeto windowsWifiEnterpriseEAPConfiguration.](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-107">Create a new [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54bd2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54bd2-108">Prerequisites</span></span>
<span data-ttu-id="54bd2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54bd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54bd2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54bd2-111">Permission type</span></span>|<span data-ttu-id="54bd2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54bd2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54bd2-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54bd2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54bd2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54bd2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="54bd2-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54bd2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54bd2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54bd2-116">Not supported.</span></span>|
|<span data-ttu-id="54bd2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54bd2-117">Application</span></span>|<span data-ttu-id="54bd2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54bd2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54bd2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54bd2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="54bd2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54bd2-120">Request headers</span></span>
|<span data-ttu-id="54bd2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54bd2-121">Header</span></span>|<span data-ttu-id="54bd2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="54bd2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54bd2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="54bd2-123">Authorization</span></span>|<span data-ttu-id="54bd2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54bd2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54bd2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="54bd2-125">Accept</span></span>|<span data-ttu-id="54bd2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54bd2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54bd2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54bd2-127">Request body</span></span>
<span data-ttu-id="54bd2-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsWifiEnterpriseEAPConfiguration.</span><span class="sxs-lookup"><span data-stu-id="54bd2-128">In the request body, supply a JSON representation for the windowsWifiEnterpriseEAPConfiguration object.</span></span>

<span data-ttu-id="54bd2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o windowsWifiEnterpriseEAPConfiguration.</span><span class="sxs-lookup"><span data-stu-id="54bd2-129">The following table shows the properties that are required when you create the windowsWifiEnterpriseEAPConfiguration.</span></span>

|<span data-ttu-id="54bd2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54bd2-130">Property</span></span>|<span data-ttu-id="54bd2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="54bd2-131">Type</span></span>|<span data-ttu-id="54bd2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="54bd2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54bd2-133">id</span><span class="sxs-lookup"><span data-stu-id="54bd2-133">id</span></span>|<span data-ttu-id="54bd2-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54bd2-134">String</span></span>|<span data-ttu-id="54bd2-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="54bd2-135">Key of the entity.</span></span> <span data-ttu-id="54bd2-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54bd2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="54bd2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54bd2-138">DateTimeOffset</span></span>|<span data-ttu-id="54bd2-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="54bd2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="54bd2-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="54bd2-141">roleScopeTagIds</span></span>|<span data-ttu-id="54bd2-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="54bd2-142">String collection</span></span>|<span data-ttu-id="54bd2-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="54bd2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="54bd2-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="54bd2-145">supportsScopeTags</span></span>|<span data-ttu-id="54bd2-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="54bd2-146">Boolean</span></span>|<span data-ttu-id="54bd2-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="54bd2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="54bd2-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="54bd2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="54bd2-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="54bd2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="54bd2-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54bd2-150">This property is read-only.</span></span> <span data-ttu-id="54bd2-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="54bd2-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="54bd2-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="54bd2-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="54bd2-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="54bd2-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="54bd2-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="54bd2-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="54bd2-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="54bd2-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="54bd2-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="54bd2-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="54bd2-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="54bd2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="54bd2-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="54bd2-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="54bd2-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="54bd2-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="54bd2-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54bd2-164">createdDateTime</span></span>|<span data-ttu-id="54bd2-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54bd2-165">DateTimeOffset</span></span>|<span data-ttu-id="54bd2-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="54bd2-166">DateTime the object was created.</span></span> <span data-ttu-id="54bd2-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-168">descrição</span><span class="sxs-lookup"><span data-stu-id="54bd2-168">description</span></span>|<span data-ttu-id="54bd2-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54bd2-169">String</span></span>|<span data-ttu-id="54bd2-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54bd2-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="54bd2-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-172">displayName</span><span class="sxs-lookup"><span data-stu-id="54bd2-172">displayName</span></span>|<span data-ttu-id="54bd2-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54bd2-173">String</span></span>|<span data-ttu-id="54bd2-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54bd2-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="54bd2-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-176">versão</span><span class="sxs-lookup"><span data-stu-id="54bd2-176">version</span></span>|<span data-ttu-id="54bd2-177">Int32</span><span class="sxs-lookup"><span data-stu-id="54bd2-177">Int32</span></span>|<span data-ttu-id="54bd2-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54bd2-178">Version of the device configuration.</span></span> <span data-ttu-id="54bd2-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-180">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="54bd2-180">preSharedKey</span></span>|<span data-ttu-id="54bd2-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54bd2-181">String</span></span>|<span data-ttu-id="54bd2-182">Esta é a chave pré-compartilhada para a rede WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="54bd2-182">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="54bd2-183">Herdado do [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-183">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-184">wifiSecurityType</span><span class="sxs-lookup"><span data-stu-id="54bd2-184">wifiSecurityType</span></span>|[<span data-ttu-id="54bd2-185">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="54bd2-185">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="54bd2-186">Especifique o Tipo de Segurança Wifi.</span><span class="sxs-lookup"><span data-stu-id="54bd2-186">Specify the Wifi Security Type.</span></span> <span data-ttu-id="54bd2-187">Herdado [do windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54bd2-187">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="54bd2-188">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="54bd2-188">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="54bd2-189">meteredConnectionLimit</span><span class="sxs-lookup"><span data-stu-id="54bd2-189">meteredConnectionLimit</span></span>|[<span data-ttu-id="54bd2-190">meteredConnectionLimitType</span><span class="sxs-lookup"><span data-stu-id="54bd2-190">meteredConnectionLimitType</span></span>](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|<span data-ttu-id="54bd2-191">Especifique o tipo de limite de conexão limitado para a conexão wifi.</span><span class="sxs-lookup"><span data-stu-id="54bd2-191">Specify the metered connection limit type for the wifi connection.</span></span> <span data-ttu-id="54bd2-192">Herdado [do windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54bd2-192">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="54bd2-193">Os valores possíveis são: `unrestricted`, `fixed`, `variable`.</span><span class="sxs-lookup"><span data-stu-id="54bd2-193">Possible values are: `unrestricted`, `fixed`, `variable`.</span></span>|
|<span data-ttu-id="54bd2-194">ssid</span><span class="sxs-lookup"><span data-stu-id="54bd2-194">ssid</span></span>|<span data-ttu-id="54bd2-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54bd2-195">String</span></span>|<span data-ttu-id="54bd2-196">Especifique o SSID da conexão wifi.</span><span class="sxs-lookup"><span data-stu-id="54bd2-196">Specify the SSID of the wifi connection.</span></span> <span data-ttu-id="54bd2-197">Herdado do [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-197">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-198">networkName</span><span class="sxs-lookup"><span data-stu-id="54bd2-198">networkName</span></span>|<span data-ttu-id="54bd2-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54bd2-199">String</span></span>|<span data-ttu-id="54bd2-200">Especifique o nome da configuração de rede.</span><span class="sxs-lookup"><span data-stu-id="54bd2-200">Specify the network configuration name.</span></span> <span data-ttu-id="54bd2-201">Herdado do [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-201">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-202">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="54bd2-202">connectAutomatically</span></span>|<span data-ttu-id="54bd2-203">Booleano</span><span class="sxs-lookup"><span data-stu-id="54bd2-203">Boolean</span></span>|<span data-ttu-id="54bd2-204">Especifique se a conexão wifi deve se conectar automaticamente quando estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="54bd2-204">Specify whether the wifi connection should connect automatically when in range.</span></span> <span data-ttu-id="54bd2-205">Herdado do [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-205">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-206">connectToPreferredNetwork</span><span class="sxs-lookup"><span data-stu-id="54bd2-206">connectToPreferredNetwork</span></span>|<span data-ttu-id="54bd2-207">Booleano</span><span class="sxs-lookup"><span data-stu-id="54bd2-207">Boolean</span></span>|<span data-ttu-id="54bd2-208">Especifique se a conexão wifi deve se conectar a redes mais preferenciais quando já estiver conectada a essa.</span><span class="sxs-lookup"><span data-stu-id="54bd2-208">Specify whether the wifi connection should connect to more preferred networks when already connected to this one.</span></span>  <span data-ttu-id="54bd2-209">Requer Que ConnectAutomatically seja verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="54bd2-209">Requires ConnectAutomatically to be true.</span></span> <span data-ttu-id="54bd2-210">Herdado do [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-210">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-211">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="54bd2-211">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="54bd2-212">Booleano</span><span class="sxs-lookup"><span data-stu-id="54bd2-212">Boolean</span></span>|<span data-ttu-id="54bd2-213">Especifique se a conexão wifi deve se conectar automaticamente mesmo quando o SSID não estiver transmitindo.</span><span class="sxs-lookup"><span data-stu-id="54bd2-213">Specify whether the wifi connection should connect automatically even when the SSID is not broadcasting.</span></span> <span data-ttu-id="54bd2-214">Herdado do [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-214">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-215">proxySetting</span><span class="sxs-lookup"><span data-stu-id="54bd2-215">proxySetting</span></span>|[<span data-ttu-id="54bd2-216">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="54bd2-216">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="54bd2-217">Especifique a configuração de proxy Wi-Fi herdada do [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54bd2-217">Specify the proxy setting for Wi-Fi configuration Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).</span></span> <span data-ttu-id="54bd2-218">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="54bd2-218">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="54bd2-219">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="54bd2-219">proxyManualAddress</span></span>|<span data-ttu-id="54bd2-220">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54bd2-220">String</span></span>|<span data-ttu-id="54bd2-221">Especifique o endereço IP do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="54bd2-221">Specify the IP address for the proxy server.</span></span> <span data-ttu-id="54bd2-222">Herdado do [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-222">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-223">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="54bd2-223">proxyManualPort</span></span>|<span data-ttu-id="54bd2-224">Int32</span><span class="sxs-lookup"><span data-stu-id="54bd2-224">Int32</span></span>|<span data-ttu-id="54bd2-225">Especifique a porta para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="54bd2-225">Specify the port for the proxy server.</span></span> <span data-ttu-id="54bd2-226">Herdado do [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-226">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-227">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="54bd2-227">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="54bd2-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54bd2-228">String</span></span>|<span data-ttu-id="54bd2-229">Especifique a URL do script de configuração do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="54bd2-229">Specify the URL for the proxy server configuration script.</span></span> <span data-ttu-id="54bd2-230">Herdado do [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-230">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-231">forceFIPSCompliance</span><span class="sxs-lookup"><span data-stu-id="54bd2-231">forceFIPSCompliance</span></span>|<span data-ttu-id="54bd2-232">Booleano</span><span class="sxs-lookup"><span data-stu-id="54bd2-232">Boolean</span></span>|<span data-ttu-id="54bd2-233">Especifique se deve forçar a conformidade fips.</span><span class="sxs-lookup"><span data-stu-id="54bd2-233">Specify whether to force FIPS compliance.</span></span> <span data-ttu-id="54bd2-234">Herdado do [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54bd2-234">Inherited from [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)</span></span>|
|<span data-ttu-id="54bd2-235">networkSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="54bd2-235">networkSingleSignOn</span></span>|[<span data-ttu-id="54bd2-236">networkSingleSignOnType</span><span class="sxs-lookup"><span data-stu-id="54bd2-236">networkSingleSignOnType</span></span>](../resources/intune-deviceconfig-networksinglesignontype.md)|<span data-ttu-id="54bd2-237">Especifique o tipo de sinal único de rede.</span><span class="sxs-lookup"><span data-stu-id="54bd2-237">Specify the network single sign on type.</span></span> <span data-ttu-id="54bd2-238">Os valores possíveis são: `disabled`, `prelogon`, `postlogon`.</span><span class="sxs-lookup"><span data-stu-id="54bd2-238">Possible values are: `disabled`, `prelogon`, `postlogon`.</span></span>|
|<span data-ttu-id="54bd2-239">maximumAuthenticationTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="54bd2-239">maximumAuthenticationTimeoutInSeconds</span></span>|<span data-ttu-id="54bd2-240">Int32</span><span class="sxs-lookup"><span data-stu-id="54bd2-240">Int32</span></span>|<span data-ttu-id="54bd2-241">Especifique o tempo limite máximo de autenticação (em segundos).</span><span class="sxs-lookup"><span data-stu-id="54bd2-241">Specify maximum authentication timeout (in seconds).</span></span>  <span data-ttu-id="54bd2-242">Intervalo válido: 1-120</span><span class="sxs-lookup"><span data-stu-id="54bd2-242">Valid range: 1-120</span></span>|
|<span data-ttu-id="54bd2-243">userBasedVirtualLan</span><span class="sxs-lookup"><span data-stu-id="54bd2-243">userBasedVirtualLan</span></span>|<span data-ttu-id="54bd2-244">Booleano</span><span class="sxs-lookup"><span data-stu-id="54bd2-244">Boolean</span></span>|<span data-ttu-id="54bd2-245">Especifica se é preciso alterar a LAN virtual usada pelo dispositivo com base nas credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="54bd2-245">Specifiy whether to change the virtual LAN used by the device based on the user’s credentials.</span></span> <span data-ttu-id="54bd2-246">Não é possível usar quando NetworkSingleSignOnType está definido como Desabilitado.</span><span class="sxs-lookup"><span data-stu-id="54bd2-246">Cannot be used when NetworkSingleSignOnType is set to Disabled.</span></span>|
|<span data-ttu-id="54bd2-247">promptForAdditionalAuthenticationCredentials</span><span class="sxs-lookup"><span data-stu-id="54bd2-247">promptForAdditionalAuthenticationCredentials</span></span>|<span data-ttu-id="54bd2-248">Booleano</span><span class="sxs-lookup"><span data-stu-id="54bd2-248">Boolean</span></span>|<span data-ttu-id="54bd2-249">Especifique se a conexão wifi deve solicitar credenciais de autenticação adicionais.</span><span class="sxs-lookup"><span data-stu-id="54bd2-249">Specify whether the wifi connection should prompt for additional authentication credentials.</span></span>|
|<span data-ttu-id="54bd2-250">enablePairwiseMasterKeyCaching</span><span class="sxs-lookup"><span data-stu-id="54bd2-250">enablePairwiseMasterKeyCaching</span></span>|<span data-ttu-id="54bd2-251">Booleano</span><span class="sxs-lookup"><span data-stu-id="54bd2-251">Boolean</span></span>|<span data-ttu-id="54bd2-252">Especifique se a conexão wifi deve habilitar o cache de chave mestra par.</span><span class="sxs-lookup"><span data-stu-id="54bd2-252">Specify whether the wifi connection should enable pairwise master key caching.</span></span>|
|<span data-ttu-id="54bd2-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="54bd2-253">maximumPairwiseMasterKeyCacheTimeInMinutes</span></span>|<span data-ttu-id="54bd2-254">Int32</span><span class="sxs-lookup"><span data-stu-id="54bd2-254">Int32</span></span>|<span data-ttu-id="54bd2-255">Especifique o tempo máximo de cache da chave mestra par (em minutos).</span><span class="sxs-lookup"><span data-stu-id="54bd2-255">Specify maximum pairwise master key cache time (in minutes).</span></span>  <span data-ttu-id="54bd2-256">Intervalo válido: 5-1440</span><span class="sxs-lookup"><span data-stu-id="54bd2-256">Valid range: 5-1440</span></span>|
|<span data-ttu-id="54bd2-257">maximumNumberOfPairwiseMasterKeysInCache</span><span class="sxs-lookup"><span data-stu-id="54bd2-257">maximumNumberOfPairwiseMasterKeysInCache</span></span>|<span data-ttu-id="54bd2-258">Int32</span><span class="sxs-lookup"><span data-stu-id="54bd2-258">Int32</span></span>|<span data-ttu-id="54bd2-259">Especifique o número máximo de chaves mestras de par no cache.</span><span class="sxs-lookup"><span data-stu-id="54bd2-259">Specify maximum number of pairwise master keys in cache.</span></span>  <span data-ttu-id="54bd2-260">Intervalo válido: 1-255</span><span class="sxs-lookup"><span data-stu-id="54bd2-260">Valid range: 1-255</span></span>|
|<span data-ttu-id="54bd2-261">enablePreAuthentication</span><span class="sxs-lookup"><span data-stu-id="54bd2-261">enablePreAuthentication</span></span>|<span data-ttu-id="54bd2-262">Booleano</span><span class="sxs-lookup"><span data-stu-id="54bd2-262">Boolean</span></span>|<span data-ttu-id="54bd2-263">Especifique se a pré-autenticação deve ser habilitada.</span><span class="sxs-lookup"><span data-stu-id="54bd2-263">Specify whether pre-authentication should be enabled.</span></span>|
|<span data-ttu-id="54bd2-264">maximumPreAuthenticationAttempts</span><span class="sxs-lookup"><span data-stu-id="54bd2-264">maximumPreAuthenticationAttempts</span></span>|<span data-ttu-id="54bd2-265">Int32</span><span class="sxs-lookup"><span data-stu-id="54bd2-265">Int32</span></span>|<span data-ttu-id="54bd2-266">Especifique as tentativas máximas de pré-autenticação.</span><span class="sxs-lookup"><span data-stu-id="54bd2-266">Specify maximum pre-authentication attempts.</span></span>  <span data-ttu-id="54bd2-267">Intervalo válido: 1-16</span><span class="sxs-lookup"><span data-stu-id="54bd2-267">Valid range: 1-16</span></span>|
|<span data-ttu-id="54bd2-268">eapType</span><span class="sxs-lookup"><span data-stu-id="54bd2-268">eapType</span></span>|[<span data-ttu-id="54bd2-269">eapType</span><span class="sxs-lookup"><span data-stu-id="54bd2-269">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="54bd2-270">Protocolo de Autenticação Extensível (EAP).</span><span class="sxs-lookup"><span data-stu-id="54bd2-270">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="54bd2-271">Indica o tipo de conjunto de protocolo EAP no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="54bd2-271">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="54bd2-272">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="54bd2-272">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="54bd2-273">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="54bd2-273">trustedServerCertificateNames</span></span>|<span data-ttu-id="54bd2-274">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="54bd2-274">String collection</span></span>|<span data-ttu-id="54bd2-275">Especifique nomes de certificados de servidor confiáveis.</span><span class="sxs-lookup"><span data-stu-id="54bd2-275">Specify trusted server certificate names.</span></span>|
|<span data-ttu-id="54bd2-276">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="54bd2-276">authenticationMethod</span></span>|[<span data-ttu-id="54bd2-277">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="54bd2-277">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="54bd2-278">Especifique o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="54bd2-278">Specify the authentication method.</span></span> <span data-ttu-id="54bd2-279">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="54bd2-279">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="54bd2-280">innerAuthenticationProtocolForEAPTTLS</span><span class="sxs-lookup"><span data-stu-id="54bd2-280">innerAuthenticationProtocolForEAPTTLS</span></span>|[<span data-ttu-id="54bd2-281">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="54bd2-281">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="54bd2-282">Especifique o protocolo de autenticação interna para TTLS EAP.</span><span class="sxs-lookup"><span data-stu-id="54bd2-282">Specify inner authentication protocol for EAP TTLS.</span></span> <span data-ttu-id="54bd2-283">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="54bd2-283">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="54bd2-284">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="54bd2-284">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="54bd2-285">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54bd2-285">String</span></span>|<span data-ttu-id="54bd2-286">Especifique a cadeia de caracteres para substituir nomes de usuário para privacidade ao usar TTLS EAP ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="54bd2-286">Specify the string to replace usernames for privacy when using EAP TTLS or PEAP.</span></span>|
|<span data-ttu-id="54bd2-287">requireCryptographicBinding</span><span class="sxs-lookup"><span data-stu-id="54bd2-287">requireCryptographicBinding</span></span>|<span data-ttu-id="54bd2-288">Booleano</span><span class="sxs-lookup"><span data-stu-id="54bd2-288">Boolean</span></span>|<span data-ttu-id="54bd2-289">Especifique se deve habilitar a associação criptográfica quando o tipo EAP estiver selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="54bd2-289">Specify whether to enable cryptographic binding when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="54bd2-290">performServerValidation</span><span class="sxs-lookup"><span data-stu-id="54bd2-290">performServerValidation</span></span>|<span data-ttu-id="54bd2-291">Booleano</span><span class="sxs-lookup"><span data-stu-id="54bd2-291">Boolean</span></span>|<span data-ttu-id="54bd2-292">Especifique se deve habilitar a verificação da identidade do servidor validando o certificado quando o tipo EAP for selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="54bd2-292">Specify whether to enable verification of server's identity by validating the certificate when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="54bd2-293">disableUserPromptForServerValidation</span><span class="sxs-lookup"><span data-stu-id="54bd2-293">disableUserPromptForServerValidation</span></span>|<span data-ttu-id="54bd2-294">Booleano</span><span class="sxs-lookup"><span data-stu-id="54bd2-294">Boolean</span></span>|<span data-ttu-id="54bd2-295">Especifique se o usuário deve ser solicitado a autorizar novos servidores para autoridades de certificação confiáveis quando o tipo EAP for selecionado como PEAP.</span><span class="sxs-lookup"><span data-stu-id="54bd2-295">Specify whether to prevent the user from being prompted to authorize new servers for trusted certification authorities when EAP type is selected as PEAP.</span></span>|
|<span data-ttu-id="54bd2-296">authenticationPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="54bd2-296">authenticationPeriodInSeconds</span></span>|<span data-ttu-id="54bd2-297">Int32</span><span class="sxs-lookup"><span data-stu-id="54bd2-297">Int32</span></span>|<span data-ttu-id="54bd2-298">Especifique o número de segundos para o cliente aguardar após uma tentativa de autenticação antes de falhar.</span><span class="sxs-lookup"><span data-stu-id="54bd2-298">Specify the number of seconds for the client to wait after an authentication attempt before failing.</span></span> <span data-ttu-id="54bd2-299">Intervalo válido 1-3600.</span><span class="sxs-lookup"><span data-stu-id="54bd2-299">Valid range 1-3600.</span></span>|
|<span data-ttu-id="54bd2-300">authenticationRetryDelayPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="54bd2-300">authenticationRetryDelayPeriodInSeconds</span></span>|<span data-ttu-id="54bd2-301">Int32</span><span class="sxs-lookup"><span data-stu-id="54bd2-301">Int32</span></span>|<span data-ttu-id="54bd2-302">Especifique o número de segundos entre uma autenticação com falha e a próxima tentativa de autenticação.</span><span class="sxs-lookup"><span data-stu-id="54bd2-302">Specify the number of seconds between a failed authentication and the next authentication attempt.</span></span> <span data-ttu-id="54bd2-303">Intervalo válido 1-3600.</span><span class="sxs-lookup"><span data-stu-id="54bd2-303">Valid range 1-3600.</span></span>|
|<span data-ttu-id="54bd2-304">eapolStartPeriodInSeconds</span><span class="sxs-lookup"><span data-stu-id="54bd2-304">eapolStartPeriodInSeconds</span></span>|<span data-ttu-id="54bd2-305">Int32</span><span class="sxs-lookup"><span data-stu-id="54bd2-305">Int32</span></span>|<span data-ttu-id="54bd2-306">Especifique o número de segundos a ser aguardado antes de enviar uma mensagem inicial EAPOL (Extensible Authentication Protocol over LAN).</span><span class="sxs-lookup"><span data-stu-id="54bd2-306">Specify the number of seconds to wait before sending an EAPOL (Extensible Authentication Protocol over LAN) Start message.</span></span> <span data-ttu-id="54bd2-307">Intervalo válido 1-3600.</span><span class="sxs-lookup"><span data-stu-id="54bd2-307">Valid range 1-3600.</span></span>|
|<span data-ttu-id="54bd2-308">maximumEAPOLStartMessages</span><span class="sxs-lookup"><span data-stu-id="54bd2-308">maximumEAPOLStartMessages</span></span>|<span data-ttu-id="54bd2-309">Int32</span><span class="sxs-lookup"><span data-stu-id="54bd2-309">Int32</span></span>|<span data-ttu-id="54bd2-310">Especifica o número máximo de mensagens EAPOL (Extensible Authentication Protocol over LAN) a serem enviadas antes de retornar a falha.</span><span class="sxs-lookup"><span data-stu-id="54bd2-310">Specifiy the maximum number of EAPOL (Extensible Authentication Protocol over LAN) Start messages to be sent before returning failure.</span></span> <span data-ttu-id="54bd2-311">Intervalo válido de 1 a 100.</span><span class="sxs-lookup"><span data-stu-id="54bd2-311">Valid range 1-100.</span></span>|
|<span data-ttu-id="54bd2-312">maximumAuthenticationFailures</span><span class="sxs-lookup"><span data-stu-id="54bd2-312">maximumAuthenticationFailures</span></span>|<span data-ttu-id="54bd2-313">Int32</span><span class="sxs-lookup"><span data-stu-id="54bd2-313">Int32</span></span>|<span data-ttu-id="54bd2-314">Especifique as falhas máximas de autenticação permitidas para um conjunto de credenciais.</span><span class="sxs-lookup"><span data-stu-id="54bd2-314">Specify the maximum authentication failures allowed for a set of credentials.</span></span> <span data-ttu-id="54bd2-315">Intervalo válido de 1 a 100.</span><span class="sxs-lookup"><span data-stu-id="54bd2-315">Valid range 1-100.</span></span>|
|<span data-ttu-id="54bd2-316">cacheCredentials</span><span class="sxs-lookup"><span data-stu-id="54bd2-316">cacheCredentials</span></span>|<span data-ttu-id="54bd2-317">Booleano</span><span class="sxs-lookup"><span data-stu-id="54bd2-317">Boolean</span></span>|<span data-ttu-id="54bd2-318">Especifique se deve armazenar em cache as credenciais do usuário no dispositivo para que os usuários não precisem continuar inserindo-as sempre que se conectarem.</span><span class="sxs-lookup"><span data-stu-id="54bd2-318">Specify whether to cache user credentials on the device so that users don’t need to keep entering them each time they connect.</span></span>|
|<span data-ttu-id="54bd2-319">authenticationType</span><span class="sxs-lookup"><span data-stu-id="54bd2-319">authenticationType</span></span>|[<span data-ttu-id="54bd2-320">wifiAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="54bd2-320">wifiAuthenticationType</span></span>](../resources/intune-deviceconfig-wifiauthenticationtype.md)|<span data-ttu-id="54bd2-321">Especifique se o usuário, o dispositivo ou o dispositivo devem ser autenticados (nenhum).</span><span class="sxs-lookup"><span data-stu-id="54bd2-321">Specify whether to authenticate the user, the device, either, or to use guest authentication (none).</span></span> <span data-ttu-id="54bd2-322">Se você estiver usando autenticação de certificado, certifique-se de que o tipo de certificado corresponde ao tipo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="54bd2-322">If you’re using certificate authentication, make sure the certificate type matches the authentication type.</span></span> <span data-ttu-id="54bd2-323">Os valores possíveis são: `none`, `user`, `machine`, `machineOrUser`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="54bd2-323">Possible values are: `none`, `user`, `machine`, `machineOrUser`, `guest`.</span></span>|



## <a name="response"></a><span data-ttu-id="54bd2-324">Resposta</span><span class="sxs-lookup"><span data-stu-id="54bd2-324">Response</span></span>
<span data-ttu-id="54bd2-325">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54bd2-325">If successful, this method returns a `201 Created` response code and a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54bd2-326">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54bd2-326">Example</span></span>

### <a name="request"></a><span data-ttu-id="54bd2-327">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54bd2-327">Request</span></span>
<span data-ttu-id="54bd2-328">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54bd2-328">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="54bd2-329">Resposta</span><span class="sxs-lookup"><span data-stu-id="54bd2-329">Response</span></span>
<span data-ttu-id="54bd2-p141">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54bd2-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




