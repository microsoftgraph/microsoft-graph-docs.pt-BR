---
title: Criar windowsPhone81VpnConfiguration
description: Crie um novo objeto de windowsPhone81VpnConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0079291ca4c22b0ee4cd04f42f63b8bd0287d87c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414568"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="afaf0-103">Criar windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="afaf0-103">Create windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="afaf0-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="afaf0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="afaf0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="afaf0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="afaf0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="afaf0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afaf0-107">Crie um novo objeto de [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="afaf0-107">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afaf0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="afaf0-108">Prerequisites</span></span>
<span data-ttu-id="afaf0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="afaf0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="afaf0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afaf0-111">Permission type</span></span>|<span data-ttu-id="afaf0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="afaf0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afaf0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afaf0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="afaf0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afaf0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="afaf0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afaf0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afaf0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afaf0-116">Not supported.</span></span>|
|<span data-ttu-id="afaf0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="afaf0-117">Application</span></span>|<span data-ttu-id="afaf0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afaf0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afaf0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afaf0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="afaf0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afaf0-120">Request headers</span></span>
|<span data-ttu-id="afaf0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="afaf0-121">Header</span></span>|<span data-ttu-id="afaf0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="afaf0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afaf0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="afaf0-123">Authorization</span></span>|<span data-ttu-id="afaf0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afaf0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afaf0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="afaf0-125">Accept</span></span>|<span data-ttu-id="afaf0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="afaf0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afaf0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afaf0-127">Request body</span></span>
<span data-ttu-id="afaf0-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="afaf0-128">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="afaf0-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="afaf0-129">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="afaf0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="afaf0-130">Property</span></span>|<span data-ttu-id="afaf0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="afaf0-131">Type</span></span>|<span data-ttu-id="afaf0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="afaf0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afaf0-133">id</span><span class="sxs-lookup"><span data-stu-id="afaf0-133">id</span></span>|<span data-ttu-id="afaf0-134">String</span><span class="sxs-lookup"><span data-stu-id="afaf0-134">String</span></span>|<span data-ttu-id="afaf0-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="afaf0-135">Key of the entity.</span></span> <span data-ttu-id="afaf0-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afaf0-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afaf0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="afaf0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="afaf0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afaf0-138">DateTimeOffset</span></span>|<span data-ttu-id="afaf0-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="afaf0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="afaf0-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afaf0-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afaf0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="afaf0-141">roleScopeTagIds</span></span>|<span data-ttu-id="afaf0-142">String collection</span><span class="sxs-lookup"><span data-stu-id="afaf0-142">String collection</span></span>|<span data-ttu-id="afaf0-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="afaf0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="afaf0-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afaf0-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afaf0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="afaf0-145">supportsScopeTags</span></span>|<span data-ttu-id="afaf0-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="afaf0-146">Boolean</span></span>|<span data-ttu-id="afaf0-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="afaf0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="afaf0-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="afaf0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="afaf0-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="afaf0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="afaf0-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="afaf0-150">This property is read-only.</span></span> <span data-ttu-id="afaf0-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afaf0-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afaf0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="afaf0-152">createdDateTime</span></span>|<span data-ttu-id="afaf0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afaf0-153">DateTimeOffset</span></span>|<span data-ttu-id="afaf0-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="afaf0-154">DateTime the object was created.</span></span> <span data-ttu-id="afaf0-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afaf0-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afaf0-156">description</span><span class="sxs-lookup"><span data-stu-id="afaf0-156">description</span></span>|<span data-ttu-id="afaf0-157">String</span><span class="sxs-lookup"><span data-stu-id="afaf0-157">String</span></span>|<span data-ttu-id="afaf0-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="afaf0-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="afaf0-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afaf0-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afaf0-160">displayName</span><span class="sxs-lookup"><span data-stu-id="afaf0-160">displayName</span></span>|<span data-ttu-id="afaf0-161">String</span><span class="sxs-lookup"><span data-stu-id="afaf0-161">String</span></span>|<span data-ttu-id="afaf0-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="afaf0-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="afaf0-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afaf0-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afaf0-164">version</span><span class="sxs-lookup"><span data-stu-id="afaf0-164">version</span></span>|<span data-ttu-id="afaf0-165">Int32</span><span class="sxs-lookup"><span data-stu-id="afaf0-165">Int32</span></span>|<span data-ttu-id="afaf0-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="afaf0-166">Version of the device configuration.</span></span> <span data-ttu-id="afaf0-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afaf0-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afaf0-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="afaf0-168">connectionName</span></span>|<span data-ttu-id="afaf0-169">String</span><span class="sxs-lookup"><span data-stu-id="afaf0-169">String</span></span>|<span data-ttu-id="afaf0-170">Nome da Conexão exibida para o usuário.</span><span class="sxs-lookup"><span data-stu-id="afaf0-170">Connection name displayed to the user.</span></span> <span data-ttu-id="afaf0-171">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afaf0-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="afaf0-172">servidores</span><span class="sxs-lookup"><span data-stu-id="afaf0-172">servers</span></span>|<span data-ttu-id="afaf0-173">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="afaf0-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="afaf0-174">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="afaf0-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="afaf0-175">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="afaf0-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="afaf0-176">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="afaf0-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="afaf0-177">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afaf0-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="afaf0-178">customXml</span><span class="sxs-lookup"><span data-stu-id="afaf0-178">customXml</span></span>|<span data-ttu-id="afaf0-179">Binária</span><span class="sxs-lookup"><span data-stu-id="afaf0-179">Binary</span></span>|<span data-ttu-id="afaf0-180">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="afaf0-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="afaf0-181">(Array de byte codificado UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afaf0-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="afaf0-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="afaf0-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="afaf0-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="afaf0-183">Boolean</span></span>|<span data-ttu-id="afaf0-184">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="afaf0-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="afaf0-185">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="afaf0-185">This property is read-only.</span></span> <span data-ttu-id="afaf0-186">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afaf0-186">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="afaf0-187">connectionType</span><span class="sxs-lookup"><span data-stu-id="afaf0-187">connectionType</span></span>|[<span data-ttu-id="afaf0-188">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="afaf0-188">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="afaf0-189">Tipo de Conexão.</span><span class="sxs-lookup"><span data-stu-id="afaf0-189">Connection type.</span></span> <span data-ttu-id="afaf0-190">Herdada do [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="afaf0-190">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="afaf0-191">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="afaf0-191">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="afaf0-192">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="afaf0-192">loginGroupOrDomain</span></span>|<span data-ttu-id="afaf0-193">String</span><span class="sxs-lookup"><span data-stu-id="afaf0-193">String</span></span>|<span data-ttu-id="afaf0-194">Grupo de login ou domínio quando o tipo de conexão está definida como Dell SonicWALL Mobile Conexão.</span><span class="sxs-lookup"><span data-stu-id="afaf0-194">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="afaf0-195">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afaf0-195">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="afaf0-196">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="afaf0-196">enableSplitTunneling</span></span>|<span data-ttu-id="afaf0-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="afaf0-197">Boolean</span></span>|<span data-ttu-id="afaf0-198">Habilite o túnel em divisão da VPN.</span><span class="sxs-lookup"><span data-stu-id="afaf0-198">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="afaf0-199">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afaf0-199">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="afaf0-200">proxyServer</span><span class="sxs-lookup"><span data-stu-id="afaf0-200">proxyServer</span></span>|[<span data-ttu-id="afaf0-201">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="afaf0-201">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="afaf0-202">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="afaf0-202">Proxy Server.</span></span> <span data-ttu-id="afaf0-203">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="afaf0-203">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="afaf0-204">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="afaf0-204">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="afaf0-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="afaf0-205">Boolean</span></span>|<span data-ttu-id="afaf0-206">Desvio VPN empresa Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="afaf0-206">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="afaf0-207">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="afaf0-207">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="afaf0-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="afaf0-208">Boolean</span></span>|<span data-ttu-id="afaf0-209">Desvio VPN em Wi-Fi residencial.</span><span class="sxs-lookup"><span data-stu-id="afaf0-209">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="afaf0-210">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="afaf0-210">authenticationMethod</span></span>|[<span data-ttu-id="afaf0-211">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="afaf0-211">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="afaf0-212">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="afaf0-212">Authentication method.</span></span> <span data-ttu-id="afaf0-213">Os valores possíveis são: `certificate` e `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="afaf0-213">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="afaf0-214">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="afaf0-214">rememberUserCredentials</span></span>|<span data-ttu-id="afaf0-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="afaf0-215">Boolean</span></span>|<span data-ttu-id="afaf0-216">Lembre-se as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="afaf0-216">Remember user credentials.</span></span>|
|<span data-ttu-id="afaf0-217">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="afaf0-217">dnsSuffixSearchList</span></span>|<span data-ttu-id="afaf0-218">String collection</span><span class="sxs-lookup"><span data-stu-id="afaf0-218">String collection</span></span>|<span data-ttu-id="afaf0-219">Lista de pesquisa de sufixo DNS.</span><span class="sxs-lookup"><span data-stu-id="afaf0-219">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="afaf0-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="afaf0-220">Response</span></span>
<span data-ttu-id="afaf0-221">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="afaf0-221">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afaf0-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="afaf0-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="afaf0-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="afaf0-223">Request</span></span>
<span data-ttu-id="afaf0-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="afaf0-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="afaf0-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="afaf0-225">Response</span></span>
<span data-ttu-id="afaf0-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="afaf0-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




