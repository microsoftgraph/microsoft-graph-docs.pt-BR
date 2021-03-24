---
title: Atualizar androidDeviceOwnerEnterpriseWiFiConfiguration
description: Atualize as propriedades de um objeto androidDeviceOwnerEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e3e31a85edf8a35b48ccf62cdcf7b9ef0bb8bb42
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133497"
---
# <a name="update-androiddeviceownerenterprisewificonfiguration"></a><span data-ttu-id="a9207-103">Atualizar androidDeviceOwnerEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9207-103">Update androidDeviceOwnerEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="a9207-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9207-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9207-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9207-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9207-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9207-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9207-107">Atualize as propriedades de [um objeto androidDeviceOwnerEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-107">Update the properties of a [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9207-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9207-108">Prerequisites</span></span>
<span data-ttu-id="a9207-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9207-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9207-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9207-111">Permission type</span></span>|<span data-ttu-id="a9207-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9207-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9207-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9207-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9207-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9207-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9207-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9207-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9207-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9207-116">Not supported.</span></span>|
|<span data-ttu-id="a9207-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9207-117">Application</span></span>|<span data-ttu-id="a9207-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9207-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9207-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9207-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a9207-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9207-120">Request headers</span></span>
|<span data-ttu-id="a9207-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9207-121">Header</span></span>|<span data-ttu-id="a9207-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a9207-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9207-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9207-123">Authorization</span></span>|<span data-ttu-id="a9207-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9207-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9207-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a9207-125">Accept</span></span>|<span data-ttu-id="a9207-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9207-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9207-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9207-127">Request body</span></span>
<span data-ttu-id="a9207-128">No corpo da solicitação, fornece uma representação JSON para o [objeto androidDeviceOwnerEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-128">In the request body, supply a JSON representation for the [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="a9207-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9207-129">The following table shows the properties that are required when you create the [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="a9207-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9207-130">Property</span></span>|<span data-ttu-id="a9207-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9207-131">Type</span></span>|<span data-ttu-id="a9207-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9207-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9207-133">id</span><span class="sxs-lookup"><span data-stu-id="a9207-133">id</span></span>|<span data-ttu-id="a9207-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9207-134">String</span></span>|<span data-ttu-id="a9207-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a9207-135">Key of the entity.</span></span> <span data-ttu-id="a9207-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9207-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9207-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a9207-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9207-138">DateTimeOffset</span></span>|<span data-ttu-id="a9207-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a9207-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a9207-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9207-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a9207-141">roleScopeTagIds</span></span>|<span data-ttu-id="a9207-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9207-142">String collection</span></span>|<span data-ttu-id="a9207-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="a9207-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a9207-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9207-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a9207-145">supportsScopeTags</span></span>|<span data-ttu-id="a9207-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="a9207-146">Boolean</span></span>|<span data-ttu-id="a9207-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a9207-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a9207-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a9207-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a9207-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a9207-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a9207-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a9207-150">This property is read-only.</span></span> <span data-ttu-id="a9207-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9207-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a9207-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a9207-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a9207-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a9207-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="a9207-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a9207-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9207-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a9207-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a9207-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a9207-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a9207-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="a9207-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a9207-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9207-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a9207-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a9207-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a9207-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a9207-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="a9207-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a9207-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9207-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9207-164">createdDateTime</span></span>|<span data-ttu-id="a9207-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9207-165">DateTimeOffset</span></span>|<span data-ttu-id="a9207-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a9207-166">DateTime the object was created.</span></span> <span data-ttu-id="a9207-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9207-168">descrição</span><span class="sxs-lookup"><span data-stu-id="a9207-168">description</span></span>|<span data-ttu-id="a9207-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9207-169">String</span></span>|<span data-ttu-id="a9207-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a9207-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a9207-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9207-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a9207-172">displayName</span></span>|<span data-ttu-id="a9207-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9207-173">String</span></span>|<span data-ttu-id="a9207-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a9207-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a9207-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9207-176">versão</span><span class="sxs-lookup"><span data-stu-id="a9207-176">version</span></span>|<span data-ttu-id="a9207-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a9207-177">Int32</span></span>|<span data-ttu-id="a9207-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a9207-178">Version of the device configuration.</span></span> <span data-ttu-id="a9207-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9207-180">networkName</span><span class="sxs-lookup"><span data-stu-id="a9207-180">networkName</span></span>|<span data-ttu-id="a9207-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9207-181">String</span></span>|<span data-ttu-id="a9207-182">Nome da rede Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-182">Network Name Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="a9207-183">ssid</span><span class="sxs-lookup"><span data-stu-id="a9207-183">ssid</span></span>|<span data-ttu-id="a9207-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9207-184">String</span></span>|<span data-ttu-id="a9207-185">Esse é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a9207-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="a9207-186">Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-186">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="a9207-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="a9207-187">connectAutomatically</span></span>|<span data-ttu-id="a9207-188">Booleano</span><span class="sxs-lookup"><span data-stu-id="a9207-188">Boolean</span></span>|<span data-ttu-id="a9207-189">Conecte-se automaticamente quando essa rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="a9207-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="a9207-190">Definir isso como true ignorará o prompt do usuário e conectará automaticamente o dispositivo Wi-Fi rede.</span><span class="sxs-lookup"><span data-stu-id="a9207-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="a9207-191">Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-191">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="a9207-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="a9207-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="a9207-193">Booleano</span><span class="sxs-lookup"><span data-stu-id="a9207-193">Boolean</span></span>|<span data-ttu-id="a9207-194">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a9207-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="a9207-195">Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-195">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="a9207-196">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="a9207-196">wiFiSecurityType</span></span>|[<span data-ttu-id="a9207-197">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="a9207-197">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="a9207-198">Indica se Wi-Fi ponto de extremidade usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="a9207-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="a9207-199">Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9207-199">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span></span> <span data-ttu-id="a9207-200">Os valores possíveis são: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="a9207-200">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="a9207-201">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="a9207-201">preSharedKey</span></span>|<span data-ttu-id="a9207-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9207-202">String</span></span>|<span data-ttu-id="a9207-203">Esta é a chave pré-compartilhada para a rede WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="a9207-203">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="a9207-204">Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-204">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="a9207-205">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="a9207-205">preSharedKeyIsSet</span></span>|<span data-ttu-id="a9207-206">Booleano</span><span class="sxs-lookup"><span data-stu-id="a9207-206">Boolean</span></span>|<span data-ttu-id="a9207-207">Esta é a chave pré-compartilhada para a rede WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="a9207-207">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="a9207-208">Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9207-208">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="a9207-209">eapType</span><span class="sxs-lookup"><span data-stu-id="a9207-209">eapType</span></span>|[<span data-ttu-id="a9207-210">androidEapType</span><span class="sxs-lookup"><span data-stu-id="a9207-210">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="a9207-211">Indica o tipo de conjunto de protocolo EAP no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="a9207-211">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="a9207-212">Os valores possíveis são: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="a9207-212">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="a9207-213">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a9207-213">authenticationMethod</span></span>|[<span data-ttu-id="a9207-214">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a9207-214">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="a9207-215">Indica o Método de Autenticação que o cliente (dispositivo) precisa usar quando o Tipo de EAP está configurado para PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="a9207-215">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="a9207-216">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="a9207-216">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a9207-217">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="a9207-217">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="a9207-218">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="a9207-218">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="a9207-219">Método não EAP para Autenticação (Identidade Interna) quando Tipo de EAP é EAP-TTLS e Authenticationmethod é Nome de Usuário e Senha.</span><span class="sxs-lookup"><span data-stu-id="a9207-219">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="a9207-220">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="a9207-220">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="a9207-221">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="a9207-221">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="a9207-222">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="a9207-222">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="a9207-223">Método não EAP para Autenticação (Identidade Interna) quando Tipo de EAP é PEAP e Authenticationmethod é Nome de Usuário e Senha.</span><span class="sxs-lookup"><span data-stu-id="a9207-223">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="a9207-224">Os valores possíveis são: `none` e `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="a9207-224">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="a9207-225">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="a9207-225">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="a9207-226">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9207-226">String</span></span>|<span data-ttu-id="a9207-227">Habilita a privacidade de identidade (Identidade Externa) quando o Tipo EAP estiver configurado para EAP-TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="a9207-227">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="a9207-228">A cadeia de caracteres fornecida aqui é usada para mascarar o nome de usuário de usuários individuais quando eles tentam se conectar Wi-Fi rede.</span><span class="sxs-lookup"><span data-stu-id="a9207-228">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="a9207-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9207-229">Response</span></span>
<span data-ttu-id="a9207-230">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9207-230">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9207-231">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9207-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9207-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9207-232">Request</span></span>
<span data-ttu-id="a9207-233">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9207-233">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1612

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration",
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
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true,
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="a9207-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9207-234">Response</span></span>
<span data-ttu-id="a9207-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9207-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1784

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration",
  "id": "7ef0d9c3-d9c3-7ef0-c3d9-f07ec3d9f07e",
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
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true,
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




