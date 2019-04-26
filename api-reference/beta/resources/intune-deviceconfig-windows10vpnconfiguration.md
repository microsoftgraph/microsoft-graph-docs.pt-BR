---
title: tipo de recurso windows10VpnConfiguration
description: Ao fornecer as configurações neste perfil, você pode instruir o dispositivo Windows 10 (desktop ou celular) a se conectar ao ponto de extremidade VPN desejado. Especificando o método de autenticação e os tipos de segurança esperados pelo ponto de extremidade da VPN, você pode tornar a conexão VPN perfeita para o usuário final.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88d32aedb16516f7659ff6e8094172e4a59f6345
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572014"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="2dcef-104">tipo de recurso windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2dcef-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="2dcef-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2dcef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2dcef-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2dcef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dcef-107">Ao fornecer as configurações neste perfil, você pode instruir o dispositivo Windows 10 (desktop ou celular) a se conectar ao ponto de extremidade VPN desejado.</span><span class="sxs-lookup"><span data-stu-id="2dcef-107">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="2dcef-108">Especificando o método de autenticação e os tipos de segurança esperados pelo ponto de extremidade da VPN, você pode tornar a conexão VPN perfeita para o usuário final.</span><span class="sxs-lookup"><span data-stu-id="2dcef-108">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="2dcef-109">Herda de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-109">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2dcef-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="2dcef-110">Methods</span></span>
|<span data-ttu-id="2dcef-111">Método</span><span class="sxs-lookup"><span data-stu-id="2dcef-111">Method</span></span>|<span data-ttu-id="2dcef-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2dcef-112">Return Type</span></span>|<span data-ttu-id="2dcef-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dcef-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2dcef-114">Listar windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="2dcef-114">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="2dcef-115">coleção [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="2dcef-116">Listar Propriedades e relações dos objetos [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2dcef-116">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="2dcef-117">Obter windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2dcef-117">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="2dcef-118">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2dcef-118">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="2dcef-119">Leia as propriedades e as relações do objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2dcef-119">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="2dcef-120">Criar windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2dcef-120">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="2dcef-121">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2dcef-121">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="2dcef-122">Criar um novo objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2dcef-122">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="2dcef-123">Excluir windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2dcef-123">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="2dcef-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2dcef-124">None</span></span>|<span data-ttu-id="2dcef-125">Exclui [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2dcef-125">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="2dcef-126">Atualizar windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2dcef-126">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="2dcef-127">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2dcef-127">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="2dcef-128">Atualiza as propriedades de um objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2dcef-128">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2dcef-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2dcef-129">Properties</span></span>
|<span data-ttu-id="2dcef-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2dcef-130">Property</span></span>|<span data-ttu-id="2dcef-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2dcef-131">Type</span></span>|<span data-ttu-id="2dcef-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dcef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dcef-133">id</span><span class="sxs-lookup"><span data-stu-id="2dcef-133">id</span></span>|<span data-ttu-id="2dcef-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2dcef-134">String</span></span>|<span data-ttu-id="2dcef-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2dcef-135">Key of the entity.</span></span> <span data-ttu-id="2dcef-136">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2dcef-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2dcef-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dcef-138">DateTimeOffset</span></span>|<span data-ttu-id="2dcef-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2dcef-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2dcef-140">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2dcef-141">roleScopeTagIds</span></span>|<span data-ttu-id="2dcef-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2dcef-142">String collection</span></span>|<span data-ttu-id="2dcef-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="2dcef-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2dcef-144">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2dcef-145">supportsScopeTags</span></span>|<span data-ttu-id="2dcef-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="2dcef-146">Boolean</span></span>|<span data-ttu-id="2dcef-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="2dcef-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2dcef-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="2dcef-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2dcef-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="2dcef-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2dcef-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2dcef-150">This property is read-only.</span></span> <span data-ttu-id="2dcef-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2dcef-152">createdDateTime</span></span>|<span data-ttu-id="2dcef-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dcef-153">DateTimeOffset</span></span>|<span data-ttu-id="2dcef-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2dcef-154">DateTime the object was created.</span></span> <span data-ttu-id="2dcef-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-156">description</span><span class="sxs-lookup"><span data-stu-id="2dcef-156">description</span></span>|<span data-ttu-id="2dcef-157">String</span><span class="sxs-lookup"><span data-stu-id="2dcef-157">String</span></span>|<span data-ttu-id="2dcef-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2dcef-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2dcef-159">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2dcef-160">displayName</span></span>|<span data-ttu-id="2dcef-161">String</span><span class="sxs-lookup"><span data-stu-id="2dcef-161">String</span></span>|<span data-ttu-id="2dcef-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2dcef-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2dcef-163">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-164">versão</span><span class="sxs-lookup"><span data-stu-id="2dcef-164">version</span></span>|<span data-ttu-id="2dcef-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2dcef-165">Int32</span></span>|<span data-ttu-id="2dcef-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2dcef-166">Version of the device configuration.</span></span> <span data-ttu-id="2dcef-167">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-168">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="2dcef-168">connectionName</span></span>|<span data-ttu-id="2dcef-169">String</span><span class="sxs-lookup"><span data-stu-id="2dcef-169">String</span></span>|<span data-ttu-id="2dcef-170">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="2dcef-170">Connection name displayed to the user.</span></span> <span data-ttu-id="2dcef-171">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-172">servidores</span><span class="sxs-lookup"><span data-stu-id="2dcef-172">servers</span></span>|<span data-ttu-id="2dcef-173">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="2dcef-174">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="2dcef-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="2dcef-175">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="2dcef-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="2dcef-176">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="2dcef-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="2dcef-177">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-178">customXml</span><span class="sxs-lookup"><span data-stu-id="2dcef-178">customXml</span></span>|<span data-ttu-id="2dcef-179">Binário</span><span class="sxs-lookup"><span data-stu-id="2dcef-179">Binary</span></span>|<span data-ttu-id="2dcef-180">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="2dcef-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="2dcef-181">(Matriz de bytes codificados por UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-182">profileTarget</span><span class="sxs-lookup"><span data-stu-id="2dcef-182">profileTarget</span></span>|[<span data-ttu-id="2dcef-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="2dcef-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="2dcef-184">Tipo de destino do perfil.</span><span class="sxs-lookup"><span data-stu-id="2dcef-184">Profile target type.</span></span> <span data-ttu-id="2dcef-185">Os valores possíveis são: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="2dcef-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="2dcef-186">Connection</span><span class="sxs-lookup"><span data-stu-id="2dcef-186">connectionType</span></span>|[<span data-ttu-id="2dcef-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="2dcef-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="2dcef-188">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="2dcef-188">Connection type.</span></span> <span data-ttu-id="2dcef-189">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="2dcef-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="2dcef-190">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="2dcef-190">enableSplitTunneling</span></span>|<span data-ttu-id="2dcef-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="2dcef-191">Boolean</span></span>|<span data-ttu-id="2dcef-192">Habilitar o túnel de divisão.</span><span class="sxs-lookup"><span data-stu-id="2dcef-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="2dcef-193">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="2dcef-193">enableAlwaysOn</span></span>|<span data-ttu-id="2dcef-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="2dcef-194">Boolean</span></span>|<span data-ttu-id="2dcef-195">Habilitar o modo Always on.</span><span class="sxs-lookup"><span data-stu-id="2dcef-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="2dcef-196">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="2dcef-196">enableDeviceTunnel</span></span>|<span data-ttu-id="2dcef-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="2dcef-197">Boolean</span></span>|<span data-ttu-id="2dcef-198">Habilitar o túnel de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2dcef-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="2dcef-199">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="2dcef-199">enableDnsRegistration</span></span>|<span data-ttu-id="2dcef-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="2dcef-200">Boolean</span></span>|<span data-ttu-id="2dcef-201">Habilitar o registro de endereço IP com DNS interno.</span><span class="sxs-lookup"><span data-stu-id="2dcef-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="2dcef-202">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="2dcef-202">dnsSuffixes</span></span>|<span data-ttu-id="2dcef-203">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2dcef-203">String collection</span></span>|<span data-ttu-id="2dcef-204">Especifique sufixos DNS para adicionar à lista de pesquisa de DNS para rotear corretamente nomes curtos.</span><span class="sxs-lookup"><span data-stu-id="2dcef-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="2dcef-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2dcef-205">authenticationMethod</span></span>|[<span data-ttu-id="2dcef-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2dcef-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="2dcef-207">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="2dcef-207">Authentication method.</span></span> <span data-ttu-id="2dcef-208">Os valores possíveis são: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="2dcef-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="2dcef-209">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="2dcef-209">rememberUserCredentials</span></span>|<span data-ttu-id="2dcef-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="2dcef-210">Boolean</span></span>|<span data-ttu-id="2dcef-211">Lembrar as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="2dcef-211">Remember user credentials.</span></span>|
|<span data-ttu-id="2dcef-212">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="2dcef-212">enableConditionalAccess</span></span>|<span data-ttu-id="2dcef-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="2dcef-213">Boolean</span></span>|<span data-ttu-id="2dcef-214">Habilitar o acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="2dcef-214">Enable conditional access.</span></span>|
|<span data-ttu-id="2dcef-215">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="2dcef-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="2dcef-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="2dcef-216">Boolean</span></span>|<span data-ttu-id="2dcef-217">Habilitar o logon único (SSO) com certificado alternativo.</span><span class="sxs-lookup"><span data-stu-id="2dcef-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="2dcef-218">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="2dcef-218">singleSignOnEku</span></span>|[<span data-ttu-id="2dcef-219">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="2dcef-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="2dcef-220">Uso de chave estendida (EKU) de logon único.</span><span class="sxs-lookup"><span data-stu-id="2dcef-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="2dcef-221">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="2dcef-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="2dcef-222">String</span><span class="sxs-lookup"><span data-stu-id="2dcef-222">String</span></span>|<span data-ttu-id="2dcef-223">Hash do emissor de logon único.</span><span class="sxs-lookup"><span data-stu-id="2dcef-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="2dcef-224">eapXml</span><span class="sxs-lookup"><span data-stu-id="2dcef-224">eapXml</span></span>|<span data-ttu-id="2dcef-225">Binário</span><span class="sxs-lookup"><span data-stu-id="2dcef-225">Binary</span></span>|<span data-ttu-id="2dcef-226">XML EAP (Extensible Authentication Protocol).</span><span class="sxs-lookup"><span data-stu-id="2dcef-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="2dcef-227">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="2dcef-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="2dcef-228">proxyServer</span><span class="sxs-lookup"><span data-stu-id="2dcef-228">proxyServer</span></span>|[<span data-ttu-id="2dcef-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="2dcef-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="2dcef-230">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="2dcef-230">Proxy Server.</span></span>|
|<span data-ttu-id="2dcef-231">associatedApps</span><span class="sxs-lookup"><span data-stu-id="2dcef-231">associatedApps</span></span>|<span data-ttu-id="2dcef-232">coleção [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="2dcef-233">Aplicativos associados.</span><span class="sxs-lookup"><span data-stu-id="2dcef-233">Associated Apps.</span></span> <span data-ttu-id="2dcef-234">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="2dcef-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="2dcef-235">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="2dcef-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="2dcef-236">Booliano</span><span class="sxs-lookup"><span data-stu-id="2dcef-236">Boolean</span></span>|<span data-ttu-id="2dcef-237">Somente os aplicativos associados podem usar Connection (VPN por aplicativo).</span><span class="sxs-lookup"><span data-stu-id="2dcef-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="2dcef-238">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="2dcef-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="2dcef-239">String</span><span class="sxs-lookup"><span data-stu-id="2dcef-239">String</span></span>|<span data-ttu-id="2dcef-240">Domínio de proteção de informações do Windows (WIP) a ser associado a essa conexão.</span><span class="sxs-lookup"><span data-stu-id="2dcef-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="2dcef-241">trafficRules</span><span class="sxs-lookup"><span data-stu-id="2dcef-241">trafficRules</span></span>|<span data-ttu-id="2dcef-242">coleção [vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="2dcef-243">Regras de tráfego.</span><span class="sxs-lookup"><span data-stu-id="2dcef-243">Traffic rules.</span></span> <span data-ttu-id="2dcef-244">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="2dcef-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="2dcef-245">roteie</span><span class="sxs-lookup"><span data-stu-id="2dcef-245">routes</span></span>|<span data-ttu-id="2dcef-246">coleção [vpnRoute](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="2dcef-247">Rotas (opcionais para provedores de terceiros).</span><span class="sxs-lookup"><span data-stu-id="2dcef-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="2dcef-248">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="2dcef-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="2dcef-249">dnsRules</span><span class="sxs-lookup"><span data-stu-id="2dcef-249">dnsRules</span></span>|<span data-ttu-id="2dcef-250">coleção [vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="2dcef-251">Regras de DNS.</span><span class="sxs-lookup"><span data-stu-id="2dcef-251">DNS rules.</span></span> <span data-ttu-id="2dcef-252">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="2dcef-252">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="2dcef-253">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="2dcef-253">trustedNetworkDomains</span></span>|<span data-ttu-id="2dcef-254">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2dcef-254">String collection</span></span>|<span data-ttu-id="2dcef-255">Domínios de rede confiáveis</span><span class="sxs-lookup"><span data-stu-id="2dcef-255">Trusted Network Domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="2dcef-256">Relações</span><span class="sxs-lookup"><span data-stu-id="2dcef-256">Relationships</span></span>
|<span data-ttu-id="2dcef-257">Relação</span><span class="sxs-lookup"><span data-stu-id="2dcef-257">Relationship</span></span>|<span data-ttu-id="2dcef-258">Tipo</span><span class="sxs-lookup"><span data-stu-id="2dcef-258">Type</span></span>|<span data-ttu-id="2dcef-259">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dcef-259">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dcef-260">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="2dcef-260">groupAssignments</span></span>|<span data-ttu-id="2dcef-261">coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-261">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="2dcef-262">A lista de atribuições de grupo para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2dcef-262">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="2dcef-263">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-263">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-264">assignments</span><span class="sxs-lookup"><span data-stu-id="2dcef-264">assignments</span></span>|<span data-ttu-id="2dcef-265">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-265">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2dcef-266">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2dcef-266">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="2dcef-267">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-267">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-268">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="2dcef-268">deviceStatuses</span></span>|<span data-ttu-id="2dcef-269">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-269">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="2dcef-270">Status da instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2dcef-270">Device configuration installation status by device.</span></span> <span data-ttu-id="2dcef-271">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-271">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-272">userStatuses</span><span class="sxs-lookup"><span data-stu-id="2dcef-272">userStatuses</span></span>|<span data-ttu-id="2dcef-273">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-273">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="2dcef-274">Status de instalação da configuração do dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="2dcef-274">Device configuration installation status by user.</span></span> <span data-ttu-id="2dcef-275">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-275">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-276">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="2dcef-276">deviceStatusOverview</span></span>|[<span data-ttu-id="2dcef-277">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="2dcef-277">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="2dcef-278">Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-278">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-279">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="2dcef-279">userStatusOverview</span></span>|[<span data-ttu-id="2dcef-280">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="2dcef-280">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="2dcef-281">Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-281">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-282">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="2dcef-282">deviceSettingStateSummaries</span></span>|<span data-ttu-id="2dcef-283">Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-283">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="2dcef-284">Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2dcef-284">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dcef-285">identityCertificate</span><span class="sxs-lookup"><span data-stu-id="2dcef-285">identityCertificate</span></span>|[<span data-ttu-id="2dcef-286">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="2dcef-286">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="2dcef-287">Certificado de identidade para autenticação de cliente quando o método de autenticação é certificado.</span><span class="sxs-lookup"><span data-stu-id="2dcef-287">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2dcef-288">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2dcef-288">JSON Representation</span></span>
<span data-ttu-id="2dcef-289">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2dcef-289">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "connectionName": "String",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ],
  "customXml": "binary",
  "profileTarget": "String",
  "connectionType": "String",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "String"
  ],
  "authenticationMethod": "String",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "String",
    "objectIdentifier": "String"
  },
  "singleSignOnIssuerHash": "String",
  "eapXml": "binary",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "String",
      "identifier": "String"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "String",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "String",
      "protocols": 1024,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "appId": "String",
      "appType": "String",
      "routingPolicyType": "String",
      "claims": "String"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "String",
      "prefixSize": 1024
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "String",
      "servers": [
        "String"
      ],
      "proxyServerUri": "String",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "String"
  ]
}
```





