---
title: Criar Androidenterprisewificonfiguration.
description: Criar um novo objeto Androidenterprisewificonfiguration..
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 466d5526682ab11dd2e8da7e1fcf1f3c8fddcc72
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166679"
---
# <a name="create-androidenterprisewificonfiguration"></a><span data-ttu-id="f2220-103">Criar Androidenterprisewificonfiguration.</span><span class="sxs-lookup"><span data-stu-id="f2220-103">Create androidEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="f2220-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2220-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2220-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2220-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2220-106">Criar um novo objeto [androidenterprisewificonfiguration.](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f2220-106">Create a new [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2220-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2220-107">Prerequisites</span></span>
<span data-ttu-id="f2220-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f2220-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f2220-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2220-110">Permission type</span></span>|<span data-ttu-id="f2220-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2220-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2220-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2220-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f2220-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2220-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f2220-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2220-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2220-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2220-115">Not supported.</span></span>|
|<span data-ttu-id="f2220-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2220-116">Application</span></span>|<span data-ttu-id="f2220-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2220-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2220-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2220-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f2220-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2220-119">Request headers</span></span>
|<span data-ttu-id="f2220-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2220-120">Header</span></span>|<span data-ttu-id="f2220-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f2220-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2220-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2220-122">Authorization</span></span>|<span data-ttu-id="f2220-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2220-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2220-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2220-124">Accept</span></span>|<span data-ttu-id="f2220-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f2220-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2220-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2220-126">Request body</span></span>
<span data-ttu-id="f2220-127">No corpo da solicitação, forneça uma representação JSON do objeto Androidenterprisewificonfiguration..</span><span class="sxs-lookup"><span data-stu-id="f2220-127">In the request body, supply a JSON representation for the androidEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="f2220-128">A tabela a seguir mostra as propriedades que são necessárias ao criar Androidenterprisewificonfiguration..</span><span class="sxs-lookup"><span data-stu-id="f2220-128">The following table shows the properties that are required when you create the androidEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="f2220-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2220-129">Property</span></span>|<span data-ttu-id="f2220-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2220-130">Type</span></span>|<span data-ttu-id="f2220-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2220-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2220-132">id</span><span class="sxs-lookup"><span data-stu-id="f2220-132">id</span></span>|<span data-ttu-id="f2220-133">String</span><span class="sxs-lookup"><span data-stu-id="f2220-133">String</span></span>|<span data-ttu-id="f2220-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f2220-134">Key of the entity.</span></span> <span data-ttu-id="f2220-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2220-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2220-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2220-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f2220-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2220-137">DateTimeOffset</span></span>|<span data-ttu-id="f2220-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f2220-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f2220-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2220-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2220-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f2220-140">roleScopeTagIds</span></span>|<span data-ttu-id="f2220-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2220-141">String collection</span></span>|<span data-ttu-id="f2220-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f2220-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f2220-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2220-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2220-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f2220-144">supportsScopeTags</span></span>|<span data-ttu-id="f2220-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2220-145">Boolean</span></span>|<span data-ttu-id="f2220-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f2220-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f2220-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f2220-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f2220-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f2220-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f2220-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2220-149">This property is read-only.</span></span> <span data-ttu-id="f2220-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2220-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2220-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2220-151">createdDateTime</span></span>|<span data-ttu-id="f2220-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2220-152">DateTimeOffset</span></span>|<span data-ttu-id="f2220-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f2220-153">DateTime the object was created.</span></span> <span data-ttu-id="f2220-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2220-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2220-155">description</span><span class="sxs-lookup"><span data-stu-id="f2220-155">description</span></span>|<span data-ttu-id="f2220-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2220-156">String</span></span>|<span data-ttu-id="f2220-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f2220-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f2220-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2220-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2220-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f2220-159">displayName</span></span>|<span data-ttu-id="f2220-160">String</span><span class="sxs-lookup"><span data-stu-id="f2220-160">String</span></span>|<span data-ttu-id="f2220-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f2220-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f2220-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2220-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2220-163">version</span><span class="sxs-lookup"><span data-stu-id="f2220-163">version</span></span>|<span data-ttu-id="f2220-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f2220-164">Int32</span></span>|<span data-ttu-id="f2220-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f2220-165">Version of the device configuration.</span></span> <span data-ttu-id="f2220-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2220-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2220-167">NetworkName</span><span class="sxs-lookup"><span data-stu-id="f2220-167">networkName</span></span>|<span data-ttu-id="f2220-168">String</span><span class="sxs-lookup"><span data-stu-id="f2220-168">String</span></span>|<span data-ttu-id="f2220-169">Nome da rede herdado de [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2220-169">Network Name Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="f2220-170">SSID</span><span class="sxs-lookup"><span data-stu-id="f2220-170">ssid</span></span>|<span data-ttu-id="f2220-171">String</span><span class="sxs-lookup"><span data-stu-id="f2220-171">String</span></span>|<span data-ttu-id="f2220-172">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f2220-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="f2220-173">Herdado de [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2220-173">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="f2220-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="f2220-174">connectAutomatically</span></span>|<span data-ttu-id="f2220-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2220-175">Boolean</span></span>|<span data-ttu-id="f2220-176">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="f2220-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="f2220-177">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f2220-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="f2220-178">Herdado de [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2220-178">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="f2220-179">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="f2220-179">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="f2220-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2220-180">Boolean</span></span>|<span data-ttu-id="f2220-181">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f2220-181">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="f2220-182">Herdado de [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2220-182">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)</span></span>|
|<span data-ttu-id="f2220-183">à</span><span class="sxs-lookup"><span data-stu-id="f2220-183">wiFiSecurityType</span></span>|[<span data-ttu-id="f2220-184">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="f2220-184">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="f2220-185">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="f2220-185">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="f2220-186">Herdado de [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2220-186">Inherited from [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md).</span></span> <span data-ttu-id="f2220-187">Os valores possíveis são: `open` e `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="f2220-187">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="f2220-188">eapType</span><span class="sxs-lookup"><span data-stu-id="f2220-188">eapType</span></span>|[<span data-ttu-id="f2220-189">androidEapType</span><span class="sxs-lookup"><span data-stu-id="f2220-189">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="f2220-190">Indica o tipo de protocolo EAP definido no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="f2220-190">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="f2220-191">Os valores possíveis são: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="f2220-191">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="f2220-192">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f2220-192">authenticationMethod</span></span>|[<span data-ttu-id="f2220-193">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f2220-193">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="f2220-194">Indica o método de autenticação que o cliente (dispositivo) precisa usar quando o tipo EAP é configurado como PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="f2220-194">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="f2220-195">Os valores possíveis são: `certificate` e `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="f2220-195">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="f2220-196">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="f2220-196">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="f2220-197">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="f2220-197">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="f2220-198">Método não EAP para autenticação (identidade interna) quando o tipo EAP é EAP-TTLS e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="f2220-198">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="f2220-199">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="f2220-199">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="f2220-200">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="f2220-200">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="f2220-201">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="f2220-201">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="f2220-202">Método não EAP para autenticação (identidade interna) quando o tipo EAP é PEAP e AuthenticationMethod é username e password.</span><span class="sxs-lookup"><span data-stu-id="f2220-202">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="f2220-203">Os valores possíveis são: `none` e `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="f2220-203">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="f2220-204">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="f2220-204">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="f2220-205">String</span><span class="sxs-lookup"><span data-stu-id="f2220-205">String</span></span>|<span data-ttu-id="f2220-206">Habilitar Privacidade de identidade (identidade externa) quando o tipo EAP é configurado como EAP-TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="f2220-206">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="f2220-207">A cadeia de caracteres fornecida aqui é usada para mascarar o nome de usuário de usuários individuais quando eles tentam se conectar à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f2220-207">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="f2220-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2220-208">Response</span></span>
<span data-ttu-id="f2220-209">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidenterprisewificonfiguration.](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2220-209">If successful, this method returns a `201 Created` response code and a [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2220-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2220-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2220-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2220-211">Request</span></span>
<span data-ttu-id="f2220-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2220-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 765

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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="f2220-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2220-213">Response</span></span>
<span data-ttu-id="f2220-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2220-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 937

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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




