---
title: Criar androidDeviceOwnerEnterpriseWiFiConfiguration
description: Crie um novo objeto androidDeviceOwnerEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 73ed73afd6bd0f82ce3a6141c60fad3b4f3a01e6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131845"
---
# <a name="create-androiddeviceownerenterprisewificonfiguration"></a><span data-ttu-id="abaca-103">Criar androidDeviceOwnerEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="abaca-103">Create androidDeviceOwnerEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="abaca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abaca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="abaca-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="abaca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abaca-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="abaca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abaca-107">Crie um novo [objeto androidDeviceOwnerEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-107">Create a new [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abaca-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="abaca-108">Prerequisites</span></span>
<span data-ttu-id="abaca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abaca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abaca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="abaca-111">Permission type</span></span>|<span data-ttu-id="abaca-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="abaca-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abaca-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="abaca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abaca-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abaca-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="abaca-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="abaca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abaca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="abaca-116">Not supported.</span></span>|
|<span data-ttu-id="abaca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="abaca-117">Application</span></span>|<span data-ttu-id="abaca-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abaca-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abaca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="abaca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="abaca-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="abaca-120">Request headers</span></span>
|<span data-ttu-id="abaca-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="abaca-121">Header</span></span>|<span data-ttu-id="abaca-122">Valor</span><span class="sxs-lookup"><span data-stu-id="abaca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abaca-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="abaca-123">Authorization</span></span>|<span data-ttu-id="abaca-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="abaca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abaca-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="abaca-125">Accept</span></span>|<span data-ttu-id="abaca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="abaca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abaca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="abaca-127">Request body</span></span>
<span data-ttu-id="abaca-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidDeviceOwnerEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="abaca-128">In the request body, supply a JSON representation for the androidDeviceOwnerEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="abaca-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o androidDeviceOwnerEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="abaca-129">The following table shows the properties that are required when you create the androidDeviceOwnerEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="abaca-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abaca-130">Property</span></span>|<span data-ttu-id="abaca-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="abaca-131">Type</span></span>|<span data-ttu-id="abaca-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="abaca-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abaca-133">id</span><span class="sxs-lookup"><span data-stu-id="abaca-133">id</span></span>|<span data-ttu-id="abaca-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abaca-134">String</span></span>|<span data-ttu-id="abaca-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="abaca-135">Key of the entity.</span></span> <span data-ttu-id="abaca-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abaca-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="abaca-137">lastModifiedDateTime</span></span>|<span data-ttu-id="abaca-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abaca-138">DateTimeOffset</span></span>|<span data-ttu-id="abaca-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="abaca-139">DateTime the object was last modified.</span></span> <span data-ttu-id="abaca-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abaca-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="abaca-141">roleScopeTagIds</span></span>|<span data-ttu-id="abaca-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="abaca-142">String collection</span></span>|<span data-ttu-id="abaca-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="abaca-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="abaca-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abaca-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="abaca-145">supportsScopeTags</span></span>|<span data-ttu-id="abaca-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="abaca-146">Boolean</span></span>|<span data-ttu-id="abaca-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="abaca-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="abaca-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="abaca-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="abaca-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="abaca-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="abaca-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="abaca-150">This property is read-only.</span></span> <span data-ttu-id="abaca-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abaca-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="abaca-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="abaca-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="abaca-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="abaca-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="abaca-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="abaca-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abaca-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="abaca-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="abaca-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="abaca-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="abaca-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="abaca-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="abaca-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abaca-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="abaca-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="abaca-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="abaca-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="abaca-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="abaca-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="abaca-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abaca-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="abaca-164">createdDateTime</span></span>|<span data-ttu-id="abaca-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abaca-165">DateTimeOffset</span></span>|<span data-ttu-id="abaca-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="abaca-166">DateTime the object was created.</span></span> <span data-ttu-id="abaca-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abaca-168">descrição</span><span class="sxs-lookup"><span data-stu-id="abaca-168">description</span></span>|<span data-ttu-id="abaca-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abaca-169">String</span></span>|<span data-ttu-id="abaca-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="abaca-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="abaca-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abaca-172">displayName</span><span class="sxs-lookup"><span data-stu-id="abaca-172">displayName</span></span>|<span data-ttu-id="abaca-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abaca-173">String</span></span>|<span data-ttu-id="abaca-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="abaca-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="abaca-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abaca-176">versão</span><span class="sxs-lookup"><span data-stu-id="abaca-176">version</span></span>|<span data-ttu-id="abaca-177">Int32</span><span class="sxs-lookup"><span data-stu-id="abaca-177">Int32</span></span>|<span data-ttu-id="abaca-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="abaca-178">Version of the device configuration.</span></span> <span data-ttu-id="abaca-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="abaca-180">networkName</span><span class="sxs-lookup"><span data-stu-id="abaca-180">networkName</span></span>|<span data-ttu-id="abaca-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abaca-181">String</span></span>|<span data-ttu-id="abaca-182">Nome da rede Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-182">Network Name Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="abaca-183">ssid</span><span class="sxs-lookup"><span data-stu-id="abaca-183">ssid</span></span>|<span data-ttu-id="abaca-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abaca-184">String</span></span>|<span data-ttu-id="abaca-185">Esse é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="abaca-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="abaca-186">Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-186">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="abaca-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="abaca-187">connectAutomatically</span></span>|<span data-ttu-id="abaca-188">Booleano</span><span class="sxs-lookup"><span data-stu-id="abaca-188">Boolean</span></span>|<span data-ttu-id="abaca-189">Conecte-se automaticamente quando essa rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="abaca-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="abaca-190">Definir isso como true ignorará o prompt do usuário e conectará automaticamente o dispositivo Wi-Fi rede.</span><span class="sxs-lookup"><span data-stu-id="abaca-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="abaca-191">Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-191">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="abaca-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="abaca-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="abaca-193">Booleano</span><span class="sxs-lookup"><span data-stu-id="abaca-193">Boolean</span></span>|<span data-ttu-id="abaca-194">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="abaca-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="abaca-195">Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-195">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="abaca-196">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="abaca-196">wiFiSecurityType</span></span>|[<span data-ttu-id="abaca-197">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="abaca-197">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="abaca-198">Indica se Wi-Fi ponto de extremidade usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="abaca-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="abaca-199">Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="abaca-199">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span></span> <span data-ttu-id="abaca-200">Os valores possíveis são: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="abaca-200">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="abaca-201">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="abaca-201">preSharedKey</span></span>|<span data-ttu-id="abaca-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abaca-202">String</span></span>|<span data-ttu-id="abaca-203">Esta é a chave pré-compartilhada para a rede WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="abaca-203">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="abaca-204">Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-204">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="abaca-205">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="abaca-205">preSharedKeyIsSet</span></span>|<span data-ttu-id="abaca-206">Booleano</span><span class="sxs-lookup"><span data-stu-id="abaca-206">Boolean</span></span>|<span data-ttu-id="abaca-207">Esta é a chave pré-compartilhada para a rede WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="abaca-207">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="abaca-208">Herdado [de androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="abaca-208">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="abaca-209">eapType</span><span class="sxs-lookup"><span data-stu-id="abaca-209">eapType</span></span>|[<span data-ttu-id="abaca-210">androidEapType</span><span class="sxs-lookup"><span data-stu-id="abaca-210">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="abaca-211">Indica o tipo de conjunto de protocolo EAP no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="abaca-211">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="abaca-212">Os valores possíveis são: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="abaca-212">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="abaca-213">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="abaca-213">authenticationMethod</span></span>|[<span data-ttu-id="abaca-214">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="abaca-214">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="abaca-215">Indica o Método de Autenticação que o cliente (dispositivo) precisa usar quando o Tipo de EAP está configurado para PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="abaca-215">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="abaca-216">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="abaca-216">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="abaca-217">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="abaca-217">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="abaca-218">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="abaca-218">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="abaca-219">Método não EAP para Autenticação (Identidade Interna) quando Tipo de EAP é EAP-TTLS e Authenticationmethod é Nome de Usuário e Senha.</span><span class="sxs-lookup"><span data-stu-id="abaca-219">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="abaca-220">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="abaca-220">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="abaca-221">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="abaca-221">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="abaca-222">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="abaca-222">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="abaca-223">Método não EAP para Autenticação (Identidade Interna) quando Tipo de EAP é PEAP e Authenticationmethod é Nome de Usuário e Senha.</span><span class="sxs-lookup"><span data-stu-id="abaca-223">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="abaca-224">Os valores possíveis são: `none` e `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="abaca-224">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="abaca-225">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="abaca-225">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="abaca-226">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="abaca-226">String</span></span>|<span data-ttu-id="abaca-227">Habilita a privacidade de identidade (Identidade Externa) quando o Tipo EAP estiver configurado para EAP-TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="abaca-227">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="abaca-228">A cadeia de caracteres fornecida aqui é usada para mascarar o nome de usuário de usuários individuais quando eles tentam se conectar Wi-Fi rede.</span><span class="sxs-lookup"><span data-stu-id="abaca-228">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="abaca-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="abaca-229">Response</span></span>
<span data-ttu-id="abaca-230">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="abaca-230">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abaca-231">Exemplo</span><span class="sxs-lookup"><span data-stu-id="abaca-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="abaca-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="abaca-232">Request</span></span>
<span data-ttu-id="abaca-233">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="abaca-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="abaca-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="abaca-234">Response</span></span>
<span data-ttu-id="abaca-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="abaca-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




