---
title: Criar androidWorkProfileEnterpriseWiFiConfiguration
description: Criar um novo objeto androidWorkProfileEnterpriseWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e22a06f5dc3b0260df81648769a8b948a2bded79
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41635464"
---
# <a name="create-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="9ac85-103">Criar androidWorkProfileEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="9ac85-103">Create androidWorkProfileEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="9ac85-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ac85-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ac85-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ac85-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ac85-106">Criar um novo objeto [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9ac85-106">Create a new [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ac85-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ac85-107">Prerequisites</span></span>
<span data-ttu-id="9ac85-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ac85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ac85-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ac85-110">Permission type</span></span>|<span data-ttu-id="9ac85-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9ac85-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ac85-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ac85-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ac85-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ac85-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ac85-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ac85-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ac85-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ac85-115">Not supported.</span></span>|
|<span data-ttu-id="9ac85-116">Application</span><span class="sxs-lookup"><span data-stu-id="9ac85-116">Application</span></span>|<span data-ttu-id="9ac85-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ac85-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ac85-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ac85-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9ac85-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ac85-119">Request headers</span></span>
|<span data-ttu-id="9ac85-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ac85-120">Header</span></span>|<span data-ttu-id="9ac85-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9ac85-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ac85-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ac85-122">Authorization</span></span>|<span data-ttu-id="9ac85-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ac85-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ac85-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9ac85-124">Accept</span></span>|<span data-ttu-id="9ac85-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9ac85-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ac85-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ac85-126">Request body</span></span>
<span data-ttu-id="9ac85-127">No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfileEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9ac85-127">In the request body, supply a JSON representation for the androidWorkProfileEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="9ac85-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWorkProfileEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9ac85-128">The following table shows the properties that are required when you create the androidWorkProfileEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="9ac85-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ac85-129">Property</span></span>|<span data-ttu-id="9ac85-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ac85-130">Type</span></span>|<span data-ttu-id="9ac85-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ac85-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ac85-132">id</span><span class="sxs-lookup"><span data-stu-id="9ac85-132">id</span></span>|<span data-ttu-id="9ac85-133">String</span><span class="sxs-lookup"><span data-stu-id="9ac85-133">String</span></span>|<span data-ttu-id="9ac85-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9ac85-134">Key of the entity.</span></span> <span data-ttu-id="9ac85-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ac85-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac85-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ac85-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9ac85-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ac85-137">DateTimeOffset</span></span>|<span data-ttu-id="9ac85-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9ac85-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9ac85-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ac85-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac85-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ac85-140">roleScopeTagIds</span></span>|<span data-ttu-id="9ac85-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9ac85-141">String collection</span></span>|<span data-ttu-id="9ac85-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="9ac85-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9ac85-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ac85-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac85-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9ac85-144">supportsScopeTags</span></span>|<span data-ttu-id="9ac85-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ac85-145">Boolean</span></span>|<span data-ttu-id="9ac85-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9ac85-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9ac85-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9ac85-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9ac85-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9ac85-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9ac85-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ac85-149">This property is read-only.</span></span> <span data-ttu-id="9ac85-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ac85-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac85-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9ac85-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9ac85-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9ac85-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9ac85-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="9ac85-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9ac85-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ac85-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac85-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9ac85-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9ac85-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9ac85-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9ac85-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="9ac85-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9ac85-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ac85-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac85-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9ac85-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9ac85-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9ac85-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9ac85-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="9ac85-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9ac85-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ac85-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac85-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ac85-163">createdDateTime</span></span>|<span data-ttu-id="9ac85-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ac85-164">DateTimeOffset</span></span>|<span data-ttu-id="9ac85-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9ac85-165">DateTime the object was created.</span></span> <span data-ttu-id="9ac85-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ac85-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac85-167">description</span><span class="sxs-lookup"><span data-stu-id="9ac85-167">description</span></span>|<span data-ttu-id="9ac85-168">String</span><span class="sxs-lookup"><span data-stu-id="9ac85-168">String</span></span>|<span data-ttu-id="9ac85-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ac85-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9ac85-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ac85-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac85-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9ac85-171">displayName</span></span>|<span data-ttu-id="9ac85-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ac85-172">String</span></span>|<span data-ttu-id="9ac85-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ac85-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9ac85-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ac85-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac85-175">versão</span><span class="sxs-lookup"><span data-stu-id="9ac85-175">version</span></span>|<span data-ttu-id="9ac85-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9ac85-176">Int32</span></span>|<span data-ttu-id="9ac85-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ac85-177">Version of the device configuration.</span></span> <span data-ttu-id="9ac85-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ac85-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ac85-179">NetworkName</span><span class="sxs-lookup"><span data-stu-id="9ac85-179">networkName</span></span>|<span data-ttu-id="9ac85-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ac85-180">String</span></span>|<span data-ttu-id="9ac85-181">Nome da rede herdado de [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ac85-181">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="9ac85-182">SSID</span><span class="sxs-lookup"><span data-stu-id="9ac85-182">ssid</span></span>|<span data-ttu-id="9ac85-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ac85-183">String</span></span>|<span data-ttu-id="9ac85-184">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9ac85-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="9ac85-185">Herdado de [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ac85-185">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="9ac85-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="9ac85-186">connectAutomatically</span></span>|<span data-ttu-id="9ac85-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ac85-187">Boolean</span></span>|<span data-ttu-id="9ac85-188">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="9ac85-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="9ac85-189">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="9ac85-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="9ac85-190">Herdado de [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ac85-190">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="9ac85-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="9ac85-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="9ac85-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ac85-192">Boolean</span></span>|<span data-ttu-id="9ac85-193">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9ac85-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="9ac85-194">Herdado de [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ac85-194">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="9ac85-195">à</span><span class="sxs-lookup"><span data-stu-id="9ac85-195">wiFiSecurityType</span></span>|[<span data-ttu-id="9ac85-196">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="9ac85-196">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="9ac85-197">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="9ac85-197">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="9ac85-198">Herdado de [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ac85-198">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="9ac85-199">Os valores possíveis são: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="9ac85-199">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="9ac85-200">eapType</span><span class="sxs-lookup"><span data-stu-id="9ac85-200">eapType</span></span>|[<span data-ttu-id="9ac85-201">androidEapType</span><span class="sxs-lookup"><span data-stu-id="9ac85-201">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="9ac85-202">Indica o tipo de protocolo EAP definido no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="9ac85-202">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="9ac85-203">Os valores possíveis são: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="9ac85-203">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="9ac85-204">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9ac85-204">authenticationMethod</span></span>|[<span data-ttu-id="9ac85-205">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9ac85-205">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="9ac85-206">Indica o método de autenticação que o cliente (dispositivo) precisa usar quando o tipo EAP é configurado como PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="9ac85-206">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="9ac85-207">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="9ac85-207">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="9ac85-208">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="9ac85-208">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="9ac85-209">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="9ac85-209">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="9ac85-210">Método não EAP para autenticação (identidade interna) quando o tipo EAP é EAP-TTLS e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="9ac85-210">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="9ac85-211">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="9ac85-211">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="9ac85-212">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="9ac85-212">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="9ac85-213">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="9ac85-213">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="9ac85-214">Método não EAP para autenticação (identidade interna) quando o tipo EAP é PEAP e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="9ac85-214">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="9ac85-215">Os valores possíveis são: `none` e `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="9ac85-215">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="9ac85-216">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="9ac85-216">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="9ac85-217">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ac85-217">String</span></span>|<span data-ttu-id="9ac85-218">Habilitar Privacidade de identidade (identidade externa) quando o tipo EAP é configurado como EAP-TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="9ac85-218">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="9ac85-219">A cadeia de caracteres fornecida aqui é usada para mascarar o nome de usuário de usuários individuais quando eles tentam se conectar à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="9ac85-219">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|
|<span data-ttu-id="9ac85-220">proxySettings</span><span class="sxs-lookup"><span data-stu-id="9ac85-220">proxySettings</span></span>|[<span data-ttu-id="9ac85-221">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="9ac85-221">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="9ac85-222">Tipo de proxy para esta conexão Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="9ac85-222">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="9ac85-223">Os valores possíveis são: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="9ac85-223">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="9ac85-224">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="9ac85-224">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="9ac85-225">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ac85-225">String</span></span>|<span data-ttu-id="9ac85-226">URL do script de configuração automática do servidor proxy quando a configuração automática estiver selecionada.</span><span class="sxs-lookup"><span data-stu-id="9ac85-226">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="9ac85-227">Essa URL normalmente é o local do Arquivo PAC (configuração automática de proxy).</span><span class="sxs-lookup"><span data-stu-id="9ac85-227">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|



## <a name="response"></a><span data-ttu-id="9ac85-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ac85-228">Response</span></span>
<span data-ttu-id="9ac85-229">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ac85-229">If successful, this method returns a `201 Created` response code and a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ac85-230">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ac85-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ac85-231">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ac85-231">Request</span></span>
<span data-ttu-id="9ac85-232">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ac85-232">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1671

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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "proxySettings": "manual",
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/"
}
```

### <a name="response"></a><span data-ttu-id="9ac85-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ac85-233">Response</span></span>
<span data-ttu-id="9ac85-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ac85-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1843

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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "proxySettings": "manual",
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/"
}
```





