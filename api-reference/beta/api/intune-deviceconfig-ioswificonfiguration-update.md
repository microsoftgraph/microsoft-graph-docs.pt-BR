---
title: Atualizar iosWiFiConfiguration
description: Atualiza as propriedades de um objeto iosWiFiConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f5bb52fbc754a2e46703fee08bccb2b87b62d81
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42747977"
---
# <a name="update-ioswificonfiguration"></a><span data-ttu-id="e1ff7-103">Atualizar iosWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1ff7-103">Update iosWiFiConfiguration</span></span>

> <span data-ttu-id="e1ff7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1ff7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1ff7-106">Atualiza as propriedades de um objeto [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e1ff7-106">Update the properties of a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1ff7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1ff7-107">Prerequisites</span></span>
<span data-ttu-id="e1ff7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1ff7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1ff7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1ff7-110">Permission type</span></span>|<span data-ttu-id="e1ff7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1ff7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1ff7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1ff7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1ff7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1ff7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1ff7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1ff7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1ff7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-115">Not supported.</span></span>|
|<span data-ttu-id="e1ff7-116">Application</span><span class="sxs-lookup"><span data-stu-id="e1ff7-116">Application</span></span>|<span data-ttu-id="e1ff7-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1ff7-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1ff7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1ff7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e1ff7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1ff7-119">Request headers</span></span>
|<span data-ttu-id="e1ff7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1ff7-120">Header</span></span>|<span data-ttu-id="e1ff7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e1ff7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1ff7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1ff7-122">Authorization</span></span>|<span data-ttu-id="e1ff7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1ff7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1ff7-124">Accept</span></span>|<span data-ttu-id="e1ff7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e1ff7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1ff7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1ff7-126">Request body</span></span>
<span data-ttu-id="e1ff7-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e1ff7-127">In the request body, supply a JSON representation for the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

<span data-ttu-id="e1ff7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e1ff7-128">The following table shows the properties that are required when you create the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span>

|<span data-ttu-id="e1ff7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1ff7-129">Property</span></span>|<span data-ttu-id="e1ff7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1ff7-130">Type</span></span>|<span data-ttu-id="e1ff7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1ff7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1ff7-132">id</span><span class="sxs-lookup"><span data-stu-id="e1ff7-132">id</span></span>|<span data-ttu-id="e1ff7-133">String</span><span class="sxs-lookup"><span data-stu-id="e1ff7-133">String</span></span>|<span data-ttu-id="e1ff7-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-134">Key of the entity.</span></span> <span data-ttu-id="e1ff7-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ff7-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ff7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1ff7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e1ff7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1ff7-137">DateTimeOffset</span></span>|<span data-ttu-id="e1ff7-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e1ff7-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ff7-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ff7-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e1ff7-140">roleScopeTagIds</span></span>|<span data-ttu-id="e1ff7-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1ff7-141">String collection</span></span>|<span data-ttu-id="e1ff7-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e1ff7-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ff7-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ff7-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e1ff7-144">supportsScopeTags</span></span>|<span data-ttu-id="e1ff7-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ff7-145">Boolean</span></span>|<span data-ttu-id="e1ff7-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e1ff7-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e1ff7-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e1ff7-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-149">This property is read-only.</span></span> <span data-ttu-id="e1ff7-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ff7-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ff7-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e1ff7-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e1ff7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e1ff7-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e1ff7-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e1ff7-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ff7-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ff7-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e1ff7-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e1ff7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e1ff7-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e1ff7-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e1ff7-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ff7-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ff7-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e1ff7-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e1ff7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e1ff7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e1ff7-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e1ff7-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ff7-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ff7-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1ff7-163">createdDateTime</span></span>|<span data-ttu-id="e1ff7-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1ff7-164">DateTimeOffset</span></span>|<span data-ttu-id="e1ff7-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-165">DateTime the object was created.</span></span> <span data-ttu-id="e1ff7-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ff7-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ff7-167">description</span><span class="sxs-lookup"><span data-stu-id="e1ff7-167">description</span></span>|<span data-ttu-id="e1ff7-168">String</span><span class="sxs-lookup"><span data-stu-id="e1ff7-168">String</span></span>|<span data-ttu-id="e1ff7-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e1ff7-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ff7-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ff7-171">displayName</span><span class="sxs-lookup"><span data-stu-id="e1ff7-171">displayName</span></span>|<span data-ttu-id="e1ff7-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1ff7-172">String</span></span>|<span data-ttu-id="e1ff7-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e1ff7-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ff7-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ff7-175">versão</span><span class="sxs-lookup"><span data-stu-id="e1ff7-175">version</span></span>|<span data-ttu-id="e1ff7-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ff7-176">Int32</span></span>|<span data-ttu-id="e1ff7-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-177">Version of the device configuration.</span></span> <span data-ttu-id="e1ff7-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1ff7-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1ff7-179">NetworkName</span><span class="sxs-lookup"><span data-stu-id="e1ff7-179">networkName</span></span>|<span data-ttu-id="e1ff7-180">String</span><span class="sxs-lookup"><span data-stu-id="e1ff7-180">String</span></span>|<span data-ttu-id="e1ff7-181">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="e1ff7-181">Network Name</span></span>|
|<span data-ttu-id="e1ff7-182">SSID</span><span class="sxs-lookup"><span data-stu-id="e1ff7-182">ssid</span></span>|<span data-ttu-id="e1ff7-183">String</span><span class="sxs-lookup"><span data-stu-id="e1ff7-183">String</span></span>|<span data-ttu-id="e1ff7-184">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="e1ff7-185">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="e1ff7-185">connectAutomatically</span></span>|<span data-ttu-id="e1ff7-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ff7-186">Boolean</span></span>|<span data-ttu-id="e1ff7-187">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-187">Connect automatically when this network is in range.</span></span> <span data-ttu-id="e1ff7-188">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-188">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="e1ff7-189">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="e1ff7-189">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="e1ff7-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1ff7-190">Boolean</span></span>|<span data-ttu-id="e1ff7-191">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="e1ff7-191">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="e1ff7-192">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="e1ff7-193">à</span><span class="sxs-lookup"><span data-stu-id="e1ff7-193">wiFiSecurityType</span></span>|[<span data-ttu-id="e1ff7-194">à</span><span class="sxs-lookup"><span data-stu-id="e1ff7-194">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="e1ff7-195">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="e1ff7-196">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-196">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="e1ff7-197">proxySettings</span><span class="sxs-lookup"><span data-stu-id="e1ff7-197">proxySettings</span></span>|[<span data-ttu-id="e1ff7-198">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="e1ff7-198">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="e1ff7-199">Tipo de proxy para esta conexão Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-199">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="e1ff7-200">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-200">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="e1ff7-201">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="e1ff7-201">proxyManualAddress</span></span>|<span data-ttu-id="e1ff7-202">String</span><span class="sxs-lookup"><span data-stu-id="e1ff7-202">String</span></span>|<span data-ttu-id="e1ff7-203">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-203">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="e1ff7-204">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="e1ff7-204">proxyManualPort</span></span>|<span data-ttu-id="e1ff7-205">Int32</span><span class="sxs-lookup"><span data-stu-id="e1ff7-205">Int32</span></span>|<span data-ttu-id="e1ff7-206">Porta do servidor proxy quando a configuração manual estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-206">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="e1ff7-207">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="e1ff7-207">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="e1ff7-208">String</span><span class="sxs-lookup"><span data-stu-id="e1ff7-208">String</span></span>|<span data-ttu-id="e1ff7-209">URL do script de configuração automática do servidor proxy quando a configuração automática estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-209">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="e1ff7-210">Essa URL normalmente é o local do Arquivo PAC (configuração automática de proxy).</span><span class="sxs-lookup"><span data-stu-id="e1ff7-210">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="e1ff7-211">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="e1ff7-211">preSharedKey</span></span>|<span data-ttu-id="e1ff7-212">String</span><span class="sxs-lookup"><span data-stu-id="e1ff7-212">String</span></span>|<span data-ttu-id="e1ff7-213">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-213">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="e1ff7-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1ff7-214">Response</span></span>
<span data-ttu-id="e1ff7-215">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-215">If successful, this method returns a `200 OK` response code and an updated [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1ff7-216">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1ff7-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1ff7-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1ff7-217">Request</span></span>
<span data-ttu-id="e1ff7-218">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-218">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1448

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
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
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="e1ff7-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1ff7-219">Response</span></span>
<span data-ttu-id="e1ff7-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1ff7-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1620

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
  "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
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
  "preSharedKey": "Pre Shared Key value"
}
```




