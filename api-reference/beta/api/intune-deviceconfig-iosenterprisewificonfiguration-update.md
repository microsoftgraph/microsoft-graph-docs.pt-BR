---
title: Atualizar iosEnterpriseWiFiConfiguration
description: Atualize as propriedades de um objeto iosEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 76022c7bf57a719c46d36afecf0989696574615e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131565"
---
# <a name="update-iosenterprisewificonfiguration"></a><span data-ttu-id="ff76e-103">Atualizar iosEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff76e-103">Update iosEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="ff76e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff76e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff76e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff76e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff76e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff76e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff76e-107">Atualize as propriedades de [um objeto iosEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-107">Update the properties of a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff76e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff76e-108">Prerequisites</span></span>
<span data-ttu-id="ff76e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff76e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff76e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff76e-111">Permission type</span></span>|<span data-ttu-id="ff76e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff76e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff76e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff76e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff76e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff76e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ff76e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff76e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff76e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff76e-116">Not supported.</span></span>|
|<span data-ttu-id="ff76e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff76e-117">Application</span></span>|<span data-ttu-id="ff76e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff76e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff76e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff76e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ff76e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff76e-120">Request headers</span></span>
|<span data-ttu-id="ff76e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff76e-121">Header</span></span>|<span data-ttu-id="ff76e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ff76e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff76e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff76e-123">Authorization</span></span>|<span data-ttu-id="ff76e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff76e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff76e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff76e-125">Accept</span></span>|<span data-ttu-id="ff76e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff76e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff76e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff76e-127">Request body</span></span>
<span data-ttu-id="ff76e-128">No corpo da solicitação, fornece uma representação JSON para o [objeto iosEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-128">In the request body, supply a JSON representation for the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="ff76e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ff76e-129">The following table shows the properties that are required when you create the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="ff76e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff76e-130">Property</span></span>|<span data-ttu-id="ff76e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff76e-131">Type</span></span>|<span data-ttu-id="ff76e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff76e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff76e-133">id</span><span class="sxs-lookup"><span data-stu-id="ff76e-133">id</span></span>|<span data-ttu-id="ff76e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff76e-134">String</span></span>|<span data-ttu-id="ff76e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ff76e-135">Key of the entity.</span></span> <span data-ttu-id="ff76e-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff76e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ff76e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff76e-138">DateTimeOffset</span></span>|<span data-ttu-id="ff76e-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ff76e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ff76e-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ff76e-141">roleScopeTagIds</span></span>|<span data-ttu-id="ff76e-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff76e-142">String collection</span></span>|<span data-ttu-id="ff76e-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="ff76e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ff76e-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ff76e-145">supportsScopeTags</span></span>|<span data-ttu-id="ff76e-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="ff76e-146">Boolean</span></span>|<span data-ttu-id="ff76e-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ff76e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ff76e-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ff76e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ff76e-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ff76e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ff76e-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff76e-150">This property is read-only.</span></span> <span data-ttu-id="ff76e-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ff76e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ff76e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ff76e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ff76e-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ff76e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ff76e-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ff76e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ff76e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ff76e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ff76e-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ff76e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ff76e-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ff76e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ff76e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ff76e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ff76e-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ff76e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ff76e-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff76e-164">createdDateTime</span></span>|<span data-ttu-id="ff76e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff76e-165">DateTimeOffset</span></span>|<span data-ttu-id="ff76e-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ff76e-166">DateTime the object was created.</span></span> <span data-ttu-id="ff76e-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-168">descrição</span><span class="sxs-lookup"><span data-stu-id="ff76e-168">description</span></span>|<span data-ttu-id="ff76e-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff76e-169">String</span></span>|<span data-ttu-id="ff76e-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff76e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ff76e-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ff76e-172">displayName</span></span>|<span data-ttu-id="ff76e-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff76e-173">String</span></span>|<span data-ttu-id="ff76e-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff76e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ff76e-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-176">versão</span><span class="sxs-lookup"><span data-stu-id="ff76e-176">version</span></span>|<span data-ttu-id="ff76e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ff76e-177">Int32</span></span>|<span data-ttu-id="ff76e-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ff76e-178">Version of the device configuration.</span></span> <span data-ttu-id="ff76e-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-180">networkName</span><span class="sxs-lookup"><span data-stu-id="ff76e-180">networkName</span></span>|<span data-ttu-id="ff76e-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff76e-181">String</span></span>|<span data-ttu-id="ff76e-182">Nome da rede Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-182">Network Name Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-183">ssid</span><span class="sxs-lookup"><span data-stu-id="ff76e-183">ssid</span></span>|<span data-ttu-id="ff76e-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff76e-184">String</span></span>|<span data-ttu-id="ff76e-185">Esse é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ff76e-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="ff76e-186">Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-186">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="ff76e-187">connectAutomatically</span></span>|<span data-ttu-id="ff76e-188">Booleano</span><span class="sxs-lookup"><span data-stu-id="ff76e-188">Boolean</span></span>|<span data-ttu-id="ff76e-189">Conecte-se automaticamente quando essa rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="ff76e-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="ff76e-190">Definir isso como true ignorará o prompt do usuário e conectará automaticamente o dispositivo Wi-Fi rede.</span><span class="sxs-lookup"><span data-stu-id="ff76e-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="ff76e-191">Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-191">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="ff76e-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="ff76e-193">Booleano</span><span class="sxs-lookup"><span data-stu-id="ff76e-193">Boolean</span></span>|<span data-ttu-id="ff76e-194">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="ff76e-194">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="ff76e-195">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ff76e-195">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="ff76e-196">Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-196">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-197">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="ff76e-197">wiFiSecurityType</span></span>|[<span data-ttu-id="ff76e-198">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="ff76e-198">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="ff76e-199">Indica se Wi-Fi ponto de extremidade usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="ff76e-199">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="ff76e-200">Herdado [de iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ff76e-200">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="ff76e-201">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="ff76e-201">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="ff76e-202">proxySettings</span><span class="sxs-lookup"><span data-stu-id="ff76e-202">proxySettings</span></span>|[<span data-ttu-id="ff76e-203">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="ff76e-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="ff76e-204">Tipo de proxy para essa Wi-Fi herdada de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ff76e-204">Proxy Type for this Wi-Fi connection Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="ff76e-205">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="ff76e-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="ff76e-206">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="ff76e-206">proxyManualAddress</span></span>|<span data-ttu-id="ff76e-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff76e-207">String</span></span>|<span data-ttu-id="ff76e-208">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual é selecionada.</span><span class="sxs-lookup"><span data-stu-id="ff76e-208">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="ff76e-209">Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-209">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-210">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="ff76e-210">proxyManualPort</span></span>|<span data-ttu-id="ff76e-211">Int32</span><span class="sxs-lookup"><span data-stu-id="ff76e-211">Int32</span></span>|<span data-ttu-id="ff76e-212">Porta do servidor proxy quando a configuração manual é selecionada.</span><span class="sxs-lookup"><span data-stu-id="ff76e-212">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="ff76e-213">Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-213">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-214">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="ff76e-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="ff76e-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff76e-215">String</span></span>|<span data-ttu-id="ff76e-216">URL do script de configuração automática do servidor proxy quando a configuração automática é selecionada.</span><span class="sxs-lookup"><span data-stu-id="ff76e-216">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="ff76e-217">Normalmente, essa URL é o local do arquivo PAC (Configuração Automática de Proxy).</span><span class="sxs-lookup"><span data-stu-id="ff76e-217">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="ff76e-218">Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-218">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-219">disableMacAddressRandomization</span><span class="sxs-lookup"><span data-stu-id="ff76e-219">disableMacAddressRandomization</span></span>|<span data-ttu-id="ff76e-220">Booleano</span><span class="sxs-lookup"><span data-stu-id="ff76e-220">Boolean</span></span>|<span data-ttu-id="ff76e-221">Se definido como true, força os dispositivos que se conectam usando esse perfil de Wi-Fi para apresentar seu endereço MAC real Wi-Fi em vez de um endereço MAC aleatório.</span><span class="sxs-lookup"><span data-stu-id="ff76e-221">If set to true, forces devices connecting using this Wi-Fi profile to present their actual Wi-Fi MAC address instead of a random MAC address.</span></span> <span data-ttu-id="ff76e-222">Aplica-se ao iOS 14 e posterior.</span><span class="sxs-lookup"><span data-stu-id="ff76e-222">Applies to iOS 14 and later.</span></span> <span data-ttu-id="ff76e-223">Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-223">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-224">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="ff76e-224">preSharedKey</span></span>|<span data-ttu-id="ff76e-225">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff76e-225">String</span></span>|<span data-ttu-id="ff76e-226">Esta é a chave pré-compartilhada para a rede WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="ff76e-226">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="ff76e-227">Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ff76e-227">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="ff76e-228">eapType</span><span class="sxs-lookup"><span data-stu-id="ff76e-228">eapType</span></span>|[<span data-ttu-id="ff76e-229">eapType</span><span class="sxs-lookup"><span data-stu-id="ff76e-229">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="ff76e-230">Protocolo de Autenticação Extensível (EAP).</span><span class="sxs-lookup"><span data-stu-id="ff76e-230">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="ff76e-231">Indica o tipo de conjunto de protocolo EAP no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="ff76e-231">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="ff76e-232">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="ff76e-232">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="ff76e-233">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff76e-233">eapFastConfiguration</span></span>|[<span data-ttu-id="ff76e-234">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="ff76e-234">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="ff76e-235">Opção de Configuração EAP-FAST quando EAP-FAST é o Tipo EAP selecionado.</span><span class="sxs-lookup"><span data-stu-id="ff76e-235">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="ff76e-236">Os valores possíveis são: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="ff76e-236">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="ff76e-237">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="ff76e-237">trustedServerCertificateNames</span></span>|<span data-ttu-id="ff76e-238">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff76e-238">String collection</span></span>|<span data-ttu-id="ff76e-239">Nomes de certificados de servidor confiáveis quando Tipo de EAP é configurado para EAP-TLS/TTLS/FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="ff76e-239">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="ff76e-240">Esse é o nome comum usado nos certificados emitidos pela autoridade de certificação confiável (CA).</span><span class="sxs-lookup"><span data-stu-id="ff76e-240">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="ff76e-241">Se você fornecer essas informações, poderá ignorar a caixa de diálogo de confiança dinâmica exibida nos dispositivos dos usuários finais quando eles se conectarem Wi-Fi rede.</span><span class="sxs-lookup"><span data-stu-id="ff76e-241">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users' devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="ff76e-242">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ff76e-242">authenticationMethod</span></span>|[<span data-ttu-id="ff76e-243">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ff76e-243">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="ff76e-244">Método de autenticação quando Tipo de EAP é configurado para PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="ff76e-244">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="ff76e-245">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="ff76e-245">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="ff76e-246">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="ff76e-246">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="ff76e-247">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="ff76e-247">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="ff76e-248">Método não EAP para autenticação quando Tipo EAP é EAP-TTLS e Authenticationmethod é Nome de Usuário e Senha.</span><span class="sxs-lookup"><span data-stu-id="ff76e-248">Non-EAP Method for Authentication when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="ff76e-249">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="ff76e-249">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="ff76e-250">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="ff76e-250">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="ff76e-251">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff76e-251">String</span></span>|<span data-ttu-id="ff76e-252">Habilita a privacidade de identidade (Identidade Externa) quando o Tipo EAP estiver configurado como EAP - TTLS, EAP - FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="ff76e-252">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP - TTLS, EAP - FAST or PEAP.</span></span> <span data-ttu-id="ff76e-253">Essa propriedade mascara os nomes de usuário com o texto que você inserir.</span><span class="sxs-lookup"><span data-stu-id="ff76e-253">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="ff76e-254">Por exemplo, se você usar 'anônimo', cada usuário que se autenticar com essa conexão Wi-Fi usando seu nome de usuário real será exibido como "anônimo".</span><span class="sxs-lookup"><span data-stu-id="ff76e-254">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|
|<span data-ttu-id="ff76e-255">usernameFormatString</span><span class="sxs-lookup"><span data-stu-id="ff76e-255">usernameFormatString</span></span>|<span data-ttu-id="ff76e-256">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff76e-256">String</span></span>|<span data-ttu-id="ff76e-257">Cadeia de caracteres de formato de nome de usuário usada para criar o nome de usuário para se conectar ao wifi</span><span class="sxs-lookup"><span data-stu-id="ff76e-257">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="ff76e-258">passwordFormatString</span><span class="sxs-lookup"><span data-stu-id="ff76e-258">passwordFormatString</span></span>|<span data-ttu-id="ff76e-259">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff76e-259">String</span></span>|<span data-ttu-id="ff76e-260">Cadeia de caracteres de formato de senha usada para criar a senha para se conectar ao wifi</span><span class="sxs-lookup"><span data-stu-id="ff76e-260">Password format string used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="ff76e-261">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff76e-261">Response</span></span>
<span data-ttu-id="ff76e-262">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff76e-262">If successful, this method returns a `200 OK` response code and an updated [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff76e-263">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff76e-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff76e-264">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff76e-264">Request</span></span>
<span data-ttu-id="ff76e-265">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff76e-265">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2017

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
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
  "disableMacAddressRandomization": true,
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value"
}
```

### <a name="response"></a><span data-ttu-id="ff76e-266">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff76e-266">Response</span></span>
<span data-ttu-id="ff76e-p129">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff76e-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2189

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
  "id": "7593f7ba-f7ba-7593-baf7-9375baf79375",
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
  "disableMacAddressRandomization": true,
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value"
}
```




