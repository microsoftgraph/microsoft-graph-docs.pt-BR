---
title: Atualizar androidDeviceOwnerEnterpriseWiFiConfiguration
description: Atualiza as propriedades de um objeto androidDeviceOwnerEnterpriseWiFiConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0a938e20c31988a903a711f569c0c63b24ff968f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759833"
---
# <a name="update-androiddeviceownerenterprisewificonfiguration"></a><span data-ttu-id="bcd65-103">Atualizar androidDeviceOwnerEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="bcd65-103">Update androidDeviceOwnerEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="bcd65-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bcd65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcd65-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bcd65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcd65-106">Atualiza as propriedades de um objeto [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bcd65-106">Update the properties of a [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcd65-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bcd65-107">Prerequisites</span></span>
<span data-ttu-id="bcd65-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcd65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcd65-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bcd65-110">Permission type</span></span>|<span data-ttu-id="bcd65-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bcd65-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcd65-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bcd65-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bcd65-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcd65-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bcd65-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bcd65-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcd65-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcd65-115">Not supported.</span></span>|
|<span data-ttu-id="bcd65-116">Application</span><span class="sxs-lookup"><span data-stu-id="bcd65-116">Application</span></span>|<span data-ttu-id="bcd65-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcd65-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcd65-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcd65-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bcd65-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bcd65-119">Request headers</span></span>
|<span data-ttu-id="bcd65-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bcd65-120">Header</span></span>|<span data-ttu-id="bcd65-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bcd65-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcd65-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bcd65-122">Authorization</span></span>|<span data-ttu-id="bcd65-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bcd65-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcd65-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bcd65-124">Accept</span></span>|<span data-ttu-id="bcd65-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bcd65-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcd65-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcd65-126">Request body</span></span>
<span data-ttu-id="bcd65-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bcd65-127">In the request body, supply a JSON representation for the [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="bcd65-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bcd65-128">The following table shows the properties that are required when you create the [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="bcd65-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bcd65-129">Property</span></span>|<span data-ttu-id="bcd65-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcd65-130">Type</span></span>|<span data-ttu-id="bcd65-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcd65-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcd65-132">id</span><span class="sxs-lookup"><span data-stu-id="bcd65-132">id</span></span>|<span data-ttu-id="bcd65-133">String</span><span class="sxs-lookup"><span data-stu-id="bcd65-133">String</span></span>|<span data-ttu-id="bcd65-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bcd65-134">Key of the entity.</span></span> <span data-ttu-id="bcd65-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bcd65-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bcd65-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcd65-137">DateTimeOffset</span></span>|<span data-ttu-id="bcd65-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="bcd65-138">DateTime the object was last modified.</span></span> <span data-ttu-id="bcd65-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bcd65-140">roleScopeTagIds</span></span>|<span data-ttu-id="bcd65-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bcd65-141">String collection</span></span>|<span data-ttu-id="bcd65-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="bcd65-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bcd65-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bcd65-144">supportsScopeTags</span></span>|<span data-ttu-id="bcd65-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="bcd65-145">Boolean</span></span>|<span data-ttu-id="bcd65-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="bcd65-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bcd65-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="bcd65-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bcd65-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="bcd65-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bcd65-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bcd65-149">This property is read-only.</span></span> <span data-ttu-id="bcd65-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bcd65-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bcd65-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bcd65-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bcd65-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="bcd65-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bcd65-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bcd65-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bcd65-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bcd65-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bcd65-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="bcd65-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bcd65-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bcd65-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bcd65-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bcd65-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bcd65-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="bcd65-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bcd65-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bcd65-163">createdDateTime</span></span>|<span data-ttu-id="bcd65-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcd65-164">DateTimeOffset</span></span>|<span data-ttu-id="bcd65-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="bcd65-165">DateTime the object was created.</span></span> <span data-ttu-id="bcd65-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-167">description</span><span class="sxs-lookup"><span data-stu-id="bcd65-167">description</span></span>|<span data-ttu-id="bcd65-168">String</span><span class="sxs-lookup"><span data-stu-id="bcd65-168">String</span></span>|<span data-ttu-id="bcd65-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bcd65-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bcd65-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-171">displayName</span><span class="sxs-lookup"><span data-stu-id="bcd65-171">displayName</span></span>|<span data-ttu-id="bcd65-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bcd65-172">String</span></span>|<span data-ttu-id="bcd65-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bcd65-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bcd65-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-175">versão</span><span class="sxs-lookup"><span data-stu-id="bcd65-175">version</span></span>|<span data-ttu-id="bcd65-176">Int32</span><span class="sxs-lookup"><span data-stu-id="bcd65-176">Int32</span></span>|<span data-ttu-id="bcd65-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bcd65-177">Version of the device configuration.</span></span> <span data-ttu-id="bcd65-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-179">NetworkName</span><span class="sxs-lookup"><span data-stu-id="bcd65-179">networkName</span></span>|<span data-ttu-id="bcd65-180">String</span><span class="sxs-lookup"><span data-stu-id="bcd65-180">String</span></span>|<span data-ttu-id="bcd65-181">Nome da rede herdado de [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-181">Network Name Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-182">SSID</span><span class="sxs-lookup"><span data-stu-id="bcd65-182">ssid</span></span>|<span data-ttu-id="bcd65-183">String</span><span class="sxs-lookup"><span data-stu-id="bcd65-183">String</span></span>|<span data-ttu-id="bcd65-184">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="bcd65-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="bcd65-185">Herdado de [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-185">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="bcd65-186">connectAutomatically</span></span>|<span data-ttu-id="bcd65-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="bcd65-187">Boolean</span></span>|<span data-ttu-id="bcd65-188">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="bcd65-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="bcd65-189">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="bcd65-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="bcd65-190">Herdado de [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-190">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="bcd65-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="bcd65-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="bcd65-192">Boolean</span></span>|<span data-ttu-id="bcd65-193">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="bcd65-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="bcd65-194">Herdado de [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-194">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-195">à</span><span class="sxs-lookup"><span data-stu-id="bcd65-195">wiFiSecurityType</span></span>|[<span data-ttu-id="bcd65-196">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="bcd65-196">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="bcd65-197">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="bcd65-197">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="bcd65-198">Herdado de [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bcd65-198">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span></span> <span data-ttu-id="bcd65-199">Os valores possíveis são: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="bcd65-199">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="bcd65-200">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="bcd65-200">preSharedKey</span></span>|<span data-ttu-id="bcd65-201">String</span><span class="sxs-lookup"><span data-stu-id="bcd65-201">String</span></span>|<span data-ttu-id="bcd65-202">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="bcd65-202">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="bcd65-203">Herdado de [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-203">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-204">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="bcd65-204">preSharedKeyIsSet</span></span>|<span data-ttu-id="bcd65-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="bcd65-205">Boolean</span></span>|<span data-ttu-id="bcd65-206">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="bcd65-206">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="bcd65-207">Herdado de [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bcd65-207">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="bcd65-208">eapType</span><span class="sxs-lookup"><span data-stu-id="bcd65-208">eapType</span></span>|[<span data-ttu-id="bcd65-209">androidEapType</span><span class="sxs-lookup"><span data-stu-id="bcd65-209">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="bcd65-210">Indica o tipo de protocolo EAP definido no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="bcd65-210">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="bcd65-211">Os valores possíveis são: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="bcd65-211">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="bcd65-212">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="bcd65-212">authenticationMethod</span></span>|[<span data-ttu-id="bcd65-213">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="bcd65-213">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="bcd65-214">Indica o método de autenticação que o cliente (dispositivo) precisa usar quando o tipo EAP é configurado como PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="bcd65-214">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="bcd65-215">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="bcd65-215">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="bcd65-216">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="bcd65-216">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="bcd65-217">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="bcd65-217">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="bcd65-218">Método não EAP para autenticação (identidade interna) quando o tipo EAP é EAP-TTLS e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="bcd65-218">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="bcd65-219">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="bcd65-219">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="bcd65-220">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="bcd65-220">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="bcd65-221">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="bcd65-221">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="bcd65-222">Método não EAP para autenticação (identidade interna) quando o tipo EAP é PEAP e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="bcd65-222">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="bcd65-223">Os valores possíveis são: `none` e `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="bcd65-223">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="bcd65-224">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="bcd65-224">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="bcd65-225">String</span><span class="sxs-lookup"><span data-stu-id="bcd65-225">String</span></span>|<span data-ttu-id="bcd65-226">Habilitar Privacidade de identidade (identidade externa) quando o tipo EAP é configurado como EAP-TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="bcd65-226">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="bcd65-227">A cadeia de caracteres fornecida aqui é usada para mascarar o nome de usuário de usuários individuais quando eles tentam se conectar à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="bcd65-227">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="bcd65-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcd65-228">Response</span></span>
<span data-ttu-id="bcd65-229">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcd65-229">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcd65-230">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bcd65-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcd65-231">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcd65-231">Request</span></span>
<span data-ttu-id="bcd65-232">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcd65-232">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bcd65-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcd65-233">Response</span></span>
<span data-ttu-id="bcd65-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bcd65-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




