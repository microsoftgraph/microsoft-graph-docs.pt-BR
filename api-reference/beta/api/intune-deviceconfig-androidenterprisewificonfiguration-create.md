---
title: Criar Androidenterprisewificonfiguration.
description: Criar um novo objeto Androidenterprisewificonfiguration..
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12a06abcf8def4780f7f64d0f8a65d164938188f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933078"
---
# <a name="create-androidenterprisewificonfiguration"></a><span data-ttu-id="0db9e-103">Criar Androidenterprisewificonfiguration.</span><span class="sxs-lookup"><span data-stu-id="0db9e-103">Create androidEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="0db9e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0db9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0db9e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0db9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0db9e-106">Criar um novo objeto [androidenterprisewificonfiguration.](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0db9e-106">Create a new [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0db9e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0db9e-107">Prerequisites</span></span>
<span data-ttu-id="0db9e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0db9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0db9e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0db9e-110">Permission type</span></span>|<span data-ttu-id="0db9e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0db9e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0db9e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0db9e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0db9e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0db9e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0db9e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0db9e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0db9e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0db9e-115">Not supported.</span></span>|
|<span data-ttu-id="0db9e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0db9e-116">Application</span></span>|<span data-ttu-id="0db9e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0db9e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0db9e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0db9e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0db9e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0db9e-119">Request headers</span></span>
|<span data-ttu-id="0db9e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0db9e-120">Header</span></span>|<span data-ttu-id="0db9e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0db9e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0db9e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0db9e-122">Authorization</span></span>|<span data-ttu-id="0db9e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0db9e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0db9e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0db9e-124">Accept</span></span>|<span data-ttu-id="0db9e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0db9e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0db9e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0db9e-126">Request body</span></span>
<span data-ttu-id="0db9e-127">No corpo da solicitação, forneça uma representação JSON do objeto Androidenterprisewificonfiguration..</span><span class="sxs-lookup"><span data-stu-id="0db9e-127">In the request body, supply a JSON representation for the androidEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="0db9e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar Androidenterprisewificonfiguration..</span><span class="sxs-lookup"><span data-stu-id="0db9e-128">The following table shows the properties that are required when you create the androidEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="0db9e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0db9e-129">Property</span></span>|<span data-ttu-id="0db9e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0db9e-130">Type</span></span>|<span data-ttu-id="0db9e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0db9e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0db9e-132">id</span><span class="sxs-lookup"><span data-stu-id="0db9e-132">id</span></span>|<span data-ttu-id="0db9e-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0db9e-133">String</span></span>|<span data-ttu-id="0db9e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0db9e-134">Key of the entity.</span></span> <span data-ttu-id="0db9e-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0db9e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0db9e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0db9e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0db9e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0db9e-137">DateTimeOffset</span></span>|<span data-ttu-id="0db9e-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0db9e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0db9e-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0db9e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0db9e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0db9e-140">roleScopeTagIds</span></span>|<span data-ttu-id="0db9e-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0db9e-141">String collection</span></span>|<span data-ttu-id="0db9e-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0db9e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0db9e-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0db9e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0db9e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0db9e-144">supportsScopeTags</span></span>|<span data-ttu-id="0db9e-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="0db9e-145">Boolean</span></span>|<span data-ttu-id="0db9e-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0db9e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0db9e-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0db9e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0db9e-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0db9e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0db9e-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0db9e-149">This property is read-only.</span></span> <span data-ttu-id="0db9e-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0db9e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0db9e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0db9e-151">createdDateTime</span></span>|<span data-ttu-id="0db9e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0db9e-152">DateTimeOffset</span></span>|<span data-ttu-id="0db9e-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0db9e-153">DateTime the object was created.</span></span> <span data-ttu-id="0db9e-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0db9e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0db9e-155">description</span><span class="sxs-lookup"><span data-stu-id="0db9e-155">description</span></span>|<span data-ttu-id="0db9e-156">String</span><span class="sxs-lookup"><span data-stu-id="0db9e-156">String</span></span>|<span data-ttu-id="0db9e-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0db9e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0db9e-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0db9e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0db9e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="0db9e-159">displayName</span></span>|<span data-ttu-id="0db9e-160">String</span><span class="sxs-lookup"><span data-stu-id="0db9e-160">String</span></span>|<span data-ttu-id="0db9e-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0db9e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0db9e-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0db9e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0db9e-163">versão</span><span class="sxs-lookup"><span data-stu-id="0db9e-163">version</span></span>|<span data-ttu-id="0db9e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="0db9e-164">Int32</span></span>|<span data-ttu-id="0db9e-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0db9e-165">Version of the device configuration.</span></span> <span data-ttu-id="0db9e-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0db9e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0db9e-167">NetworkName</span><span class="sxs-lookup"><span data-stu-id="0db9e-167">networkName</span></span>|<span data-ttu-id="0db9e-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0db9e-168">String</span></span>|<span data-ttu-id="0db9e-169">Nome da rede herdado de [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0db9e-169">Network Name Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="0db9e-170">SSID</span><span class="sxs-lookup"><span data-stu-id="0db9e-170">ssid</span></span>|<span data-ttu-id="0db9e-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0db9e-171">String</span></span>|<span data-ttu-id="0db9e-172">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0db9e-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="0db9e-173">Herdado de [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0db9e-173">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="0db9e-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="0db9e-174">connectAutomatically</span></span>|<span data-ttu-id="0db9e-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="0db9e-175">Boolean</span></span>|<span data-ttu-id="0db9e-176">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="0db9e-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="0db9e-177">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="0db9e-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="0db9e-178">Herdado de [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0db9e-178">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="0db9e-179">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="0db9e-179">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="0db9e-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="0db9e-180">Boolean</span></span>|<span data-ttu-id="0db9e-181">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0db9e-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="0db9e-182">Herdado de [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0db9e-182">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="0db9e-183">à</span><span class="sxs-lookup"><span data-stu-id="0db9e-183">wiFiSecurityType</span></span>|[<span data-ttu-id="0db9e-184">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="0db9e-184">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="0db9e-185">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="0db9e-185">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="0db9e-186">Herdado de [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0db9e-186">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span> <span data-ttu-id="0db9e-187">Os valores possíveis são: `open` e `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="0db9e-187">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="0db9e-188">eapType</span><span class="sxs-lookup"><span data-stu-id="0db9e-188">eapType</span></span>|[<span data-ttu-id="0db9e-189">androidEapType</span><span class="sxs-lookup"><span data-stu-id="0db9e-189">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="0db9e-190">Indica o tipo de protocolo EAP definido no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="0db9e-190">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="0db9e-191">Os valores possíveis são: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="0db9e-191">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="0db9e-192">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0db9e-192">authenticationMethod</span></span>|[<span data-ttu-id="0db9e-193">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0db9e-193">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="0db9e-194">Indica o método de autenticação que o cliente (dispositivo) precisa usar quando o tipo EAP é configurado como PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="0db9e-194">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="0db9e-195">Os valores possíveis são: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="0db9e-195">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="0db9e-196">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="0db9e-196">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="0db9e-197">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="0db9e-197">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="0db9e-198">Método não EAP para autenticação (identidade interna) quando o tipo EAP é EAP-TTLS e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="0db9e-198">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="0db9e-199">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="0db9e-199">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="0db9e-200">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="0db9e-200">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="0db9e-201">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="0db9e-201">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="0db9e-202">Método não EAP para autenticação (identidade interna) quando o tipo EAP é PEAP e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="0db9e-202">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="0db9e-203">Os valores possíveis são: `none` e `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="0db9e-203">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="0db9e-204">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="0db9e-204">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="0db9e-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0db9e-205">String</span></span>|<span data-ttu-id="0db9e-206">Habilitar Privacidade de identidade (identidade externa) quando o tipo EAP é configurado como EAP-TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="0db9e-206">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="0db9e-207">A cadeia de caracteres fornecida aqui é usada para mascarar o nome de usuário de usuários individuais quando eles tentam se conectar à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="0db9e-207">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|
|<span data-ttu-id="0db9e-208">usernameFormatString</span><span class="sxs-lookup"><span data-stu-id="0db9e-208">usernameFormatString</span></span>|<span data-ttu-id="0db9e-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0db9e-209">String</span></span>|<span data-ttu-id="0db9e-210">Cadeia de caracteres de formato de nome de usuário usada para criar o nome de usuário para se conectar</span><span class="sxs-lookup"><span data-stu-id="0db9e-210">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="0db9e-211">passwordFormatString</span><span class="sxs-lookup"><span data-stu-id="0db9e-211">passwordFormatString</span></span>|<span data-ttu-id="0db9e-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0db9e-212">String</span></span>|<span data-ttu-id="0db9e-213">Cadeia de caracteres de formato de senha usada para criar a senha para se conectar ao wifi</span><span class="sxs-lookup"><span data-stu-id="0db9e-213">Password format string used to build the password to connect to wifi</span></span>|
|<span data-ttu-id="0db9e-214">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="0db9e-214">preSharedKey</span></span>|<span data-ttu-id="0db9e-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0db9e-215">String</span></span>|<span data-ttu-id="0db9e-216">PreSharedKey usado para criar a senha para se conectar ao wifi</span><span class="sxs-lookup"><span data-stu-id="0db9e-216">PreSharedKey used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="0db9e-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="0db9e-217">Response</span></span>
<span data-ttu-id="0db9e-218">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidenterprisewificonfiguration.](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0db9e-218">If successful, this method returns a `201 Created` response code and a [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0db9e-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0db9e-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="0db9e-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0db9e-220">Request</span></span>
<span data-ttu-id="0db9e-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0db9e-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 926

{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="0db9e-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="0db9e-222">Response</span></span>
<span data-ttu-id="0db9e-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0db9e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1098

{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
  "id": "972edff4-dff4-972e-f4df-2e97f4df2e97",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




