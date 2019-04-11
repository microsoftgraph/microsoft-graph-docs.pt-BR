---
title: tipo de recurso windows10VpnConfiguration
description: Ao fornecer as configurações neste perfil, você pode instruir o dispositivo Windows 10 (desktop ou celular) a se conectar ao ponto de extremidade VPN desejado. Especificando o método de autenticação e os tipos de segurança esperados pelo ponto de extremidade da VPN, você pode tornar a conexão VPN perfeita para o usuário final.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88d32aedb16516f7659ff6e8094172e4a59f6345
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794551"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="db0f1-104">tipo de recurso windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="db0f1-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="db0f1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="db0f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db0f1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db0f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db0f1-107">Ao fornecer as configurações neste perfil, você pode instruir o dispositivo Windows 10 (desktop ou celular) a se conectar ao ponto de extremidade VPN desejado.</span><span class="sxs-lookup"><span data-stu-id="db0f1-107">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="db0f1-108">Especificando o método de autenticação e os tipos de segurança esperados pelo ponto de extremidade da VPN, você pode tornar a conexão VPN perfeita para o usuário final.</span><span class="sxs-lookup"><span data-stu-id="db0f1-108">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="db0f1-109">Herda de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-109">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="db0f1-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="db0f1-110">Methods</span></span>
|<span data-ttu-id="db0f1-111">Método</span><span class="sxs-lookup"><span data-stu-id="db0f1-111">Method</span></span>|<span data-ttu-id="db0f1-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="db0f1-112">Return Type</span></span>|<span data-ttu-id="db0f1-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="db0f1-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="db0f1-114">Listar windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="db0f1-114">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="db0f1-115">coleção [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-115">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="db0f1-116">Listar Propriedades e relações dos objetos [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="db0f1-116">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="db0f1-117">Obter windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="db0f1-117">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="db0f1-118">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="db0f1-118">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="db0f1-119">Leia as propriedades e as relações do objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="db0f1-119">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="db0f1-120">Criar windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="db0f1-120">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="db0f1-121">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="db0f1-121">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="db0f1-122">Criar um novo objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="db0f1-122">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="db0f1-123">Excluir windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="db0f1-123">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="db0f1-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db0f1-124">None</span></span>|<span data-ttu-id="db0f1-125">Exclui [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db0f1-125">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="db0f1-126">Atualizar windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="db0f1-126">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="db0f1-127">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="db0f1-127">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="db0f1-128">Atualiza as propriedades de um objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="db0f1-128">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="db0f1-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db0f1-129">Properties</span></span>
|<span data-ttu-id="db0f1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db0f1-130">Property</span></span>|<span data-ttu-id="db0f1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="db0f1-131">Type</span></span>|<span data-ttu-id="db0f1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="db0f1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db0f1-133">id</span><span class="sxs-lookup"><span data-stu-id="db0f1-133">id</span></span>|<span data-ttu-id="db0f1-134">String</span><span class="sxs-lookup"><span data-stu-id="db0f1-134">String</span></span>|<span data-ttu-id="db0f1-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="db0f1-135">Key of the entity.</span></span> <span data-ttu-id="db0f1-136">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db0f1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="db0f1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db0f1-138">DateTimeOffset</span></span>|<span data-ttu-id="db0f1-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="db0f1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="db0f1-140">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="db0f1-141">roleScopeTagIds</span></span>|<span data-ttu-id="db0f1-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="db0f1-142">String collection</span></span>|<span data-ttu-id="db0f1-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="db0f1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="db0f1-144">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="db0f1-145">supportsScopeTags</span></span>|<span data-ttu-id="db0f1-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="db0f1-146">Boolean</span></span>|<span data-ttu-id="db0f1-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="db0f1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="db0f1-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="db0f1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="db0f1-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="db0f1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="db0f1-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="db0f1-150">This property is read-only.</span></span> <span data-ttu-id="db0f1-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db0f1-152">createdDateTime</span></span>|<span data-ttu-id="db0f1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db0f1-153">DateTimeOffset</span></span>|<span data-ttu-id="db0f1-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="db0f1-154">DateTime the object was created.</span></span> <span data-ttu-id="db0f1-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-156">description</span><span class="sxs-lookup"><span data-stu-id="db0f1-156">description</span></span>|<span data-ttu-id="db0f1-157">String</span><span class="sxs-lookup"><span data-stu-id="db0f1-157">String</span></span>|<span data-ttu-id="db0f1-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db0f1-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="db0f1-159">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-160">displayName</span><span class="sxs-lookup"><span data-stu-id="db0f1-160">displayName</span></span>|<span data-ttu-id="db0f1-161">String</span><span class="sxs-lookup"><span data-stu-id="db0f1-161">String</span></span>|<span data-ttu-id="db0f1-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db0f1-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="db0f1-163">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-164">versão</span><span class="sxs-lookup"><span data-stu-id="db0f1-164">version</span></span>|<span data-ttu-id="db0f1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="db0f1-165">Int32</span></span>|<span data-ttu-id="db0f1-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db0f1-166">Version of the device configuration.</span></span> <span data-ttu-id="db0f1-167">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-168">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="db0f1-168">connectionName</span></span>|<span data-ttu-id="db0f1-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db0f1-169">String</span></span>|<span data-ttu-id="db0f1-170">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="db0f1-170">Connection name displayed to the user.</span></span> <span data-ttu-id="db0f1-171">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-172">servidores</span><span class="sxs-lookup"><span data-stu-id="db0f1-172">servers</span></span>|<span data-ttu-id="db0f1-173">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="db0f1-174">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="db0f1-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="db0f1-175">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="db0f1-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="db0f1-176">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="db0f1-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="db0f1-177">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-178">customXml</span><span class="sxs-lookup"><span data-stu-id="db0f1-178">customXml</span></span>|<span data-ttu-id="db0f1-179">Binary</span><span class="sxs-lookup"><span data-stu-id="db0f1-179">Binary</span></span>|<span data-ttu-id="db0f1-180">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="db0f1-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="db0f1-181">(Matriz de bytes codificados por UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-182">profileTarget</span><span class="sxs-lookup"><span data-stu-id="db0f1-182">profileTarget</span></span>|[<span data-ttu-id="db0f1-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="db0f1-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="db0f1-184">Tipo de destino do perfil.</span><span class="sxs-lookup"><span data-stu-id="db0f1-184">Profile target type.</span></span> <span data-ttu-id="db0f1-185">Os valores possíveis são: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="db0f1-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="db0f1-186">Connection</span><span class="sxs-lookup"><span data-stu-id="db0f1-186">connectionType</span></span>|[<span data-ttu-id="db0f1-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="db0f1-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="db0f1-188">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="db0f1-188">Connection type.</span></span> <span data-ttu-id="db0f1-189">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="db0f1-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="db0f1-190">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="db0f1-190">enableSplitTunneling</span></span>|<span data-ttu-id="db0f1-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="db0f1-191">Boolean</span></span>|<span data-ttu-id="db0f1-192">Habilitar o túnel de divisão.</span><span class="sxs-lookup"><span data-stu-id="db0f1-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="db0f1-193">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="db0f1-193">enableAlwaysOn</span></span>|<span data-ttu-id="db0f1-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="db0f1-194">Boolean</span></span>|<span data-ttu-id="db0f1-195">Habilitar o modo Always on.</span><span class="sxs-lookup"><span data-stu-id="db0f1-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="db0f1-196">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="db0f1-196">enableDeviceTunnel</span></span>|<span data-ttu-id="db0f1-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="db0f1-197">Boolean</span></span>|<span data-ttu-id="db0f1-198">Habilitar o túnel de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db0f1-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="db0f1-199">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="db0f1-199">enableDnsRegistration</span></span>|<span data-ttu-id="db0f1-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="db0f1-200">Boolean</span></span>|<span data-ttu-id="db0f1-201">Habilitar o registro de endereço IP com DNS interno.</span><span class="sxs-lookup"><span data-stu-id="db0f1-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="db0f1-202">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="db0f1-202">dnsSuffixes</span></span>|<span data-ttu-id="db0f1-203">Coleção String</span><span class="sxs-lookup"><span data-stu-id="db0f1-203">String collection</span></span>|<span data-ttu-id="db0f1-204">Especifique sufixos DNS para adicionar à lista de pesquisa de DNS para rotear corretamente nomes curtos.</span><span class="sxs-lookup"><span data-stu-id="db0f1-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="db0f1-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="db0f1-205">authenticationMethod</span></span>|[<span data-ttu-id="db0f1-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="db0f1-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="db0f1-207">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="db0f1-207">Authentication method.</span></span> <span data-ttu-id="db0f1-208">Os valores possíveis são: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="db0f1-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="db0f1-209">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="db0f1-209">rememberUserCredentials</span></span>|<span data-ttu-id="db0f1-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="db0f1-210">Boolean</span></span>|<span data-ttu-id="db0f1-211">Lembrar as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="db0f1-211">Remember user credentials.</span></span>|
|<span data-ttu-id="db0f1-212">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="db0f1-212">enableConditionalAccess</span></span>|<span data-ttu-id="db0f1-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="db0f1-213">Boolean</span></span>|<span data-ttu-id="db0f1-214">Habilitar o acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="db0f1-214">Enable conditional access.</span></span>|
|<span data-ttu-id="db0f1-215">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="db0f1-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="db0f1-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="db0f1-216">Boolean</span></span>|<span data-ttu-id="db0f1-217">Habilitar o logon único (SSO) com certificado alternativo.</span><span class="sxs-lookup"><span data-stu-id="db0f1-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="db0f1-218">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="db0f1-218">singleSignOnEku</span></span>|[<span data-ttu-id="db0f1-219">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="db0f1-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="db0f1-220">Uso de chave estendida (EKU) de logon único.</span><span class="sxs-lookup"><span data-stu-id="db0f1-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="db0f1-221">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="db0f1-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="db0f1-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db0f1-222">String</span></span>|<span data-ttu-id="db0f1-223">Hash do emissor de logon único.</span><span class="sxs-lookup"><span data-stu-id="db0f1-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="db0f1-224">eapXml</span><span class="sxs-lookup"><span data-stu-id="db0f1-224">eapXml</span></span>|<span data-ttu-id="db0f1-225">Binary</span><span class="sxs-lookup"><span data-stu-id="db0f1-225">Binary</span></span>|<span data-ttu-id="db0f1-226">XML EAP (Extensible Authentication Protocol).</span><span class="sxs-lookup"><span data-stu-id="db0f1-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="db0f1-227">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="db0f1-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="db0f1-228">proxyServer</span><span class="sxs-lookup"><span data-stu-id="db0f1-228">proxyServer</span></span>|[<span data-ttu-id="db0f1-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="db0f1-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="db0f1-230">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="db0f1-230">Proxy Server.</span></span>|
|<span data-ttu-id="db0f1-231">associatedApps</span><span class="sxs-lookup"><span data-stu-id="db0f1-231">associatedApps</span></span>|<span data-ttu-id="db0f1-232">coleção [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="db0f1-233">Aplicativos associados.</span><span class="sxs-lookup"><span data-stu-id="db0f1-233">Associated Apps.</span></span> <span data-ttu-id="db0f1-234">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="db0f1-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="db0f1-235">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="db0f1-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="db0f1-236">Booliano</span><span class="sxs-lookup"><span data-stu-id="db0f1-236">Boolean</span></span>|<span data-ttu-id="db0f1-237">Somente os aplicativos associados podem usar Connection (VPN por aplicativo).</span><span class="sxs-lookup"><span data-stu-id="db0f1-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="db0f1-238">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="db0f1-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="db0f1-239">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db0f1-239">String</span></span>|<span data-ttu-id="db0f1-240">Domínio de proteção de informações do Windows (WIP) a ser associado a essa conexão.</span><span class="sxs-lookup"><span data-stu-id="db0f1-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="db0f1-241">trafficRules</span><span class="sxs-lookup"><span data-stu-id="db0f1-241">trafficRules</span></span>|<span data-ttu-id="db0f1-242">coleção [vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="db0f1-243">Regras de tráfego.</span><span class="sxs-lookup"><span data-stu-id="db0f1-243">Traffic rules.</span></span> <span data-ttu-id="db0f1-244">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="db0f1-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="db0f1-245">roteie</span><span class="sxs-lookup"><span data-stu-id="db0f1-245">routes</span></span>|<span data-ttu-id="db0f1-246">coleção [vpnRoute](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="db0f1-247">Rotas (opcionais para provedores de terceiros).</span><span class="sxs-lookup"><span data-stu-id="db0f1-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="db0f1-248">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="db0f1-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="db0f1-249">dnsRules</span><span class="sxs-lookup"><span data-stu-id="db0f1-249">dnsRules</span></span>|<span data-ttu-id="db0f1-250">coleção [vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="db0f1-251">Regras de DNS.</span><span class="sxs-lookup"><span data-stu-id="db0f1-251">DNS rules.</span></span> <span data-ttu-id="db0f1-252">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="db0f1-252">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="db0f1-253">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="db0f1-253">trustedNetworkDomains</span></span>|<span data-ttu-id="db0f1-254">Coleção String</span><span class="sxs-lookup"><span data-stu-id="db0f1-254">String collection</span></span>|<span data-ttu-id="db0f1-255">Domínios de rede confiáveis</span><span class="sxs-lookup"><span data-stu-id="db0f1-255">Trusted Network Domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="db0f1-256">Relações</span><span class="sxs-lookup"><span data-stu-id="db0f1-256">Relationships</span></span>
|<span data-ttu-id="db0f1-257">Relação</span><span class="sxs-lookup"><span data-stu-id="db0f1-257">Relationship</span></span>|<span data-ttu-id="db0f1-258">Tipo</span><span class="sxs-lookup"><span data-stu-id="db0f1-258">Type</span></span>|<span data-ttu-id="db0f1-259">Descrição</span><span class="sxs-lookup"><span data-stu-id="db0f1-259">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db0f1-260">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="db0f1-260">groupAssignments</span></span>|<span data-ttu-id="db0f1-261">coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-261">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="db0f1-262">A lista de atribuições de grupo para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db0f1-262">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="db0f1-263">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-263">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-264">assignments</span><span class="sxs-lookup"><span data-stu-id="db0f1-264">assignments</span></span>|<span data-ttu-id="db0f1-265">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-265">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="db0f1-266">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db0f1-266">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="db0f1-267">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-267">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-268">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="db0f1-268">deviceStatuses</span></span>|<span data-ttu-id="db0f1-269">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-269">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="db0f1-270">Status da instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db0f1-270">Device configuration installation status by device.</span></span> <span data-ttu-id="db0f1-271">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-271">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-272">userStatuses</span><span class="sxs-lookup"><span data-stu-id="db0f1-272">userStatuses</span></span>|<span data-ttu-id="db0f1-273">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-273">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="db0f1-274">Status de instalação da configuração do dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="db0f1-274">Device configuration installation status by user.</span></span> <span data-ttu-id="db0f1-275">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-275">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-276">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="db0f1-276">deviceStatusOverview</span></span>|[<span data-ttu-id="db0f1-277">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="db0f1-277">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="db0f1-278">Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-278">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-279">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="db0f1-279">userStatusOverview</span></span>|[<span data-ttu-id="db0f1-280">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="db0f1-280">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="db0f1-281">Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-281">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-282">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="db0f1-282">deviceSettingStateSummaries</span></span>|<span data-ttu-id="db0f1-283">Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-283">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="db0f1-284">Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db0f1-284">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db0f1-285">identityCertificate</span><span class="sxs-lookup"><span data-stu-id="db0f1-285">identityCertificate</span></span>|[<span data-ttu-id="db0f1-286">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="db0f1-286">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="db0f1-287">Certificado de identidade para autenticação de cliente quando o método de autenticação é certificado.</span><span class="sxs-lookup"><span data-stu-id="db0f1-287">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db0f1-288">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db0f1-288">JSON Representation</span></span>
<span data-ttu-id="db0f1-289">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db0f1-289">Here is a JSON representation of the resource.</span></span>
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





