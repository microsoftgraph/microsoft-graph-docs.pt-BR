---
title: Criar androidForWorkEnterpriseWiFiConfiguration
description: Crie um novo objeto de androidForWorkEnterpriseWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 00c1e8a14fa838c5042196023dfc52f7fafde19d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853729"
---
# <a name="create-androidforworkenterprisewificonfiguration"></a><span data-ttu-id="8fac4-103">Criar androidForWorkEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="8fac4-103">Create androidForWorkEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="8fac4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8fac4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8fac4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8fac4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8fac4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8fac4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fac4-107">Crie um novo objeto de [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8fac4-107">Create a new [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8fac4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8fac4-108">Prerequisites</span></span>
<span data-ttu-id="8fac4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fac4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fac4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8fac4-111">Permission type</span></span>|<span data-ttu-id="8fac4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8fac4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fac4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8fac4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8fac4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fac4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8fac4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8fac4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fac4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fac4-116">Not supported.</span></span>|
|<span data-ttu-id="8fac4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8fac4-117">Application</span></span>|<span data-ttu-id="8fac4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fac4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fac4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fac4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8fac4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8fac4-120">Request headers</span></span>
|<span data-ttu-id="8fac4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8fac4-121">Header</span></span>|<span data-ttu-id="8fac4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8fac4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fac4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8fac4-123">Authorization</span></span>|<span data-ttu-id="8fac4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8fac4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fac4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8fac4-125">Accept</span></span>|<span data-ttu-id="8fac4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8fac4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fac4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8fac4-127">Request body</span></span>
<span data-ttu-id="8fac4-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8fac4-128">In the request body, supply a JSON representation for the androidForWorkEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="8fac4-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidForWorkEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8fac4-129">The following table shows the properties that are required when you create the androidForWorkEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="8fac4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8fac4-130">Property</span></span>|<span data-ttu-id="8fac4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8fac4-131">Type</span></span>|<span data-ttu-id="8fac4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fac4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fac4-133">id</span><span class="sxs-lookup"><span data-stu-id="8fac4-133">id</span></span>|<span data-ttu-id="8fac4-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8fac4-134">String</span></span>|<span data-ttu-id="8fac4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8fac4-135">Key of the entity.</span></span> <span data-ttu-id="8fac4-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fac4-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fac4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fac4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8fac4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fac4-138">DateTimeOffset</span></span>|<span data-ttu-id="8fac4-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8fac4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8fac4-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fac4-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fac4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8fac4-141">roleScopeTagIds</span></span>|<span data-ttu-id="8fac4-142">String collection</span><span class="sxs-lookup"><span data-stu-id="8fac4-142">String collection</span></span>|<span data-ttu-id="8fac4-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="8fac4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8fac4-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fac4-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fac4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8fac4-145">supportsScopeTags</span></span>|<span data-ttu-id="8fac4-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="8fac4-146">Boolean</span></span>|<span data-ttu-id="8fac4-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="8fac4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8fac4-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="8fac4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8fac4-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="8fac4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8fac4-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8fac4-150">This property is read-only.</span></span> <span data-ttu-id="8fac4-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fac4-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fac4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8fac4-152">createdDateTime</span></span>|<span data-ttu-id="8fac4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fac4-153">DateTimeOffset</span></span>|<span data-ttu-id="8fac4-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8fac4-154">DateTime the object was created.</span></span> <span data-ttu-id="8fac4-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fac4-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fac4-156">description</span><span class="sxs-lookup"><span data-stu-id="8fac4-156">description</span></span>|<span data-ttu-id="8fac4-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8fac4-157">String</span></span>|<span data-ttu-id="8fac4-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8fac4-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8fac4-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fac4-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fac4-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8fac4-160">displayName</span></span>|<span data-ttu-id="8fac4-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8fac4-161">String</span></span>|<span data-ttu-id="8fac4-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8fac4-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8fac4-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fac4-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fac4-164">version</span><span class="sxs-lookup"><span data-stu-id="8fac4-164">version</span></span>|<span data-ttu-id="8fac4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8fac4-165">Int32</span></span>|<span data-ttu-id="8fac4-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8fac4-166">Version of the device configuration.</span></span> <span data-ttu-id="8fac4-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fac4-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fac4-168">networkName</span><span class="sxs-lookup"><span data-stu-id="8fac4-168">networkName</span></span>|<span data-ttu-id="8fac4-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8fac4-169">String</span></span>|<span data-ttu-id="8fac4-170">Herdado de nome de rede de [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fac4-170">Network Name Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="8fac4-171">SSID</span><span class="sxs-lookup"><span data-stu-id="8fac4-171">ssid</span></span>|<span data-ttu-id="8fac4-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8fac4-172">String</span></span>|<span data-ttu-id="8fac4-173">Este é o nome da rede Wi-Fi que é difundido para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8fac4-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="8fac4-174">Herdado de [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fac4-174">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="8fac4-175">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="8fac4-175">connectAutomatically</span></span>|<span data-ttu-id="8fac4-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="8fac4-176">Boolean</span></span>|<span data-ttu-id="8fac4-177">Conecte automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="8fac4-177">Connect automatically when this network is in range.</span></span> <span data-ttu-id="8fac4-178">Essa configuração como true ignorar o prompt do usuário e se conecte automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="8fac4-178">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="8fac4-179">Herdado de [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fac4-179">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="8fac4-180">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="8fac4-180">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="8fac4-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="8fac4-181">Boolean</span></span>|<span data-ttu-id="8fac4-182">Quando definido como true, esse perfil força o dispositivo para se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8fac4-182">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="8fac4-183">Herdado de [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fac4-183">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="8fac4-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="8fac4-184">wiFiSecurityType</span></span>|[<span data-ttu-id="8fac4-185">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="8fac4-185">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="8fac4-186">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseada em EAP.</span><span class="sxs-lookup"><span data-stu-id="8fac4-186">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="8fac4-187">Herdada do [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8fac4-187">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span> <span data-ttu-id="8fac4-188">Os valores possíveis são: `open` e `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="8fac4-188">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="8fac4-189">eapType</span><span class="sxs-lookup"><span data-stu-id="8fac4-189">eapType</span></span>|[<span data-ttu-id="8fac4-190">androidEapType</span><span class="sxs-lookup"><span data-stu-id="8fac4-190">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="8fac4-191">Indica o tipo de protocolo EAP definir no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="8fac4-191">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="8fac4-192">Os valores possíveis são: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="8fac4-192">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="8fac4-193">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8fac4-193">authenticationMethod</span></span>|[<span data-ttu-id="8fac4-194">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8fac4-194">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="8fac4-195">Indica o método de autenticação, o cliente (dispositivo) precisa usar quando o tipo de EAP é configurado para PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="8fac4-195">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="8fac4-196">Os valores possíveis são: `certificate` e `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="8fac4-196">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="8fac4-197">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="8fac4-197">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="8fac4-198">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="8fac4-198">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="8fac4-199">Método de não-EAP para autenticação (identidade Inner) quando o tipo de EAP é EAP-TTLS e Authenticationmethod é Username e Password.</span><span class="sxs-lookup"><span data-stu-id="8fac4-199">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="8fac4-200">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="8fac4-200">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="8fac4-201">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="8fac4-201">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="8fac4-202">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="8fac4-202">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="8fac4-203">Método de não-EAP para autenticação (identidade Inner) quando o tipo de EAP é PEAP e Authenticationmethod é Username e Password.</span><span class="sxs-lookup"><span data-stu-id="8fac4-203">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="8fac4-204">Os valores possíveis são: `none` e `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="8fac4-204">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="8fac4-205">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="8fac4-205">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="8fac4-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8fac4-206">String</span></span>|<span data-ttu-id="8fac4-207">Habilite privacidade de identidade (identidade externa) quando o tipo de EAP é configurado para EAP-TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="8fac4-207">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="8fac4-208">A cadeia de caracteres fornecida aqui é usada para o nome de usuário de usuários individuais de máscara quando eles tentam se conectar à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="8fac4-208">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="8fac4-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fac4-209">Response</span></span>
<span data-ttu-id="8fac4-210">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8fac4-210">If successful, this method returns a `201 Created` response code and a [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fac4-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8fac4-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="8fac4-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8fac4-212">Request</span></span>
<span data-ttu-id="8fac4-213">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8fac4-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 836

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="8fac4-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fac4-214">Response</span></span>
<span data-ttu-id="8fac4-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8fac4-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 944

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
  "id": "742d953a-953a-742d-3a95-2d743a952d74",
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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```





