---
title: Criar Androidenterprisewificonfiguration.
description: Criar um novo objeto Androidenterprisewificonfiguration..
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b590051c886fd41cecd9f1ad7e04145516016ff6
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534691"
---
# <a name="create-androidenterprisewificonfiguration"></a><span data-ttu-id="91f23-103">Criar Androidenterprisewificonfiguration.</span><span class="sxs-lookup"><span data-stu-id="91f23-103">Create androidEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="91f23-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="91f23-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91f23-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91f23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91f23-106">Criar um novo objeto [androidenterprisewificonfiguration.](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="91f23-106">Create a new [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91f23-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91f23-107">Prerequisites</span></span>
<span data-ttu-id="91f23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91f23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91f23-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91f23-110">Permission type</span></span>|<span data-ttu-id="91f23-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="91f23-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91f23-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91f23-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91f23-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91f23-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="91f23-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91f23-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91f23-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91f23-115">Not supported.</span></span>|
|<span data-ttu-id="91f23-116">Application</span><span class="sxs-lookup"><span data-stu-id="91f23-116">Application</span></span>|<span data-ttu-id="91f23-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91f23-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91f23-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91f23-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="91f23-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91f23-119">Request headers</span></span>
|<span data-ttu-id="91f23-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91f23-120">Header</span></span>|<span data-ttu-id="91f23-121">Valor</span><span class="sxs-lookup"><span data-stu-id="91f23-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91f23-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="91f23-122">Authorization</span></span>|<span data-ttu-id="91f23-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91f23-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91f23-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="91f23-124">Accept</span></span>|<span data-ttu-id="91f23-125">application/json</span><span class="sxs-lookup"><span data-stu-id="91f23-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91f23-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91f23-126">Request body</span></span>
<span data-ttu-id="91f23-127">No corpo da solicitação, forneça uma representação JSON do objeto Androidenterprisewificonfiguration..</span><span class="sxs-lookup"><span data-stu-id="91f23-127">In the request body, supply a JSON representation for the androidEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="91f23-128">A tabela a seguir mostra as propriedades que são necessárias ao criar Androidenterprisewificonfiguration..</span><span class="sxs-lookup"><span data-stu-id="91f23-128">The following table shows the properties that are required when you create the androidEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="91f23-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91f23-129">Property</span></span>|<span data-ttu-id="91f23-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="91f23-130">Type</span></span>|<span data-ttu-id="91f23-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="91f23-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91f23-132">id</span><span class="sxs-lookup"><span data-stu-id="91f23-132">id</span></span>|<span data-ttu-id="91f23-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91f23-133">String</span></span>|<span data-ttu-id="91f23-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="91f23-134">Key of the entity.</span></span> <span data-ttu-id="91f23-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f23-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f23-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91f23-136">lastModifiedDateTime</span></span>|<span data-ttu-id="91f23-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91f23-137">DateTimeOffset</span></span>|<span data-ttu-id="91f23-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="91f23-138">DateTime the object was last modified.</span></span> <span data-ttu-id="91f23-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f23-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f23-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="91f23-140">roleScopeTagIds</span></span>|<span data-ttu-id="91f23-141">String collection</span><span class="sxs-lookup"><span data-stu-id="91f23-141">String collection</span></span>|<span data-ttu-id="91f23-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="91f23-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="91f23-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f23-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f23-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="91f23-144">supportsScopeTags</span></span>|<span data-ttu-id="91f23-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="91f23-145">Boolean</span></span>|<span data-ttu-id="91f23-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="91f23-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="91f23-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="91f23-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="91f23-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="91f23-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="91f23-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="91f23-149">This property is read-only.</span></span> <span data-ttu-id="91f23-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f23-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f23-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="91f23-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="91f23-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="91f23-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="91f23-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="91f23-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="91f23-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f23-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f23-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="91f23-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="91f23-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="91f23-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="91f23-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="91f23-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="91f23-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f23-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f23-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="91f23-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="91f23-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="91f23-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="91f23-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="91f23-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="91f23-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f23-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f23-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91f23-163">createdDateTime</span></span>|<span data-ttu-id="91f23-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91f23-164">DateTimeOffset</span></span>|<span data-ttu-id="91f23-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="91f23-165">DateTime the object was created.</span></span> <span data-ttu-id="91f23-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f23-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f23-167">description</span><span class="sxs-lookup"><span data-stu-id="91f23-167">description</span></span>|<span data-ttu-id="91f23-168">String</span><span class="sxs-lookup"><span data-stu-id="91f23-168">String</span></span>|<span data-ttu-id="91f23-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="91f23-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="91f23-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f23-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f23-171">displayName</span><span class="sxs-lookup"><span data-stu-id="91f23-171">displayName</span></span>|<span data-ttu-id="91f23-172">String</span><span class="sxs-lookup"><span data-stu-id="91f23-172">String</span></span>|<span data-ttu-id="91f23-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="91f23-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="91f23-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f23-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f23-175">versão</span><span class="sxs-lookup"><span data-stu-id="91f23-175">version</span></span>|<span data-ttu-id="91f23-176">Int32</span><span class="sxs-lookup"><span data-stu-id="91f23-176">Int32</span></span>|<span data-ttu-id="91f23-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="91f23-177">Version of the device configuration.</span></span> <span data-ttu-id="91f23-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f23-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f23-179">NetworkName</span><span class="sxs-lookup"><span data-stu-id="91f23-179">networkName</span></span>|<span data-ttu-id="91f23-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91f23-180">String</span></span>|<span data-ttu-id="91f23-181">Nome da rede herdado de [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f23-181">Network Name Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="91f23-182">SSID</span><span class="sxs-lookup"><span data-stu-id="91f23-182">ssid</span></span>|<span data-ttu-id="91f23-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91f23-183">String</span></span>|<span data-ttu-id="91f23-184">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="91f23-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="91f23-185">Herdado de [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f23-185">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="91f23-186">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="91f23-186">connectAutomatically</span></span>|<span data-ttu-id="91f23-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="91f23-187">Boolean</span></span>|<span data-ttu-id="91f23-188">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="91f23-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="91f23-189">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="91f23-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="91f23-190">Herdado de [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f23-190">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="91f23-191">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="91f23-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="91f23-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="91f23-192">Boolean</span></span>|<span data-ttu-id="91f23-193">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="91f23-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="91f23-194">Herdado de [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f23-194">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="91f23-195">à</span><span class="sxs-lookup"><span data-stu-id="91f23-195">wiFiSecurityType</span></span>|[<span data-ttu-id="91f23-196">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="91f23-196">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="91f23-197">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="91f23-197">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="91f23-198">Herdado de [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91f23-198">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span> <span data-ttu-id="91f23-199">Os valores possíveis são: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="91f23-199">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="91f23-200">eapType</span><span class="sxs-lookup"><span data-stu-id="91f23-200">eapType</span></span>|[<span data-ttu-id="91f23-201">androidEapType</span><span class="sxs-lookup"><span data-stu-id="91f23-201">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="91f23-202">Indica o tipo de protocolo EAP definido no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="91f23-202">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="91f23-203">Os valores possíveis são: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="91f23-203">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="91f23-204">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="91f23-204">authenticationMethod</span></span>|[<span data-ttu-id="91f23-205">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="91f23-205">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="91f23-206">Indica o método de autenticação que o cliente (dispositivo) precisa usar quando o tipo EAP é configurado como PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="91f23-206">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="91f23-207">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="91f23-207">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="91f23-208">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="91f23-208">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="91f23-209">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="91f23-209">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="91f23-210">Método não EAP para autenticação (identidade interna) quando o tipo EAP é EAP-TTLS e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="91f23-210">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="91f23-211">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="91f23-211">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="91f23-212">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="91f23-212">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="91f23-213">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="91f23-213">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="91f23-214">Método não EAP para autenticação (identidade interna) quando o tipo EAP é PEAP e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="91f23-214">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="91f23-215">Os valores possíveis são: `none` e `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="91f23-215">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="91f23-216">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="91f23-216">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="91f23-217">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91f23-217">String</span></span>|<span data-ttu-id="91f23-218">Habilitar Privacidade de identidade (identidade externa) quando o tipo EAP é configurado como EAP-TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="91f23-218">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="91f23-219">A cadeia de caracteres fornecida aqui é usada para mascarar o nome de usuário de usuários individuais quando eles tentam se conectar à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="91f23-219">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|
|<span data-ttu-id="91f23-220">usernameFormatString</span><span class="sxs-lookup"><span data-stu-id="91f23-220">usernameFormatString</span></span>|<span data-ttu-id="91f23-221">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91f23-221">String</span></span>|<span data-ttu-id="91f23-222">Cadeia de caracteres de formato de nome de usuário usada para criar o nome de usuário para se conectar</span><span class="sxs-lookup"><span data-stu-id="91f23-222">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="91f23-223">passwordFormatString</span><span class="sxs-lookup"><span data-stu-id="91f23-223">passwordFormatString</span></span>|<span data-ttu-id="91f23-224">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91f23-224">String</span></span>|<span data-ttu-id="91f23-225">Cadeia de caracteres de formato de senha usada para criar a senha para se conectar ao wifi</span><span class="sxs-lookup"><span data-stu-id="91f23-225">Password format string used to build the password to connect to wifi</span></span>|
|<span data-ttu-id="91f23-226">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="91f23-226">preSharedKey</span></span>|<span data-ttu-id="91f23-227">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91f23-227">String</span></span>|<span data-ttu-id="91f23-228">PreSharedKey usado para criar a senha para se conectar ao wifi</span><span class="sxs-lookup"><span data-stu-id="91f23-228">PreSharedKey used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="91f23-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="91f23-229">Response</span></span>
<span data-ttu-id="91f23-230">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidenterprisewificonfiguration.](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91f23-230">If successful, this method returns a `201 Created` response code and a [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91f23-231">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91f23-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="91f23-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91f23-232">Request</span></span>
<span data-ttu-id="91f23-233">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91f23-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1699

{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
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
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value",
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="91f23-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="91f23-234">Response</span></span>
<span data-ttu-id="91f23-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91f23-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1871

{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
  "id": "972edff4-dff4-972e-f4df-2e97f4df2e97",
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
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value",
  "preSharedKey": "Pre Shared Key value"
}
```






