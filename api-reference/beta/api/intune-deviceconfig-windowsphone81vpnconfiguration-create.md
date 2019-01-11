---
title: Criar windowsPhone81VpnConfiguration
description: Crie um novo objeto de windowsPhone81VpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0dfaa4f7c6a40f3acaa83583093291db6196cf79
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844622"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="3be95-103">Criar windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3be95-103">Create windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="3be95-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3be95-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3be95-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3be95-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3be95-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3be95-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3be95-107">Crie um novo objeto de [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3be95-107">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3be95-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3be95-108">Prerequisites</span></span>
<span data-ttu-id="3be95-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3be95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3be95-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3be95-111">Permission type</span></span>|<span data-ttu-id="3be95-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3be95-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3be95-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3be95-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3be95-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3be95-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3be95-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3be95-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3be95-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3be95-116">Not supported.</span></span>|
|<span data-ttu-id="3be95-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3be95-117">Application</span></span>|<span data-ttu-id="3be95-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3be95-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3be95-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3be95-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3be95-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3be95-120">Request headers</span></span>
|<span data-ttu-id="3be95-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3be95-121">Header</span></span>|<span data-ttu-id="3be95-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3be95-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3be95-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3be95-123">Authorization</span></span>|<span data-ttu-id="3be95-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3be95-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3be95-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3be95-125">Accept</span></span>|<span data-ttu-id="3be95-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3be95-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3be95-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3be95-127">Request body</span></span>
<span data-ttu-id="3be95-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3be95-128">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="3be95-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3be95-129">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="3be95-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3be95-130">Property</span></span>|<span data-ttu-id="3be95-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3be95-131">Type</span></span>|<span data-ttu-id="3be95-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3be95-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3be95-133">id</span><span class="sxs-lookup"><span data-stu-id="3be95-133">id</span></span>|<span data-ttu-id="3be95-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3be95-134">String</span></span>|<span data-ttu-id="3be95-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3be95-135">Key of the entity.</span></span> <span data-ttu-id="3be95-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3be95-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3be95-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3be95-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3be95-138">DateTimeOffset</span></span>|<span data-ttu-id="3be95-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3be95-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3be95-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3be95-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3be95-141">roleScopeTagIds</span></span>|<span data-ttu-id="3be95-142">String collection</span><span class="sxs-lookup"><span data-stu-id="3be95-142">String collection</span></span>|<span data-ttu-id="3be95-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="3be95-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3be95-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3be95-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3be95-145">supportsScopeTags</span></span>|<span data-ttu-id="3be95-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="3be95-146">Boolean</span></span>|<span data-ttu-id="3be95-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="3be95-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3be95-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="3be95-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3be95-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="3be95-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3be95-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3be95-150">This property is read-only.</span></span> <span data-ttu-id="3be95-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3be95-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3be95-152">createdDateTime</span></span>|<span data-ttu-id="3be95-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3be95-153">DateTimeOffset</span></span>|<span data-ttu-id="3be95-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3be95-154">DateTime the object was created.</span></span> <span data-ttu-id="3be95-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3be95-156">description</span><span class="sxs-lookup"><span data-stu-id="3be95-156">description</span></span>|<span data-ttu-id="3be95-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3be95-157">String</span></span>|<span data-ttu-id="3be95-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3be95-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3be95-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3be95-160">displayName</span><span class="sxs-lookup"><span data-stu-id="3be95-160">displayName</span></span>|<span data-ttu-id="3be95-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3be95-161">String</span></span>|<span data-ttu-id="3be95-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3be95-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3be95-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3be95-164">version</span><span class="sxs-lookup"><span data-stu-id="3be95-164">version</span></span>|<span data-ttu-id="3be95-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3be95-165">Int32</span></span>|<span data-ttu-id="3be95-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3be95-166">Version of the device configuration.</span></span> <span data-ttu-id="3be95-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3be95-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="3be95-168">connectionName</span></span>|<span data-ttu-id="3be95-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3be95-169">String</span></span>|<span data-ttu-id="3be95-170">Nome da Conexão exibida para o usuário.</span><span class="sxs-lookup"><span data-stu-id="3be95-170">Connection name displayed to the user.</span></span> <span data-ttu-id="3be95-171">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3be95-172">servidores</span><span class="sxs-lookup"><span data-stu-id="3be95-172">servers</span></span>|<span data-ttu-id="3be95-173">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="3be95-174">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="3be95-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="3be95-175">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="3be95-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="3be95-176">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="3be95-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3be95-177">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3be95-178">customXml</span><span class="sxs-lookup"><span data-stu-id="3be95-178">customXml</span></span>|<span data-ttu-id="3be95-179">Binária</span><span class="sxs-lookup"><span data-stu-id="3be95-179">Binary</span></span>|<span data-ttu-id="3be95-180">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="3be95-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="3be95-181">(Array de byte codificado UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="3be95-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="3be95-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="3be95-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="3be95-183">Boolean</span></span>|<span data-ttu-id="3be95-184">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="3be95-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="3be95-185">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3be95-185">This property is read-only.</span></span> <span data-ttu-id="3be95-186">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-186">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="3be95-187">connectionType</span><span class="sxs-lookup"><span data-stu-id="3be95-187">connectionType</span></span>|[<span data-ttu-id="3be95-188">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="3be95-188">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="3be95-189">Tipo de Conexão.</span><span class="sxs-lookup"><span data-stu-id="3be95-189">Connection type.</span></span> <span data-ttu-id="3be95-190">Herdada do [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3be95-190">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="3be95-191">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="3be95-191">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="3be95-192">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="3be95-192">loginGroupOrDomain</span></span>|<span data-ttu-id="3be95-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3be95-193">String</span></span>|<span data-ttu-id="3be95-194">Grupo de login ou domínio quando o tipo de conexão está definida como Dell SonicWALL Mobile Conexão.</span><span class="sxs-lookup"><span data-stu-id="3be95-194">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="3be95-195">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-195">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="3be95-196">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="3be95-196">enableSplitTunneling</span></span>|<span data-ttu-id="3be95-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="3be95-197">Boolean</span></span>|<span data-ttu-id="3be95-198">Habilite o túnel em divisão da VPN.</span><span class="sxs-lookup"><span data-stu-id="3be95-198">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="3be95-199">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-199">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="3be95-200">proxyServer</span><span class="sxs-lookup"><span data-stu-id="3be95-200">proxyServer</span></span>|[<span data-ttu-id="3be95-201">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="3be95-201">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="3be95-202">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="3be95-202">Proxy Server.</span></span> <span data-ttu-id="3be95-203">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3be95-203">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="3be95-204">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="3be95-204">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="3be95-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="3be95-205">Boolean</span></span>|<span data-ttu-id="3be95-206">Desvio VPN empresa Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="3be95-206">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="3be95-207">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="3be95-207">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="3be95-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="3be95-208">Boolean</span></span>|<span data-ttu-id="3be95-209">Desvio VPN em Wi-Fi residencial.</span><span class="sxs-lookup"><span data-stu-id="3be95-209">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="3be95-210">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3be95-210">authenticationMethod</span></span>|[<span data-ttu-id="3be95-211">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3be95-211">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="3be95-212">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3be95-212">Authentication method.</span></span> <span data-ttu-id="3be95-213">Os valores possíveis são: `certificate` e `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="3be95-213">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="3be95-214">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="3be95-214">rememberUserCredentials</span></span>|<span data-ttu-id="3be95-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="3be95-215">Boolean</span></span>|<span data-ttu-id="3be95-216">Lembre-se as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="3be95-216">Remember user credentials.</span></span>|
|<span data-ttu-id="3be95-217">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="3be95-217">dnsSuffixSearchList</span></span>|<span data-ttu-id="3be95-218">String collection</span><span class="sxs-lookup"><span data-stu-id="3be95-218">String collection</span></span>|<span data-ttu-id="3be95-219">Lista de pesquisa de sufixo DNS.</span><span class="sxs-lookup"><span data-stu-id="3be95-219">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="3be95-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="3be95-220">Response</span></span>
<span data-ttu-id="3be95-221">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3be95-221">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3be95-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3be95-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="3be95-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3be95-223">Request</span></span>
<span data-ttu-id="3be95-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3be95-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1307

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="3be95-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="3be95-225">Response</span></span>
<span data-ttu-id="3be95-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3be95-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





