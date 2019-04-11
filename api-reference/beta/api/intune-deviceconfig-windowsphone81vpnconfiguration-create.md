---
title: Criar windowsPhone81VpnConfiguration
description: Criar um novo objeto windowsPhone81VpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb5813815bec4e72319f61ceb50571ffd04321c6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789308"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="23ae6-103">Criar windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="23ae6-103">Create windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="23ae6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="23ae6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23ae6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23ae6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23ae6-106">Criar um novo objeto [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="23ae6-106">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23ae6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="23ae6-107">Prerequisites</span></span>
<span data-ttu-id="23ae6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23ae6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23ae6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23ae6-110">Permission type</span></span>|<span data-ttu-id="23ae6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="23ae6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23ae6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23ae6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="23ae6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23ae6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23ae6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23ae6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23ae6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23ae6-115">Not supported.</span></span>|
|<span data-ttu-id="23ae6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23ae6-116">Application</span></span>|<span data-ttu-id="23ae6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23ae6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23ae6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23ae6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="23ae6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23ae6-119">Request headers</span></span>
|<span data-ttu-id="23ae6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23ae6-120">Header</span></span>|<span data-ttu-id="23ae6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="23ae6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23ae6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="23ae6-122">Authorization</span></span>|<span data-ttu-id="23ae6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23ae6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23ae6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="23ae6-124">Accept</span></span>|<span data-ttu-id="23ae6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="23ae6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23ae6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23ae6-126">Request body</span></span>
<span data-ttu-id="23ae6-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="23ae6-127">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="23ae6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="23ae6-128">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="23ae6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23ae6-129">Property</span></span>|<span data-ttu-id="23ae6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="23ae6-130">Type</span></span>|<span data-ttu-id="23ae6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="23ae6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23ae6-132">id</span><span class="sxs-lookup"><span data-stu-id="23ae6-132">id</span></span>|<span data-ttu-id="23ae6-133">String</span><span class="sxs-lookup"><span data-stu-id="23ae6-133">String</span></span>|<span data-ttu-id="23ae6-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="23ae6-134">Key of the entity.</span></span> <span data-ttu-id="23ae6-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23ae6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23ae6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23ae6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="23ae6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23ae6-137">DateTimeOffset</span></span>|<span data-ttu-id="23ae6-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="23ae6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="23ae6-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23ae6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23ae6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="23ae6-140">roleScopeTagIds</span></span>|<span data-ttu-id="23ae6-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="23ae6-141">String collection</span></span>|<span data-ttu-id="23ae6-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="23ae6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="23ae6-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23ae6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23ae6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="23ae6-144">supportsScopeTags</span></span>|<span data-ttu-id="23ae6-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="23ae6-145">Boolean</span></span>|<span data-ttu-id="23ae6-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="23ae6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="23ae6-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="23ae6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="23ae6-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="23ae6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="23ae6-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23ae6-149">This property is read-only.</span></span> <span data-ttu-id="23ae6-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23ae6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23ae6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23ae6-151">createdDateTime</span></span>|<span data-ttu-id="23ae6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23ae6-152">DateTimeOffset</span></span>|<span data-ttu-id="23ae6-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="23ae6-153">DateTime the object was created.</span></span> <span data-ttu-id="23ae6-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23ae6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23ae6-155">description</span><span class="sxs-lookup"><span data-stu-id="23ae6-155">description</span></span>|<span data-ttu-id="23ae6-156">String</span><span class="sxs-lookup"><span data-stu-id="23ae6-156">String</span></span>|<span data-ttu-id="23ae6-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23ae6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="23ae6-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23ae6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23ae6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="23ae6-159">displayName</span></span>|<span data-ttu-id="23ae6-160">String</span><span class="sxs-lookup"><span data-stu-id="23ae6-160">String</span></span>|<span data-ttu-id="23ae6-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23ae6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="23ae6-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23ae6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23ae6-163">versão</span><span class="sxs-lookup"><span data-stu-id="23ae6-163">version</span></span>|<span data-ttu-id="23ae6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="23ae6-164">Int32</span></span>|<span data-ttu-id="23ae6-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="23ae6-165">Version of the device configuration.</span></span> <span data-ttu-id="23ae6-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23ae6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23ae6-167">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="23ae6-167">connectionName</span></span>|<span data-ttu-id="23ae6-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23ae6-168">String</span></span>|<span data-ttu-id="23ae6-169">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="23ae6-169">Connection name displayed to the user.</span></span> <span data-ttu-id="23ae6-170">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23ae6-170">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="23ae6-171">servidores</span><span class="sxs-lookup"><span data-stu-id="23ae6-171">servers</span></span>|<span data-ttu-id="23ae6-172">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="23ae6-172">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="23ae6-173">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="23ae6-173">List of VPN Servers on the network.</span></span> <span data-ttu-id="23ae6-174">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="23ae6-174">Make sure end users can access these network locations.</span></span> <span data-ttu-id="23ae6-175">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="23ae6-175">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="23ae6-176">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23ae6-176">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="23ae6-177">customXml</span><span class="sxs-lookup"><span data-stu-id="23ae6-177">customXml</span></span>|<span data-ttu-id="23ae6-178">Binary</span><span class="sxs-lookup"><span data-stu-id="23ae6-178">Binary</span></span>|<span data-ttu-id="23ae6-179">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="23ae6-179">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="23ae6-180">(Matriz de bytes codificados por UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23ae6-180">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="23ae6-181">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="23ae6-181">applyOnlyToWindows81</span></span>|<span data-ttu-id="23ae6-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="23ae6-182">Boolean</span></span>|<span data-ttu-id="23ae6-183">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="23ae6-183">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="23ae6-184">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="23ae6-184">This property is read-only.</span></span> <span data-ttu-id="23ae6-185">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23ae6-185">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="23ae6-186">Connection</span><span class="sxs-lookup"><span data-stu-id="23ae6-186">connectionType</span></span>|[<span data-ttu-id="23ae6-187">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="23ae6-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="23ae6-188">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="23ae6-188">Connection type.</span></span> <span data-ttu-id="23ae6-189">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="23ae6-189">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="23ae6-190">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="23ae6-190">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="23ae6-191">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="23ae6-191">loginGroupOrDomain</span></span>|<span data-ttu-id="23ae6-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23ae6-192">String</span></span>|<span data-ttu-id="23ae6-193">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="23ae6-193">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="23ae6-194">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23ae6-194">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="23ae6-195">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="23ae6-195">enableSplitTunneling</span></span>|<span data-ttu-id="23ae6-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="23ae6-196">Boolean</span></span>|<span data-ttu-id="23ae6-197">Habilitar o tunelamento dividido para a VPN.</span><span class="sxs-lookup"><span data-stu-id="23ae6-197">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="23ae6-198">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23ae6-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="23ae6-199">proxyServer</span><span class="sxs-lookup"><span data-stu-id="23ae6-199">proxyServer</span></span>|[<span data-ttu-id="23ae6-200">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="23ae6-200">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="23ae6-201">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="23ae6-201">Proxy Server.</span></span> <span data-ttu-id="23ae6-202">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="23ae6-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="23ae6-203">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="23ae6-203">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="23ae6-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="23ae6-204">Boolean</span></span>|<span data-ttu-id="23ae6-205">Ignorar VPN no Wi-Fi da empresa.</span><span class="sxs-lookup"><span data-stu-id="23ae6-205">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="23ae6-206">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="23ae6-206">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="23ae6-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="23ae6-207">Boolean</span></span>|<span data-ttu-id="23ae6-208">Ignorar VPN no Wi-Fi domiciliar.</span><span class="sxs-lookup"><span data-stu-id="23ae6-208">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="23ae6-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="23ae6-209">authenticationMethod</span></span>|[<span data-ttu-id="23ae6-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="23ae6-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="23ae6-211">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="23ae6-211">Authentication method.</span></span> <span data-ttu-id="23ae6-212">Os valores possíveis são: `certificate` e `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="23ae6-212">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="23ae6-213">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="23ae6-213">rememberUserCredentials</span></span>|<span data-ttu-id="23ae6-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="23ae6-214">Boolean</span></span>|<span data-ttu-id="23ae6-215">Lembrar as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="23ae6-215">Remember user credentials.</span></span>|
|<span data-ttu-id="23ae6-216">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="23ae6-216">dnsSuffixSearchList</span></span>|<span data-ttu-id="23ae6-217">Coleção String</span><span class="sxs-lookup"><span data-stu-id="23ae6-217">String collection</span></span>|<span data-ttu-id="23ae6-218">Lista de pesquisa de sufixo DNS.</span><span class="sxs-lookup"><span data-stu-id="23ae6-218">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="23ae6-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="23ae6-219">Response</span></span>
<span data-ttu-id="23ae6-220">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23ae6-220">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23ae6-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23ae6-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="23ae6-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23ae6-222">Request</span></span>
<span data-ttu-id="23ae6-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23ae6-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1243

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
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
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="23ae6-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="23ae6-224">Response</span></span>
<span data-ttu-id="23ae6-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23ae6-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1415

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "id": "7cecc0db-c0db-7cec-dbc0-ec7cdbc0ec7c",
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
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```





