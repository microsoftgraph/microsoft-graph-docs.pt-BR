---
title: Atualizar androidForWorkEnterpriseWiFiConfiguration
description: Atualize as propriedades de um objeto androidForWorkEnterpriseWiFiConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2372183bb9ea8d31a65c8d1bbbf614ddb9cd421d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417984"
---
# <a name="update-androidforworkenterprisewificonfiguration"></a><span data-ttu-id="b0fb7-103">Atualizar androidForWorkEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0fb7-103">Update androidForWorkEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="b0fb7-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b0fb7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0fb7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0fb7-107">Atualize as propriedades de um objeto [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b0fb7-107">Update the properties of a [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0fb7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0fb7-108">Prerequisites</span></span>
<span data-ttu-id="b0fb7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b0fb7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b0fb7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0fb7-111">Permission type</span></span>|<span data-ttu-id="b0fb7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0fb7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0fb7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0fb7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0fb7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0fb7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0fb7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0fb7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0fb7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-116">Not supported.</span></span>|
|<span data-ttu-id="b0fb7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0fb7-117">Application</span></span>|<span data-ttu-id="b0fb7-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0fb7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0fb7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b0fb7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0fb7-120">Request headers</span></span>
|<span data-ttu-id="b0fb7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0fb7-121">Header</span></span>|<span data-ttu-id="b0fb7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b0fb7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0fb7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0fb7-123">Authorization</span></span>|<span data-ttu-id="b0fb7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0fb7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b0fb7-125">Accept</span></span>|<span data-ttu-id="b0fb7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0fb7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0fb7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0fb7-127">Request body</span></span>
<span data-ttu-id="b0fb7-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b0fb7-128">In the request body, supply a JSON representation for the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="b0fb7-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0fb7-129">The following table shows the properties that are required when you create the [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="b0fb7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0fb7-130">Property</span></span>|<span data-ttu-id="b0fb7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0fb7-131">Type</span></span>|<span data-ttu-id="b0fb7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0fb7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0fb7-133">id</span><span class="sxs-lookup"><span data-stu-id="b0fb7-133">id</span></span>|<span data-ttu-id="b0fb7-134">String</span><span class="sxs-lookup"><span data-stu-id="b0fb7-134">String</span></span>|<span data-ttu-id="b0fb7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-135">Key of the entity.</span></span> <span data-ttu-id="b0fb7-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0fb7-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0fb7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0fb7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b0fb7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0fb7-138">DateTimeOffset</span></span>|<span data-ttu-id="b0fb7-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b0fb7-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0fb7-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0fb7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b0fb7-141">roleScopeTagIds</span></span>|<span data-ttu-id="b0fb7-142">String collection</span><span class="sxs-lookup"><span data-stu-id="b0fb7-142">String collection</span></span>|<span data-ttu-id="b0fb7-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b0fb7-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0fb7-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0fb7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b0fb7-145">supportsScopeTags</span></span>|<span data-ttu-id="b0fb7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0fb7-146">Boolean</span></span>|<span data-ttu-id="b0fb7-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b0fb7-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b0fb7-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b0fb7-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-150">This property is read-only.</span></span> <span data-ttu-id="b0fb7-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0fb7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0fb7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0fb7-152">createdDateTime</span></span>|<span data-ttu-id="b0fb7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0fb7-153">DateTimeOffset</span></span>|<span data-ttu-id="b0fb7-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-154">DateTime the object was created.</span></span> <span data-ttu-id="b0fb7-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0fb7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0fb7-156">description</span><span class="sxs-lookup"><span data-stu-id="b0fb7-156">description</span></span>|<span data-ttu-id="b0fb7-157">String</span><span class="sxs-lookup"><span data-stu-id="b0fb7-157">String</span></span>|<span data-ttu-id="b0fb7-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b0fb7-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0fb7-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0fb7-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b0fb7-160">displayName</span></span>|<span data-ttu-id="b0fb7-161">String</span><span class="sxs-lookup"><span data-stu-id="b0fb7-161">String</span></span>|<span data-ttu-id="b0fb7-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b0fb7-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0fb7-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0fb7-164">version</span><span class="sxs-lookup"><span data-stu-id="b0fb7-164">version</span></span>|<span data-ttu-id="b0fb7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b0fb7-165">Int32</span></span>|<span data-ttu-id="b0fb7-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-166">Version of the device configuration.</span></span> <span data-ttu-id="b0fb7-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0fb7-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0fb7-168">networkName</span><span class="sxs-lookup"><span data-stu-id="b0fb7-168">networkName</span></span>|<span data-ttu-id="b0fb7-169">String</span><span class="sxs-lookup"><span data-stu-id="b0fb7-169">String</span></span>|<span data-ttu-id="b0fb7-170">Herdado de nome de rede de [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0fb7-170">Network Name Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="b0fb7-171">SSID</span><span class="sxs-lookup"><span data-stu-id="b0fb7-171">ssid</span></span>|<span data-ttu-id="b0fb7-172">String</span><span class="sxs-lookup"><span data-stu-id="b0fb7-172">String</span></span>|<span data-ttu-id="b0fb7-173">Este é o nome da rede Wi-Fi que é difundido para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="b0fb7-174">Herdado de [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0fb7-174">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="b0fb7-175">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="b0fb7-175">connectAutomatically</span></span>|<span data-ttu-id="b0fb7-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0fb7-176">Boolean</span></span>|<span data-ttu-id="b0fb7-177">Conecte automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-177">Connect automatically when this network is in range.</span></span> <span data-ttu-id="b0fb7-178">Essa configuração como true ignorar o prompt do usuário e se conecte automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-178">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="b0fb7-179">Herdado de [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0fb7-179">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="b0fb7-180">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="b0fb7-180">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="b0fb7-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0fb7-181">Boolean</span></span>|<span data-ttu-id="b0fb7-182">Quando definido como true, esse perfil força o dispositivo para se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-182">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="b0fb7-183">Herdado de [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0fb7-183">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)</span></span>|
|<span data-ttu-id="b0fb7-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b0fb7-184">wiFiSecurityType</span></span>|[<span data-ttu-id="b0fb7-185">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="b0fb7-185">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="b0fb7-186">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseada em EAP.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-186">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="b0fb7-187">Herdada do [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0fb7-187">Inherited from [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span> <span data-ttu-id="b0fb7-188">Os valores possíveis são: `open` e `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-188">Possible values are: `open`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="b0fb7-189">eapType</span><span class="sxs-lookup"><span data-stu-id="b0fb7-189">eapType</span></span>|[<span data-ttu-id="b0fb7-190">androidEapType</span><span class="sxs-lookup"><span data-stu-id="b0fb7-190">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="b0fb7-191">Indica o tipo de protocolo EAP definir no ponto de extremidade Wi-Fi (roteador).</span><span class="sxs-lookup"><span data-stu-id="b0fb7-191">Indicates the type of EAP protocol set on the the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="b0fb7-192">Os valores possíveis são: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-192">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="b0fb7-193">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b0fb7-193">authenticationMethod</span></span>|[<span data-ttu-id="b0fb7-194">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b0fb7-194">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="b0fb7-195">Indica o método de autenticação, o cliente (dispositivo) precisa usar quando o tipo de EAP é configurado para PEAP ou EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-195">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="b0fb7-196">Os valores possíveis são: `certificate` e `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-196">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="b0fb7-197">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="b0fb7-197">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="b0fb7-198">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="b0fb7-198">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="b0fb7-199">Método de não-EAP para autenticação (identidade Inner) quando o tipo de EAP é EAP-TTLS e Authenticationmethod é Username e Password.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-199">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="b0fb7-200">Os valores possíveis são: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-200">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="b0fb7-201">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="b0fb7-201">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="b0fb7-202">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="b0fb7-202">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="b0fb7-203">Método de não-EAP para autenticação (identidade Inner) quando o tipo de EAP é PEAP e Authenticationmethod é Username e Password.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-203">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="b0fb7-204">Os valores possíveis são: `none` e `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-204">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="b0fb7-205">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="b0fb7-205">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="b0fb7-206">String</span><span class="sxs-lookup"><span data-stu-id="b0fb7-206">String</span></span>|<span data-ttu-id="b0fb7-207">Habilite privacidade de identidade (identidade externa) quando o tipo de EAP é configurado para EAP-TTLS ou PEAP.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-207">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="b0fb7-208">A cadeia de caracteres fornecida aqui é usada para o nome de usuário de usuários individuais de máscara quando eles tentam se conectar à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-208">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="b0fb7-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0fb7-209">Response</span></span>
<span data-ttu-id="b0fb7-210">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-210">If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidforworkenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0fb7-211">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0fb7-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0fb7-212">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0fb7-212">Request</span></span>
<span data-ttu-id="b0fb7-213">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 772

{
  "@odata.type": "#microsoft.graph.androidForWorkEnterpriseWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="b0fb7-214">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0fb7-214">Response</span></span>
<span data-ttu-id="b0fb7-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0fb7-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




