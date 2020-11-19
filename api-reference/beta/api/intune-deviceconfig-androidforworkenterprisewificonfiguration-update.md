---
title: Atualizar androidForWorkEnterpriseWiFiConfiguration
description: Atualiza as propriedades de um objeto androidForWorkEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 45206bae46d805fc234a989d97e47b0c27a52b7b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49239159"
---
# <a name="update-androidforworkenterprisewificonfiguration"></a><span data-ttu-id="d78e1-103">Atualizar androidForWorkEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="d78e1-103">Update androidForWorkEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="d78e1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d78e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d78e1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d78e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d78e1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d78e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d78e1-107">Atualiza as propriedades de um objeto [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d78e1-107">Update the properties of a [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d78e1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d78e1-108">Prerequisites</span></span>
<span data-ttu-id="d78e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d78e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d78e1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d78e1-111">Permission type</span></span>|<span data-ttu-id="d78e1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d78e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d78e1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d78e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d78e1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d78e1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d78e1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d78e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d78e1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d78e1-116">Not supported.</span></span>|
|<span data-ttu-id="d78e1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d78e1-117">Application</span></span>|<span data-ttu-id="d78e1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d78e1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d78e1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d78e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d78e1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d78e1-120">Request headers</span></span>
|<span data-ttu-id="d78e1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d78e1-121">Header</span></span>|<span data-ttu-id="d78e1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d78e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d78e1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d78e1-123">Authorization</span></span>|<span data-ttu-id="d78e1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d78e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d78e1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d78e1-125">Accept</span></span>|<span data-ttu-id="d78e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d78e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d78e1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d78e1-127">Request body</span></span>
<span data-ttu-id="d78e1-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d78e1-128">In the request body, supply a JSON representation for the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="d78e1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d78e1-129">The following table shows the properties that are required when you create the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="d78e1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d78e1-130">Property</span></span>|<span data-ttu-id="d78e1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d78e1-131">Type</span></span>|<span data-ttu-id="d78e1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d78e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d78e1-133">id</span><span class="sxs-lookup"><span data-stu-id="d78e1-133">id</span></span>|<span data-ttu-id="d78e1-134">String</span><span class="sxs-lookup"><span data-stu-id="d78e1-134">String</span></span>|<span data-ttu-id="d78e1-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d78e1-135">Key of the entity.</span></span> <span data-ttu-id="d78e1-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d78e1-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78e1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d78e1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d78e1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d78e1-138">DateTimeOffset</span></span>|<span data-ttu-id="d78e1-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d78e1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d78e1-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d78e1-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78e1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d78e1-141">roleScopeTagIds</span></span>|<span data-ttu-id="d78e1-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d78e1-142">String collection</span></span>|<span data-ttu-id="d78e1-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d78e1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d78e1-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d78e1-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78e1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d78e1-145">supportsScopeTags</span></span>|<span data-ttu-id="d78e1-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="d78e1-146">Boolean</span></span>|<span data-ttu-id="d78e1-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d78e1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d78e1-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d78e1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d78e1-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d78e1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d78e1-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d78e1-150">This property is read-only.</span></span> <span data-ttu-id="d78e1-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d78e1-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78e1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d78e1-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d78e1-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d78e1-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d78e1-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="d78e1-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d78e1-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d78e1-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78e1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d78e1-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d78e1-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d78e1-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d78e1-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="d78e1-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d78e1-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d78e1-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78e1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d78e1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d78e1-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d78e1-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d78e1-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="d78e1-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d78e1-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d78e1-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78e1-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d78e1-164">createdDateTime</span></span>|<span data-ttu-id="d78e1-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d78e1-165">DateTimeOffset</span></span>|<span data-ttu-id="d78e1-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d78e1-166">DateTime the object was created.</span></span> <span data-ttu-id="d78e1-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d78e1-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78e1-168">description</span><span class="sxs-lookup"><span data-stu-id="d78e1-168">description</span></span>|<span data-ttu-id="d78e1-169">String</span><span class="sxs-lookup"><span data-stu-id="d78e1-169">String</span></span>|<span data-ttu-id="d78e1-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d78e1-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d78e1-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d78e1-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78e1-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d78e1-172">displayName</span></span>|<span data-ttu-id="d78e1-173">String</span><span class="sxs-lookup"><span data-stu-id="d78e1-173">String</span></span>|<span data-ttu-id="d78e1-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d78e1-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d78e1-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d78e1-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78e1-176">versão</span><span class="sxs-lookup"><span data-stu-id="d78e1-176">version</span></span>|<span data-ttu-id="d78e1-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d78e1-177">Int32</span></span>|<span data-ttu-id="d78e1-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d78e1-178">Version of the device configuration.</span></span> <span data-ttu-id="d78e1-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d78e1-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d78e1-180">NetworkName</span><span class="sxs-lookup"><span data-stu-id="d78e1-180">networkName</span></span>|<span data-ttu-id="d78e1-181">String</span><span class="sxs-lookup"><span data-stu-id="d78e1-181">String</span></span>|<span data-ttu-id="d78e1-182">Nome da rede herdado de [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d78e1-182">Network Name Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="d78e1-183">SSID</span><span class="sxs-lookup"><span data-stu-id="d78e1-183">ssid</span></span>|<span data-ttu-id="d78e1-184">String</span><span class="sxs-lookup"><span data-stu-id="d78e1-184">String</span></span>|<span data-ttu-id="d78e1-185">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d78e1-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="d78e1-186">Herdado de [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d78e1-186">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="d78e1-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="d78e1-187">connectAutomatically</span></span>|<span data-ttu-id="d78e1-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="d78e1-188">Boolean</span></span>|<span data-ttu-id="d78e1-189">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="d78e1-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="d78e1-190">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo ao Wi-Fi rede.</span><span class="sxs-lookup"><span data-stu-id="d78e1-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="d78e1-191">Herdado de [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d78e1-191">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="d78e1-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="d78e1-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="d78e1-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="d78e1-193">Boolean</span></span>|<span data-ttu-id="d78e1-194">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d78e1-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="d78e1-195">Herdado de [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d78e1-195">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="d78e1-196">à</span><span class="sxs-lookup"><span data-stu-id="d78e1-196">wiFiSecurityType</span></span>|[<span data-ttu-id="d78e1-197">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="d78e1-197">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="d78e1-198">Indica se Wi-Fi ponto de extremidade usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="d78e1-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="d78e1-199">Herdado de [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d78e1-199">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span> <span data-ttu-id="d78e1-200">Os valores possíveis são: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="d78e1-200">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="d78e1-201">eapType</span><span class="sxs-lookup"><span data-stu-id="d78e1-201">eapType</span></span>|[<span data-ttu-id="d78e1-202">androidEapType</span><span class="sxs-lookup"><span data-stu-id="d78e1-202">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="d78e1-203">Indica o tipo de protocolo EAP definido no ponto de extremidade de Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="d78e1-203">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="d78e1-204">Os valores possíveis são: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="d78e1-204">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="d78e1-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d78e1-205">authenticationMethod</span></span>|[<span data-ttu-id="d78e1-206">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d78e1-206">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="d78e1-207">Indica o método de autenticação que o cliente (dispositivo) precisa usar quando o tipo EAP é configurado como PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="d78e1-207">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="d78e1-208">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="d78e1-208">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="d78e1-209">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="d78e1-209">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="d78e1-210">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="d78e1-210">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="d78e1-211">Método não EAP para autenticação (identidade interna) quando o tipo EAP é EAP-TTLS e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="d78e1-211">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="d78e1-212">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="d78e1-212">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="d78e1-213">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="d78e1-213">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="d78e1-214">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="d78e1-214">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="d78e1-215">Método não EAP para autenticação (identidade interna) quando o tipo EAP é PEAP e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="d78e1-215">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="d78e1-216">Os valores possíveis são: `none` e `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="d78e1-216">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="d78e1-217">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="d78e1-217">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="d78e1-218">String</span><span class="sxs-lookup"><span data-stu-id="d78e1-218">String</span></span>|<span data-ttu-id="d78e1-219">Habilitar Privacidade de identidade (identidade externa) quando o tipo EAP é configurado como EAP-TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="d78e1-219">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="d78e1-220">A cadeia de caracteres fornecida aqui é usada para mascarar o nome de usuário de usuários individuais quando eles tentam se conectar à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="d78e1-220">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="d78e1-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="d78e1-221">Response</span></span>
<span data-ttu-id="d78e1-222">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d78e1-222">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d78e1-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d78e1-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="d78e1-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d78e1-224">Request</span></span>
<span data-ttu-id="d78e1-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d78e1-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1545

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
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
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="d78e1-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="d78e1-226">Response</span></span>
<span data-ttu-id="d78e1-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d78e1-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1717

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
  "id": "742d953a-953a-742d-3a95-2d743a952d74",
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
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




