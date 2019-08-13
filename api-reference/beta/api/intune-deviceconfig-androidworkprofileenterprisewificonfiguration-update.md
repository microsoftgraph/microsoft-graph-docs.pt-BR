---
title: Atualizar androidWorkProfileEnterpriseWiFiConfiguration
description: Atualiza as propriedades de um objeto androidWorkProfileEnterpriseWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a62a4405f4f4f93294e6b65877aec8a512ed25c5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311253"
---
# <a name="update-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="54895-103">Atualizar androidWorkProfileEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="54895-103">Update androidWorkProfileEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="54895-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54895-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54895-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54895-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54895-106">Atualiza as propriedades de um objeto [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="54895-106">Update the properties of a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54895-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54895-107">Prerequisites</span></span>
<span data-ttu-id="54895-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54895-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54895-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54895-110">Permission type</span></span>|<span data-ttu-id="54895-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="54895-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54895-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54895-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54895-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54895-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="54895-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54895-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54895-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54895-115">Not supported.</span></span>|
|<span data-ttu-id="54895-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54895-116">Application</span></span>|<span data-ttu-id="54895-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54895-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54895-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54895-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="54895-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54895-119">Request headers</span></span>
|<span data-ttu-id="54895-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54895-120">Header</span></span>|<span data-ttu-id="54895-121">Valor</span><span class="sxs-lookup"><span data-stu-id="54895-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54895-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="54895-122">Authorization</span></span>|<span data-ttu-id="54895-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54895-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54895-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="54895-124">Accept</span></span>|<span data-ttu-id="54895-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54895-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54895-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54895-126">Request body</span></span>
<span data-ttu-id="54895-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="54895-127">In the request body, supply a JSON representation for the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="54895-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54895-128">The following table shows the properties that are required when you create the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="54895-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54895-129">Property</span></span>|<span data-ttu-id="54895-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="54895-130">Type</span></span>|<span data-ttu-id="54895-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="54895-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54895-132">id</span><span class="sxs-lookup"><span data-stu-id="54895-132">id</span></span>|<span data-ttu-id="54895-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54895-133">String</span></span>|<span data-ttu-id="54895-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="54895-134">Key of the entity.</span></span> <span data-ttu-id="54895-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54895-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54895-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54895-136">lastModifiedDateTime</span></span>|<span data-ttu-id="54895-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54895-137">DateTimeOffset</span></span>|<span data-ttu-id="54895-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="54895-138">DateTime the object was last modified.</span></span> <span data-ttu-id="54895-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54895-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54895-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="54895-140">roleScopeTagIds</span></span>|<span data-ttu-id="54895-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="54895-141">String collection</span></span>|<span data-ttu-id="54895-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="54895-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="54895-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54895-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54895-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="54895-144">supportsScopeTags</span></span>|<span data-ttu-id="54895-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="54895-145">Boolean</span></span>|<span data-ttu-id="54895-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="54895-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="54895-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="54895-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="54895-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="54895-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="54895-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54895-149">This property is read-only.</span></span> <span data-ttu-id="54895-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54895-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54895-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="54895-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="54895-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="54895-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="54895-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="54895-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="54895-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54895-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54895-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="54895-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="54895-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="54895-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="54895-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="54895-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="54895-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54895-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54895-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="54895-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="54895-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="54895-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="54895-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="54895-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="54895-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54895-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54895-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54895-163">createdDateTime</span></span>|<span data-ttu-id="54895-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54895-164">DateTimeOffset</span></span>|<span data-ttu-id="54895-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="54895-165">DateTime the object was created.</span></span> <span data-ttu-id="54895-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54895-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54895-167">descrição</span><span class="sxs-lookup"><span data-stu-id="54895-167">description</span></span>|<span data-ttu-id="54895-168">String</span><span class="sxs-lookup"><span data-stu-id="54895-168">String</span></span>|<span data-ttu-id="54895-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54895-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="54895-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54895-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54895-171">displayName</span><span class="sxs-lookup"><span data-stu-id="54895-171">displayName</span></span>|<span data-ttu-id="54895-172">String</span><span class="sxs-lookup"><span data-stu-id="54895-172">String</span></span>|<span data-ttu-id="54895-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54895-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="54895-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54895-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54895-175">versão</span><span class="sxs-lookup"><span data-stu-id="54895-175">version</span></span>|<span data-ttu-id="54895-176">Int32</span><span class="sxs-lookup"><span data-stu-id="54895-176">Int32</span></span>|<span data-ttu-id="54895-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="54895-177">Version of the device configuration.</span></span> <span data-ttu-id="54895-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54895-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54895-179">NetworkName</span><span class="sxs-lookup"><span data-stu-id="54895-179">networkName</span></span>|<span data-ttu-id="54895-180">String</span><span class="sxs-lookup"><span data-stu-id="54895-180">String</span></span>|<span data-ttu-id="54895-181">Nome da rede herdado de [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54895-181">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="54895-182">SSID</span><span class="sxs-lookup"><span data-stu-id="54895-182">ssid</span></span>|<span data-ttu-id="54895-183">String</span><span class="sxs-lookup"><span data-stu-id="54895-183">String</span></span>|<span data-ttu-id="54895-184">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="54895-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="54895-185">Herdado de [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54895-185">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="54895-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="54895-186">connectAutomatically</span></span>|<span data-ttu-id="54895-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="54895-187">Boolean</span></span>|<span data-ttu-id="54895-188">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="54895-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="54895-189">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="54895-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="54895-190">Herdado de [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54895-190">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="54895-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="54895-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="54895-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="54895-192">Boolean</span></span>|<span data-ttu-id="54895-193">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="54895-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="54895-194">Herdado de [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54895-194">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="54895-195">à</span><span class="sxs-lookup"><span data-stu-id="54895-195">wiFiSecurityType</span></span>|[<span data-ttu-id="54895-196">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="54895-196">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="54895-197">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="54895-197">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="54895-198">Herdado de [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54895-198">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="54895-199">Os valores possíveis são: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="54895-199">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="54895-200">eapType</span><span class="sxs-lookup"><span data-stu-id="54895-200">eapType</span></span>|[<span data-ttu-id="54895-201">androidEapType</span><span class="sxs-lookup"><span data-stu-id="54895-201">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="54895-202">Indica o tipo de protocolo EAP definido no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="54895-202">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="54895-203">Os valores possíveis são: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="54895-203">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="54895-204">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="54895-204">authenticationMethod</span></span>|[<span data-ttu-id="54895-205">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="54895-205">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="54895-206">Indica o método de autenticação que o cliente (dispositivo) precisa usar quando o tipo EAP é configurado como PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="54895-206">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="54895-207">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="54895-207">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="54895-208">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="54895-208">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="54895-209">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="54895-209">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="54895-210">Método não EAP para autenticação (identidade interna) quando o tipo EAP é EAP-TTLS e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="54895-210">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="54895-211">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="54895-211">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="54895-212">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="54895-212">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="54895-213">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="54895-213">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="54895-214">Método não EAP para autenticação (identidade interna) quando o tipo EAP é PEAP e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="54895-214">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="54895-215">Os valores possíveis são: `none` e `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="54895-215">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="54895-216">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="54895-216">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="54895-217">String</span><span class="sxs-lookup"><span data-stu-id="54895-217">String</span></span>|<span data-ttu-id="54895-218">Habilitar Privacidade de identidade (identidade externa) quando o tipo EAP é configurado como EAP-TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="54895-218">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="54895-219">A cadeia de caracteres fornecida aqui é usada para mascarar o nome de usuário de usuários individuais quando eles tentam se conectar à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="54895-219">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="54895-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="54895-220">Response</span></span>
<span data-ttu-id="54895-221">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54895-221">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54895-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54895-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="54895-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54895-223">Request</span></span>
<span data-ttu-id="54895-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54895-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1549

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="54895-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="54895-225">Response</span></span>
<span data-ttu-id="54895-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54895-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1721

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
  "id": "c48cd726-d726-c48c-26d7-8cc426d78cc4",
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






