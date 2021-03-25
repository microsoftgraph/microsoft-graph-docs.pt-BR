---
title: Criar iosEnterpriseWiFiConfiguration
description: Crie um novo objeto iosEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 79df6dba6a4058b66f97bb95f74feb88a1a2e7b4
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151330"
---
# <a name="create-iosenterprisewificonfiguration"></a><span data-ttu-id="6e76d-103">Criar iosEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e76d-103">Create iosEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="6e76d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e76d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e76d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6e76d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e76d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6e76d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e76d-107">Crie um novo [objeto iosEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-107">Create a new [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e76d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6e76d-108">Prerequisites</span></span>
<span data-ttu-id="6e76d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e76d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e76d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e76d-111">Permission type</span></span>|<span data-ttu-id="6e76d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e76d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e76d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e76d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6e76d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e76d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6e76d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e76d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e76d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e76d-116">Not supported.</span></span>|
|<span data-ttu-id="6e76d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e76d-117">Application</span></span>|<span data-ttu-id="6e76d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e76d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e76d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e76d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6e76d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e76d-120">Request headers</span></span>
|<span data-ttu-id="6e76d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e76d-121">Header</span></span>|<span data-ttu-id="6e76d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6e76d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e76d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e76d-123">Authorization</span></span>|<span data-ttu-id="6e76d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e76d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e76d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6e76d-125">Accept</span></span>|<span data-ttu-id="6e76d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e76d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e76d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e76d-127">Request body</span></span>
<span data-ttu-id="6e76d-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6e76d-128">In the request body, supply a JSON representation for the iosEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="6e76d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6e76d-129">The following table shows the properties that are required when you create the iosEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="6e76d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e76d-130">Property</span></span>|<span data-ttu-id="6e76d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e76d-131">Type</span></span>|<span data-ttu-id="6e76d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e76d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e76d-133">id</span><span class="sxs-lookup"><span data-stu-id="6e76d-133">id</span></span>|<span data-ttu-id="6e76d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e76d-134">String</span></span>|<span data-ttu-id="6e76d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6e76d-135">Key of the entity.</span></span> <span data-ttu-id="6e76d-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e76d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6e76d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e76d-138">DateTimeOffset</span></span>|<span data-ttu-id="6e76d-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6e76d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6e76d-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6e76d-141">roleScopeTagIds</span></span>|<span data-ttu-id="6e76d-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e76d-142">String collection</span></span>|<span data-ttu-id="6e76d-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="6e76d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6e76d-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6e76d-145">supportsScopeTags</span></span>|<span data-ttu-id="6e76d-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="6e76d-146">Boolean</span></span>|<span data-ttu-id="6e76d-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6e76d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6e76d-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6e76d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6e76d-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6e76d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6e76d-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6e76d-150">This property is read-only.</span></span> <span data-ttu-id="6e76d-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6e76d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6e76d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6e76d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6e76d-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="6e76d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6e76d-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6e76d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6e76d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6e76d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6e76d-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="6e76d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6e76d-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6e76d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6e76d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6e76d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6e76d-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="6e76d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6e76d-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6e76d-164">createdDateTime</span></span>|<span data-ttu-id="6e76d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e76d-165">DateTimeOffset</span></span>|<span data-ttu-id="6e76d-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6e76d-166">DateTime the object was created.</span></span> <span data-ttu-id="6e76d-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-168">descrição</span><span class="sxs-lookup"><span data-stu-id="6e76d-168">description</span></span>|<span data-ttu-id="6e76d-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e76d-169">String</span></span>|<span data-ttu-id="6e76d-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6e76d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6e76d-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6e76d-172">displayName</span></span>|<span data-ttu-id="6e76d-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e76d-173">String</span></span>|<span data-ttu-id="6e76d-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6e76d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6e76d-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-176">versão</span><span class="sxs-lookup"><span data-stu-id="6e76d-176">version</span></span>|<span data-ttu-id="6e76d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6e76d-177">Int32</span></span>|<span data-ttu-id="6e76d-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6e76d-178">Version of the device configuration.</span></span> <span data-ttu-id="6e76d-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-180">networkName</span><span class="sxs-lookup"><span data-stu-id="6e76d-180">networkName</span></span>|<span data-ttu-id="6e76d-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e76d-181">String</span></span>|<span data-ttu-id="6e76d-182">Nome da rede Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-182">Network Name Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-183">ssid</span><span class="sxs-lookup"><span data-stu-id="6e76d-183">ssid</span></span>|<span data-ttu-id="6e76d-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e76d-184">String</span></span>|<span data-ttu-id="6e76d-185">Esse é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6e76d-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="6e76d-186">Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-186">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="6e76d-187">connectAutomatically</span></span>|<span data-ttu-id="6e76d-188">Booleano</span><span class="sxs-lookup"><span data-stu-id="6e76d-188">Boolean</span></span>|<span data-ttu-id="6e76d-189">Conecte-se automaticamente quando essa rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="6e76d-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="6e76d-190">Definir isso como true ignorará o prompt do usuário e conectará automaticamente o dispositivo Wi-Fi rede.</span><span class="sxs-lookup"><span data-stu-id="6e76d-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="6e76d-191">Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-191">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="6e76d-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="6e76d-193">Booleano</span><span class="sxs-lookup"><span data-stu-id="6e76d-193">Boolean</span></span>|<span data-ttu-id="6e76d-194">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="6e76d-194">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="6e76d-195">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6e76d-195">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="6e76d-196">Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-196">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-197">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="6e76d-197">wiFiSecurityType</span></span>|[<span data-ttu-id="6e76d-198">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="6e76d-198">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="6e76d-199">Indica se Wi-Fi ponto de extremidade usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="6e76d-199">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="6e76d-200">Herdado [de iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e76d-200">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="6e76d-201">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="6e76d-201">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="6e76d-202">proxySettings</span><span class="sxs-lookup"><span data-stu-id="6e76d-202">proxySettings</span></span>|[<span data-ttu-id="6e76d-203">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="6e76d-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="6e76d-204">Tipo de proxy para essa Wi-Fi herdada de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6e76d-204">Proxy Type for this Wi-Fi connection Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="6e76d-205">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="6e76d-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="6e76d-206">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="6e76d-206">proxyManualAddress</span></span>|<span data-ttu-id="6e76d-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e76d-207">String</span></span>|<span data-ttu-id="6e76d-208">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual é selecionada.</span><span class="sxs-lookup"><span data-stu-id="6e76d-208">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="6e76d-209">Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-209">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-210">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="6e76d-210">proxyManualPort</span></span>|<span data-ttu-id="6e76d-211">Int32</span><span class="sxs-lookup"><span data-stu-id="6e76d-211">Int32</span></span>|<span data-ttu-id="6e76d-212">Porta do servidor proxy quando a configuração manual é selecionada.</span><span class="sxs-lookup"><span data-stu-id="6e76d-212">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="6e76d-213">Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-213">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-214">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="6e76d-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="6e76d-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e76d-215">String</span></span>|<span data-ttu-id="6e76d-216">URL do script de configuração automática do servidor proxy quando a configuração automática é selecionada.</span><span class="sxs-lookup"><span data-stu-id="6e76d-216">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="6e76d-217">Normalmente, essa URL é o local do arquivo PAC (Configuração Automática de Proxy).</span><span class="sxs-lookup"><span data-stu-id="6e76d-217">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="6e76d-218">Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-218">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-219">disableMacAddressRandomization</span><span class="sxs-lookup"><span data-stu-id="6e76d-219">disableMacAddressRandomization</span></span>|<span data-ttu-id="6e76d-220">Booleano</span><span class="sxs-lookup"><span data-stu-id="6e76d-220">Boolean</span></span>|<span data-ttu-id="6e76d-221">Se definido como true, força os dispositivos que se conectam usando esse perfil de Wi-Fi para apresentar seu endereço MAC real Wi-Fi em vez de um endereço MAC aleatório.</span><span class="sxs-lookup"><span data-stu-id="6e76d-221">If set to true, forces devices connecting using this Wi-Fi profile to present their actual Wi-Fi MAC address instead of a random MAC address.</span></span> <span data-ttu-id="6e76d-222">Aplica-se ao iOS 14 e posterior.</span><span class="sxs-lookup"><span data-stu-id="6e76d-222">Applies to iOS 14 and later.</span></span> <span data-ttu-id="6e76d-223">Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-223">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-224">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="6e76d-224">preSharedKey</span></span>|<span data-ttu-id="6e76d-225">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e76d-225">String</span></span>|<span data-ttu-id="6e76d-226">Esta é a chave pré-compartilhada para a rede WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="6e76d-226">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="6e76d-227">Herdado do [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6e76d-227">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="6e76d-228">eapType</span><span class="sxs-lookup"><span data-stu-id="6e76d-228">eapType</span></span>|[<span data-ttu-id="6e76d-229">eapType</span><span class="sxs-lookup"><span data-stu-id="6e76d-229">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="6e76d-230">Protocolo de Autenticação Extensível (EAP).</span><span class="sxs-lookup"><span data-stu-id="6e76d-230">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="6e76d-231">Indica o tipo de conjunto de protocolo EAP no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="6e76d-231">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="6e76d-232">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="6e76d-232">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="6e76d-233">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e76d-233">eapFastConfiguration</span></span>|[<span data-ttu-id="6e76d-234">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e76d-234">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="6e76d-235">Opção de Configuração EAP-FAST quando EAP-FAST é o Tipo EAP selecionado.</span><span class="sxs-lookup"><span data-stu-id="6e76d-235">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="6e76d-236">Os valores possíveis são: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="6e76d-236">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="6e76d-237">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="6e76d-237">trustedServerCertificateNames</span></span>|<span data-ttu-id="6e76d-238">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e76d-238">String collection</span></span>|<span data-ttu-id="6e76d-239">Nomes de certificados de servidor confiáveis quando Tipo de EAP é configurado para EAP-TLS/TTLS/FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="6e76d-239">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="6e76d-240">Esse é o nome comum usado nos certificados emitidos pela autoridade de certificação confiável (CA).</span><span class="sxs-lookup"><span data-stu-id="6e76d-240">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="6e76d-241">Se você fornecer essas informações, poderá ignorar a caixa de diálogo de confiança dinâmica exibida nos dispositivos dos usuários finais quando eles se conectarem Wi-Fi rede.</span><span class="sxs-lookup"><span data-stu-id="6e76d-241">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users' devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="6e76d-242">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6e76d-242">authenticationMethod</span></span>|[<span data-ttu-id="6e76d-243">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6e76d-243">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="6e76d-244">Método de autenticação quando Tipo de EAP é configurado para PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="6e76d-244">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="6e76d-245">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="6e76d-245">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="6e76d-246">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="6e76d-246">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="6e76d-247">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="6e76d-247">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="6e76d-248">Método não EAP para autenticação quando Tipo EAP é EAP-TTLS e Authenticationmethod é Nome de Usuário e Senha.</span><span class="sxs-lookup"><span data-stu-id="6e76d-248">Non-EAP Method for Authentication when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="6e76d-249">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="6e76d-249">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="6e76d-250">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="6e76d-250">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="6e76d-251">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e76d-251">String</span></span>|<span data-ttu-id="6e76d-252">Habilita a privacidade de identidade (Identidade Externa) quando o Tipo EAP estiver configurado como EAP - TTLS, EAP - FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="6e76d-252">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP - TTLS, EAP - FAST or PEAP.</span></span> <span data-ttu-id="6e76d-253">Essa propriedade mascara os nomes de usuário com o texto que você inserir.</span><span class="sxs-lookup"><span data-stu-id="6e76d-253">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="6e76d-254">Por exemplo, se você usar 'anônimo', cada usuário que se autenticar com essa conexão Wi-Fi usando seu nome de usuário real será exibido como "anônimo".</span><span class="sxs-lookup"><span data-stu-id="6e76d-254">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|
|<span data-ttu-id="6e76d-255">usernameFormatString</span><span class="sxs-lookup"><span data-stu-id="6e76d-255">usernameFormatString</span></span>|<span data-ttu-id="6e76d-256">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e76d-256">String</span></span>|<span data-ttu-id="6e76d-257">Cadeia de caracteres de formato de nome de usuário usada para criar o nome de usuário para se conectar ao wifi</span><span class="sxs-lookup"><span data-stu-id="6e76d-257">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="6e76d-258">passwordFormatString</span><span class="sxs-lookup"><span data-stu-id="6e76d-258">passwordFormatString</span></span>|<span data-ttu-id="6e76d-259">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6e76d-259">String</span></span>|<span data-ttu-id="6e76d-260">Cadeia de caracteres de formato de senha usada para criar a senha para se conectar ao wifi</span><span class="sxs-lookup"><span data-stu-id="6e76d-260">Password format string used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="6e76d-261">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e76d-261">Response</span></span>
<span data-ttu-id="6e76d-262">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e76d-262">If successful, this method returns a `201 Created` response code and a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e76d-263">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e76d-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e76d-264">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e76d-264">Request</span></span>
<span data-ttu-id="6e76d-265">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e76d-265">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="6e76d-266">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e76d-266">Response</span></span>
<span data-ttu-id="6e76d-p129">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e76d-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




