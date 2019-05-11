---
title: Criar windows10VpnConfiguration
description: Criar um novo objeto windows10VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 79231ff97883108fd8e01d491d2145ecd4f2f3d9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918385"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="88beb-103">Criar windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="88beb-103">Create windows10VpnConfiguration</span></span>

> <span data-ttu-id="88beb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88beb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88beb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88beb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88beb-106">Criar um novo objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="88beb-106">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88beb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="88beb-107">Prerequisites</span></span>
<span data-ttu-id="88beb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88beb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88beb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88beb-110">Permission type</span></span>|<span data-ttu-id="88beb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="88beb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88beb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88beb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88beb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88beb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88beb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88beb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88beb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88beb-115">Not supported.</span></span>|
|<span data-ttu-id="88beb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88beb-116">Application</span></span>|<span data-ttu-id="88beb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="88beb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88beb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88beb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="88beb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88beb-119">Request headers</span></span>
|<span data-ttu-id="88beb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="88beb-120">Header</span></span>|<span data-ttu-id="88beb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="88beb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88beb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="88beb-122">Authorization</span></span>|<span data-ttu-id="88beb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88beb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88beb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="88beb-124">Accept</span></span>|<span data-ttu-id="88beb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="88beb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88beb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88beb-126">Request body</span></span>
<span data-ttu-id="88beb-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="88beb-127">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="88beb-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="88beb-128">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="88beb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88beb-129">Property</span></span>|<span data-ttu-id="88beb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="88beb-130">Type</span></span>|<span data-ttu-id="88beb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="88beb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88beb-132">id</span><span class="sxs-lookup"><span data-stu-id="88beb-132">id</span></span>|<span data-ttu-id="88beb-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88beb-133">String</span></span>|<span data-ttu-id="88beb-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="88beb-134">Key of the entity.</span></span> <span data-ttu-id="88beb-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88beb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88beb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88beb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="88beb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88beb-137">DateTimeOffset</span></span>|<span data-ttu-id="88beb-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="88beb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="88beb-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88beb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88beb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="88beb-140">roleScopeTagIds</span></span>|<span data-ttu-id="88beb-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="88beb-141">String collection</span></span>|<span data-ttu-id="88beb-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="88beb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="88beb-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88beb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88beb-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="88beb-144">supportsScopeTags</span></span>|<span data-ttu-id="88beb-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="88beb-145">Boolean</span></span>|<span data-ttu-id="88beb-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="88beb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="88beb-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="88beb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="88beb-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="88beb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="88beb-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="88beb-149">This property is read-only.</span></span> <span data-ttu-id="88beb-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88beb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88beb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88beb-151">createdDateTime</span></span>|<span data-ttu-id="88beb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88beb-152">DateTimeOffset</span></span>|<span data-ttu-id="88beb-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="88beb-153">DateTime the object was created.</span></span> <span data-ttu-id="88beb-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88beb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88beb-155">description</span><span class="sxs-lookup"><span data-stu-id="88beb-155">description</span></span>|<span data-ttu-id="88beb-156">String</span><span class="sxs-lookup"><span data-stu-id="88beb-156">String</span></span>|<span data-ttu-id="88beb-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="88beb-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="88beb-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88beb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88beb-159">displayName</span><span class="sxs-lookup"><span data-stu-id="88beb-159">displayName</span></span>|<span data-ttu-id="88beb-160">String</span><span class="sxs-lookup"><span data-stu-id="88beb-160">String</span></span>|<span data-ttu-id="88beb-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="88beb-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="88beb-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88beb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88beb-163">versão</span><span class="sxs-lookup"><span data-stu-id="88beb-163">version</span></span>|<span data-ttu-id="88beb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="88beb-164">Int32</span></span>|<span data-ttu-id="88beb-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="88beb-165">Version of the device configuration.</span></span> <span data-ttu-id="88beb-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88beb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88beb-167">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="88beb-167">connectionName</span></span>|<span data-ttu-id="88beb-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88beb-168">String</span></span>|<span data-ttu-id="88beb-169">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="88beb-169">Connection name displayed to the user.</span></span> <span data-ttu-id="88beb-170">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88beb-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="88beb-171">servidores</span><span class="sxs-lookup"><span data-stu-id="88beb-171">servers</span></span>|<span data-ttu-id="88beb-172">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="88beb-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="88beb-173">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="88beb-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="88beb-174">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="88beb-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="88beb-175">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="88beb-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="88beb-176">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88beb-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="88beb-177">customXml</span><span class="sxs-lookup"><span data-stu-id="88beb-177">customXml</span></span>|<span data-ttu-id="88beb-178">Binária</span><span class="sxs-lookup"><span data-stu-id="88beb-178">Binary</span></span>|<span data-ttu-id="88beb-179">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="88beb-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="88beb-180">(Matriz de bytes codificados por UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88beb-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="88beb-181">profileTarget</span><span class="sxs-lookup"><span data-stu-id="88beb-181">profileTarget</span></span>|[<span data-ttu-id="88beb-182">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="88beb-182">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="88beb-183">Tipo de destino do perfil.</span><span class="sxs-lookup"><span data-stu-id="88beb-183">Profile target type.</span></span> <span data-ttu-id="88beb-184">Os valores possíveis são: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="88beb-184">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="88beb-185">Connection</span><span class="sxs-lookup"><span data-stu-id="88beb-185">connectionType</span></span>|[<span data-ttu-id="88beb-186">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="88beb-186">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="88beb-187">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="88beb-187">Connection type.</span></span> <span data-ttu-id="88beb-188">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="88beb-188">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="88beb-189">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="88beb-189">enableSplitTunneling</span></span>|<span data-ttu-id="88beb-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="88beb-190">Boolean</span></span>|<span data-ttu-id="88beb-191">Habilitar o túnel de divisão.</span><span class="sxs-lookup"><span data-stu-id="88beb-191">Enable split tunneling.</span></span>|
|<span data-ttu-id="88beb-192">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="88beb-192">enableAlwaysOn</span></span>|<span data-ttu-id="88beb-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="88beb-193">Boolean</span></span>|<span data-ttu-id="88beb-194">Habilitar o modo Always on.</span><span class="sxs-lookup"><span data-stu-id="88beb-194">Enable Always On mode.</span></span>|
|<span data-ttu-id="88beb-195">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="88beb-195">enableDeviceTunnel</span></span>|<span data-ttu-id="88beb-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="88beb-196">Boolean</span></span>|<span data-ttu-id="88beb-197">Habilitar o túnel de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="88beb-197">Enable device tunnel.</span></span>|
|<span data-ttu-id="88beb-198">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="88beb-198">enableDnsRegistration</span></span>|<span data-ttu-id="88beb-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="88beb-199">Boolean</span></span>|<span data-ttu-id="88beb-200">Habilitar o registro de endereço IP com DNS interno.</span><span class="sxs-lookup"><span data-stu-id="88beb-200">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="88beb-201">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="88beb-201">dnsSuffixes</span></span>|<span data-ttu-id="88beb-202">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="88beb-202">String collection</span></span>|<span data-ttu-id="88beb-203">Especifique sufixos DNS para adicionar à lista de pesquisa de DNS para rotear corretamente nomes curtos.</span><span class="sxs-lookup"><span data-stu-id="88beb-203">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="88beb-204">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="88beb-204">authenticationMethod</span></span>|[<span data-ttu-id="88beb-205">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="88beb-205">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="88beb-206">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="88beb-206">Authentication method.</span></span> <span data-ttu-id="88beb-207">Os valores possíveis são: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="88beb-207">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="88beb-208">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="88beb-208">rememberUserCredentials</span></span>|<span data-ttu-id="88beb-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="88beb-209">Boolean</span></span>|<span data-ttu-id="88beb-210">Lembrar as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="88beb-210">Remember user credentials.</span></span>|
|<span data-ttu-id="88beb-211">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="88beb-211">enableConditionalAccess</span></span>|<span data-ttu-id="88beb-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="88beb-212">Boolean</span></span>|<span data-ttu-id="88beb-213">Habilitar o acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="88beb-213">Enable conditional access.</span></span>|
|<span data-ttu-id="88beb-214">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="88beb-214">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="88beb-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="88beb-215">Boolean</span></span>|<span data-ttu-id="88beb-216">Habilitar o logon único (SSO) com certificado alternativo.</span><span class="sxs-lookup"><span data-stu-id="88beb-216">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="88beb-217">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="88beb-217">singleSignOnEku</span></span>|[<span data-ttu-id="88beb-218">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="88beb-218">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="88beb-219">Uso de chave estendida (EKU) de logon único.</span><span class="sxs-lookup"><span data-stu-id="88beb-219">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="88beb-220">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="88beb-220">singleSignOnIssuerHash</span></span>|<span data-ttu-id="88beb-221">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88beb-221">String</span></span>|<span data-ttu-id="88beb-222">Hash do emissor de logon único.</span><span class="sxs-lookup"><span data-stu-id="88beb-222">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="88beb-223">eapXml</span><span class="sxs-lookup"><span data-stu-id="88beb-223">eapXml</span></span>|<span data-ttu-id="88beb-224">Binária</span><span class="sxs-lookup"><span data-stu-id="88beb-224">Binary</span></span>|<span data-ttu-id="88beb-225">XML EAP (Extensible Authentication Protocol).</span><span class="sxs-lookup"><span data-stu-id="88beb-225">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="88beb-226">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="88beb-226">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="88beb-227">proxyServer</span><span class="sxs-lookup"><span data-stu-id="88beb-227">proxyServer</span></span>|[<span data-ttu-id="88beb-228">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="88beb-228">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="88beb-229">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="88beb-229">Proxy Server.</span></span>|
|<span data-ttu-id="88beb-230">associatedApps</span><span class="sxs-lookup"><span data-stu-id="88beb-230">associatedApps</span></span>|<span data-ttu-id="88beb-231">coleção [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="88beb-231">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="88beb-232">Aplicativos associados.</span><span class="sxs-lookup"><span data-stu-id="88beb-232">Associated Apps.</span></span> <span data-ttu-id="88beb-233">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="88beb-233">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="88beb-234">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="88beb-234">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="88beb-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="88beb-235">Boolean</span></span>|<span data-ttu-id="88beb-236">Somente os aplicativos associados podem usar Connection (VPN por aplicativo).</span><span class="sxs-lookup"><span data-stu-id="88beb-236">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="88beb-237">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="88beb-237">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="88beb-238">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88beb-238">String</span></span>|<span data-ttu-id="88beb-239">Domínio de proteção de informações do Windows (WIP) a ser associado a essa conexão.</span><span class="sxs-lookup"><span data-stu-id="88beb-239">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="88beb-240">trafficRules</span><span class="sxs-lookup"><span data-stu-id="88beb-240">trafficRules</span></span>|<span data-ttu-id="88beb-241">coleção [vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="88beb-241">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="88beb-242">Regras de tráfego.</span><span class="sxs-lookup"><span data-stu-id="88beb-242">Traffic rules.</span></span> <span data-ttu-id="88beb-243">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="88beb-243">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="88beb-244">roteie</span><span class="sxs-lookup"><span data-stu-id="88beb-244">routes</span></span>|<span data-ttu-id="88beb-245">coleção [vpnRoute](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="88beb-245">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="88beb-246">Rotas (opcionais para provedores de terceiros).</span><span class="sxs-lookup"><span data-stu-id="88beb-246">Routes (optional for third-party providers).</span></span> <span data-ttu-id="88beb-247">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="88beb-247">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="88beb-248">dnsRules</span><span class="sxs-lookup"><span data-stu-id="88beb-248">dnsRules</span></span>|<span data-ttu-id="88beb-249">coleção [vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="88beb-249">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="88beb-250">Regras de DNS.</span><span class="sxs-lookup"><span data-stu-id="88beb-250">DNS rules.</span></span> <span data-ttu-id="88beb-251">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="88beb-251">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="88beb-252">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="88beb-252">trustedNetworkDomains</span></span>|<span data-ttu-id="88beb-253">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="88beb-253">String collection</span></span>|<span data-ttu-id="88beb-254">Domínios de rede confiáveis</span><span class="sxs-lookup"><span data-stu-id="88beb-254">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="88beb-255">Resposta</span><span class="sxs-lookup"><span data-stu-id="88beb-255">Response</span></span>
<span data-ttu-id="88beb-256">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88beb-256">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88beb-257">Exemplo</span><span class="sxs-lookup"><span data-stu-id="88beb-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="88beb-258">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88beb-258">Request</span></span>
<span data-ttu-id="88beb-259">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="88beb-259">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3387

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="88beb-260">Resposta</span><span class="sxs-lookup"><span data-stu-id="88beb-260">Response</span></span>
<span data-ttu-id="88beb-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="88beb-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3559

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ]
}
```




