---
title: Atualizar macOSEnterpriseWiFiConfiguration
description: Atualize as propriedades de um objeto macOSEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4299de6dd2ec44aae245340b3dd38ecf77e4681a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151197"
---
# <a name="update-macosenterprisewificonfiguration"></a><span data-ttu-id="4c5cf-103">Atualizar macOSEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="4c5cf-103">Update macOSEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="4c5cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c5cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c5cf-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c5cf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c5cf-107">Atualize as propriedades de [um objeto macOSEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-107">Update the properties of a [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c5cf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4c5cf-108">Prerequisites</span></span>
<span data-ttu-id="4c5cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c5cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c5cf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c5cf-111">Permission type</span></span>|<span data-ttu-id="4c5cf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c5cf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c5cf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c5cf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c5cf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c5cf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-116">Not supported.</span></span>|
|<span data-ttu-id="4c5cf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c5cf-117">Application</span></span>|<span data-ttu-id="4c5cf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c5cf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c5cf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c5cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4c5cf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c5cf-120">Request headers</span></span>
|<span data-ttu-id="4c5cf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c5cf-121">Header</span></span>|<span data-ttu-id="4c5cf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4c5cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c5cf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c5cf-123">Authorization</span></span>|<span data-ttu-id="4c5cf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c5cf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4c5cf-125">Accept</span></span>|<span data-ttu-id="4c5cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c5cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c5cf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c5cf-127">Request body</span></span>
<span data-ttu-id="4c5cf-128">No corpo da solicitação, fornece uma representação JSON para o [objeto macOSEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-128">In the request body, supply a JSON representation for the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="4c5cf-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c5cf-129">The following table shows the properties that are required when you create the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="4c5cf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c5cf-130">Property</span></span>|<span data-ttu-id="4c5cf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c5cf-131">Type</span></span>|<span data-ttu-id="4c5cf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c5cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c5cf-133">id</span><span class="sxs-lookup"><span data-stu-id="4c5cf-133">id</span></span>|<span data-ttu-id="4c5cf-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c5cf-134">String</span></span>|<span data-ttu-id="4c5cf-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-135">Key of the entity.</span></span> <span data-ttu-id="4c5cf-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c5cf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4c5cf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c5cf-138">DateTimeOffset</span></span>|<span data-ttu-id="4c5cf-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4c5cf-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4c5cf-141">roleScopeTagIds</span></span>|<span data-ttu-id="4c5cf-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c5cf-142">String collection</span></span>|<span data-ttu-id="4c5cf-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4c5cf-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4c5cf-145">supportsScopeTags</span></span>|<span data-ttu-id="4c5cf-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="4c5cf-146">Boolean</span></span>|<span data-ttu-id="4c5cf-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4c5cf-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4c5cf-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4c5cf-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-150">This property is read-only.</span></span> <span data-ttu-id="4c5cf-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4c5cf-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4c5cf-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4c5cf-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4c5cf-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4c5cf-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4c5cf-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4c5cf-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4c5cf-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4c5cf-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4c5cf-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4c5cf-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4c5cf-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4c5cf-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4c5cf-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4c5cf-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c5cf-164">createdDateTime</span></span>|<span data-ttu-id="4c5cf-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c5cf-165">DateTimeOffset</span></span>|<span data-ttu-id="4c5cf-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-166">DateTime the object was created.</span></span> <span data-ttu-id="4c5cf-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-168">descrição</span><span class="sxs-lookup"><span data-stu-id="4c5cf-168">description</span></span>|<span data-ttu-id="4c5cf-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c5cf-169">String</span></span>|<span data-ttu-id="4c5cf-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4c5cf-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4c5cf-172">displayName</span></span>|<span data-ttu-id="4c5cf-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c5cf-173">String</span></span>|<span data-ttu-id="4c5cf-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4c5cf-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-176">versão</span><span class="sxs-lookup"><span data-stu-id="4c5cf-176">version</span></span>|<span data-ttu-id="4c5cf-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4c5cf-177">Int32</span></span>|<span data-ttu-id="4c5cf-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-178">Version of the device configuration.</span></span> <span data-ttu-id="4c5cf-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-180">networkName</span><span class="sxs-lookup"><span data-stu-id="4c5cf-180">networkName</span></span>|<span data-ttu-id="4c5cf-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c5cf-181">String</span></span>|<span data-ttu-id="4c5cf-182">Nome da rede Herdado [de macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-182">Network Name Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-183">ssid</span><span class="sxs-lookup"><span data-stu-id="4c5cf-183">ssid</span></span>|<span data-ttu-id="4c5cf-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c5cf-184">String</span></span>|<span data-ttu-id="4c5cf-185">Esse é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="4c5cf-186">Herdado [do macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-186">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="4c5cf-187">connectAutomatically</span></span>|<span data-ttu-id="4c5cf-188">Booleano</span><span class="sxs-lookup"><span data-stu-id="4c5cf-188">Boolean</span></span>|<span data-ttu-id="4c5cf-189">Conecte-se automaticamente quando essa rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="4c5cf-190">Definir isso como true ignorará o prompt do usuário e conectará automaticamente o dispositivo Wi-Fi rede.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="4c5cf-191">Herdado [do macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-191">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="4c5cf-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="4c5cf-193">Booleano</span><span class="sxs-lookup"><span data-stu-id="4c5cf-193">Boolean</span></span>|<span data-ttu-id="4c5cf-194">Conecte-se quando a rede não estiver transmitindo seu nome (SSID).</span><span class="sxs-lookup"><span data-stu-id="4c5cf-194">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="4c5cf-195">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-195">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="4c5cf-196">Herdado [do macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-196">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-197">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="4c5cf-197">wiFiSecurityType</span></span>|[<span data-ttu-id="4c5cf-198">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="4c5cf-198">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="4c5cf-199">Indica se Wi-Fi ponto de extremidade usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-199">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="4c5cf-200">Herdado [de macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c5cf-200">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="4c5cf-201">Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-201">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="4c5cf-202">proxySettings</span><span class="sxs-lookup"><span data-stu-id="4c5cf-202">proxySettings</span></span>|[<span data-ttu-id="4c5cf-203">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="4c5cf-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="4c5cf-204">Tipo de proxy para essa Wi-Fi herdada de [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c5cf-204">Proxy Type for this Wi-Fi connection Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="4c5cf-205">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="4c5cf-206">proxyManualAddress</span><span class="sxs-lookup"><span data-stu-id="4c5cf-206">proxyManualAddress</span></span>|<span data-ttu-id="4c5cf-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c5cf-207">String</span></span>|<span data-ttu-id="4c5cf-208">Endereço IP ou nome de host DNS do servidor proxy quando a configuração manual é selecionada.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-208">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="4c5cf-209">Herdado [do macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-209">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-210">proxyManualPort</span><span class="sxs-lookup"><span data-stu-id="4c5cf-210">proxyManualPort</span></span>|<span data-ttu-id="4c5cf-211">Int32</span><span class="sxs-lookup"><span data-stu-id="4c5cf-211">Int32</span></span>|<span data-ttu-id="4c5cf-212">Porta do servidor proxy quando a configuração manual é selecionada.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-212">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="4c5cf-213">Herdado [do macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-213">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-214">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="4c5cf-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="4c5cf-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c5cf-215">String</span></span>|<span data-ttu-id="4c5cf-216">URL do script de configuração automática do servidor proxy quando a configuração automática é selecionada.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-216">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="4c5cf-217">Normalmente, essa URL é o local do arquivo PAC (Configuração Automática de Proxy).</span><span class="sxs-lookup"><span data-stu-id="4c5cf-217">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="4c5cf-218">Herdado [do macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-218">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-219">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="4c5cf-219">preSharedKey</span></span>|<span data-ttu-id="4c5cf-220">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c5cf-220">String</span></span>|<span data-ttu-id="4c5cf-221">Esta é a chave pré-compartilhada para a rede WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-221">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="4c5cf-222">Herdado [do macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c5cf-222">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="4c5cf-223">eapType</span><span class="sxs-lookup"><span data-stu-id="4c5cf-223">eapType</span></span>|[<span data-ttu-id="4c5cf-224">eapType</span><span class="sxs-lookup"><span data-stu-id="4c5cf-224">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="4c5cf-225">Protocolo de Autenticação Extensível (EAP).</span><span class="sxs-lookup"><span data-stu-id="4c5cf-225">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="4c5cf-226">Indica o tipo de conjunto de protocolo EAP no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="4c5cf-226">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="4c5cf-227">Os possíveis valores são: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-227">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="4c5cf-228">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="4c5cf-228">eapFastConfiguration</span></span>|[<span data-ttu-id="4c5cf-229">eapFastConfiguration</span><span class="sxs-lookup"><span data-stu-id="4c5cf-229">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="4c5cf-230">Opção de Configuração EAP-FAST quando EAP-FAST é o Tipo EAP selecionado.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-230">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="4c5cf-231">Os valores possíveis são: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-231">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="4c5cf-232">trustedServerCertificateNames</span><span class="sxs-lookup"><span data-stu-id="4c5cf-232">trustedServerCertificateNames</span></span>|<span data-ttu-id="4c5cf-233">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c5cf-233">String collection</span></span>|<span data-ttu-id="4c5cf-234">Nomes de certificados de servidor confiáveis quando Tipo de EAP é configurado para EAP-TLS/TTLS/FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-234">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="4c5cf-235">Esse é o nome comum usado nos certificados emitidos pela autoridade de certificação confiável (CA).</span><span class="sxs-lookup"><span data-stu-id="4c5cf-235">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="4c5cf-236">Se você fornecer essas informações, poderá ignorar a caixa de diálogo de confiança dinâmica exibida em dispositivos de usuários finais quando eles se conectarem a essa rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-236">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="4c5cf-237">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4c5cf-237">authenticationMethod</span></span>|[<span data-ttu-id="4c5cf-238">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4c5cf-238">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="4c5cf-239">Método de autenticação quando Tipo de EAP é configurado para PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-239">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="4c5cf-240">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-240">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="4c5cf-241">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="4c5cf-241">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="4c5cf-242">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="4c5cf-242">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="4c5cf-243">Método não EAP para Autenticação (Identidade Interna) quando Tipo de EAP é EAP-TTLS e Authenticationmethod é Nome de Usuário e Senha.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-243">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="4c5cf-244">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-244">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="4c5cf-245">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="4c5cf-245">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="4c5cf-246">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c5cf-246">String</span></span>|<span data-ttu-id="4c5cf-247">Habilita a privacidade de identidade (Identidade Externa) quando o Tipo EAP estiver configurado para EAP-TTLS, EAP-FAST ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-247">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="4c5cf-248">Essa propriedade mascara os nomes de usuário com o texto que você inserir.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-248">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="4c5cf-249">Por exemplo, se você usar 'anônimo', cada usuário que se autenticar com essa conexão Wi-Fi usando seu nome de usuário real será exibido como "anônimo".</span><span class="sxs-lookup"><span data-stu-id="4c5cf-249">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="4c5cf-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c5cf-250">Response</span></span>
<span data-ttu-id="4c5cf-251">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-251">If successful, this method returns a `200 OK` response code and an updated [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c5cf-252">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c5cf-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c5cf-253">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c5cf-253">Request</span></span>
<span data-ttu-id="4c5cf-254">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-254">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1858

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
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
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="4c5cf-255">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c5cf-255">Response</span></span>
<span data-ttu-id="4c5cf-p128">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c5cf-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2030

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
  "id": "7a6f9a2e-9a2e-7a6f-2e9a-6f7a2e9a6f7a",
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
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




