---
title: tipo de recurso de windows10VpnConfiguration
description: Fornecendo as configurações neste perfil, você poderá instruir o dispositivo Windows 10 (área de trabalho ou celular) para se conectar ao ponto de extremidade VPN desejado. Especificando os tipos de segurança e o método de autenticação esperado pelo ponto de extremidade VPN que você pode fazer a conexão VPN perfeita para usuário final.
author: tfitzmac
ms.openlocfilehash: 1dbbdb5a7065214ab6a290215f2c6016f8ad74bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340695"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="1588b-104">tipo de recurso de windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1588b-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="1588b-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1588b-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1588b-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1588b-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1588b-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1588b-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1588b-108">Fornecendo as configurações neste perfil, você poderá instruir o dispositivo Windows 10 (área de trabalho ou celular) para se conectar ao ponto de extremidade VPN desejado.</span><span class="sxs-lookup"><span data-stu-id="1588b-108">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="1588b-109">Especificando os tipos de segurança e o método de autenticação esperado pelo ponto de extremidade VPN que você pode fazer a conexão VPN perfeita para usuário final.</span><span class="sxs-lookup"><span data-stu-id="1588b-109">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>

<span data-ttu-id="1588b-110">Herda de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-110">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1588b-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="1588b-111">Methods</span></span>
|<span data-ttu-id="1588b-112">Método</span><span class="sxs-lookup"><span data-stu-id="1588b-112">Method</span></span>|<span data-ttu-id="1588b-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1588b-113">Return Type</span></span>|<span data-ttu-id="1588b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="1588b-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1588b-115">Lista windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="1588b-115">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="1588b-116">coleção [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="1588b-117">Lista as propriedades e os relacionamentos dos objetos [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1588b-117">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="1588b-118">Obter windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1588b-118">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="1588b-119">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1588b-119">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="1588b-120">Leia as propriedades e os relacionamentos do objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1588b-120">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="1588b-121">Criar windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1588b-121">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="1588b-122">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1588b-122">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="1588b-123">Crie um novo objeto de [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1588b-123">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="1588b-124">Excluir windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1588b-124">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="1588b-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1588b-125">None</span></span>|<span data-ttu-id="1588b-126">Exclui um [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1588b-126">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="1588b-127">Atualizar windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1588b-127">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="1588b-128">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1588b-128">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="1588b-129">Atualize as propriedades de um objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1588b-129">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1588b-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1588b-130">Properties</span></span>
|<span data-ttu-id="1588b-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1588b-131">Property</span></span>|<span data-ttu-id="1588b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1588b-132">Type</span></span>|<span data-ttu-id="1588b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1588b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1588b-134">id</span><span class="sxs-lookup"><span data-stu-id="1588b-134">id</span></span>|<span data-ttu-id="1588b-135">String</span><span class="sxs-lookup"><span data-stu-id="1588b-135">String</span></span>|<span data-ttu-id="1588b-136">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1588b-136">Key of the entity.</span></span> <span data-ttu-id="1588b-137">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1588b-138">lastModifiedDateTime</span></span>|<span data-ttu-id="1588b-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1588b-139">DateTimeOffset</span></span>|<span data-ttu-id="1588b-140">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1588b-140">DateTime the object was last modified.</span></span> <span data-ttu-id="1588b-141">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1588b-142">roleScopeTagIds</span></span>|<span data-ttu-id="1588b-143">String collection</span><span class="sxs-lookup"><span data-stu-id="1588b-143">String collection</span></span>|<span data-ttu-id="1588b-144">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="1588b-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1588b-145">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-145">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-146">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1588b-146">supportsScopeTags</span></span>|<span data-ttu-id="1588b-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="1588b-147">Boolean</span></span>|<span data-ttu-id="1588b-148">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="1588b-148">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1588b-149">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="1588b-149">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1588b-150">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="1588b-150">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1588b-151">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1588b-151">This property is read-only.</span></span> <span data-ttu-id="1588b-152">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1588b-153">createdDateTime</span></span>|<span data-ttu-id="1588b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1588b-154">DateTimeOffset</span></span>|<span data-ttu-id="1588b-155">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1588b-155">DateTime the object was created.</span></span> <span data-ttu-id="1588b-156">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-157">description</span><span class="sxs-lookup"><span data-stu-id="1588b-157">description</span></span>|<span data-ttu-id="1588b-158">String</span><span class="sxs-lookup"><span data-stu-id="1588b-158">String</span></span>|<span data-ttu-id="1588b-159">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1588b-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1588b-160">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-161">displayName</span><span class="sxs-lookup"><span data-stu-id="1588b-161">displayName</span></span>|<span data-ttu-id="1588b-162">String</span><span class="sxs-lookup"><span data-stu-id="1588b-162">String</span></span>|<span data-ttu-id="1588b-163">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1588b-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1588b-164">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-165">version</span><span class="sxs-lookup"><span data-stu-id="1588b-165">version</span></span>|<span data-ttu-id="1588b-166">Int32</span><span class="sxs-lookup"><span data-stu-id="1588b-166">Int32</span></span>|<span data-ttu-id="1588b-167">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1588b-167">Version of the device configuration.</span></span> <span data-ttu-id="1588b-168">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-169">connectionName</span><span class="sxs-lookup"><span data-stu-id="1588b-169">connectionName</span></span>|<span data-ttu-id="1588b-170">String</span><span class="sxs-lookup"><span data-stu-id="1588b-170">String</span></span>|<span data-ttu-id="1588b-171">Nome da Conexão exibida para o usuário.</span><span class="sxs-lookup"><span data-stu-id="1588b-171">Connection name displayed to the user.</span></span> <span data-ttu-id="1588b-172">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-172">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-173">servidores</span><span class="sxs-lookup"><span data-stu-id="1588b-173">servers</span></span>|<span data-ttu-id="1588b-174">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-174">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="1588b-175">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="1588b-175">List of VPN Servers on the network.</span></span> <span data-ttu-id="1588b-176">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="1588b-176">Make sure end users can access these network locations.</span></span> <span data-ttu-id="1588b-177">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="1588b-177">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="1588b-178">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-178">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-179">customXml</span><span class="sxs-lookup"><span data-stu-id="1588b-179">customXml</span></span>|<span data-ttu-id="1588b-180">Binária</span><span class="sxs-lookup"><span data-stu-id="1588b-180">Binary</span></span>|<span data-ttu-id="1588b-181">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="1588b-181">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="1588b-182">(Array de byte codificado UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-182">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-183">profileTarget</span><span class="sxs-lookup"><span data-stu-id="1588b-183">profileTarget</span></span>|[<span data-ttu-id="1588b-184">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="1588b-184">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="1588b-185">Tipo de perfil de destino.</span><span class="sxs-lookup"><span data-stu-id="1588b-185">Profile target type.</span></span> <span data-ttu-id="1588b-186">Os valores possíveis são: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="1588b-186">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="1588b-187">connectionType</span><span class="sxs-lookup"><span data-stu-id="1588b-187">connectionType</span></span>|[<span data-ttu-id="1588b-188">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="1588b-188">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="1588b-189">Tipo de Conexão.</span><span class="sxs-lookup"><span data-stu-id="1588b-189">Connection type.</span></span> <span data-ttu-id="1588b-190">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="1588b-190">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="1588b-191">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="1588b-191">enableSplitTunneling</span></span>|<span data-ttu-id="1588b-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="1588b-192">Boolean</span></span>|<span data-ttu-id="1588b-193">Habilite o túnel em divisão.</span><span class="sxs-lookup"><span data-stu-id="1588b-193">Enable split tunneling.</span></span>|
|<span data-ttu-id="1588b-194">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="1588b-194">enableAlwaysOn</span></span>|<span data-ttu-id="1588b-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="1588b-195">Boolean</span></span>|<span data-ttu-id="1588b-196">Habilite o modo Always On.</span><span class="sxs-lookup"><span data-stu-id="1588b-196">Enable Always On mode.</span></span>|
|<span data-ttu-id="1588b-197">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="1588b-197">enableDeviceTunnel</span></span>|<span data-ttu-id="1588b-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="1588b-198">Boolean</span></span>|<span data-ttu-id="1588b-199">Habilite o túnel de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1588b-199">Enable device tunnel.</span></span>|
|<span data-ttu-id="1588b-200">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="1588b-200">enableDnsRegistration</span></span>|<span data-ttu-id="1588b-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="1588b-201">Boolean</span></span>|<span data-ttu-id="1588b-202">Habilite o registro de endereço IP com DNS interno.</span><span class="sxs-lookup"><span data-stu-id="1588b-202">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="1588b-203">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="1588b-203">dnsSuffixes</span></span>|<span data-ttu-id="1588b-204">String collection</span><span class="sxs-lookup"><span data-stu-id="1588b-204">String collection</span></span>|<span data-ttu-id="1588b-205">Especifica os sufixos DNS para adicionar à lista de pesquisa de DNS para rotear corretamente nomes curtos.</span><span class="sxs-lookup"><span data-stu-id="1588b-205">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="1588b-206">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1588b-206">authenticationMethod</span></span>|[<span data-ttu-id="1588b-207">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1588b-207">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="1588b-208">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="1588b-208">Authentication method.</span></span> <span data-ttu-id="1588b-209">Os valores possíveis são: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="1588b-209">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="1588b-210">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="1588b-210">rememberUserCredentials</span></span>|<span data-ttu-id="1588b-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="1588b-211">Boolean</span></span>|<span data-ttu-id="1588b-212">Lembre-se as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="1588b-212">Remember user credentials.</span></span>|
|<span data-ttu-id="1588b-213">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="1588b-213">enableConditionalAccess</span></span>|<span data-ttu-id="1588b-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="1588b-214">Boolean</span></span>|<span data-ttu-id="1588b-215">Habilite o acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="1588b-215">Enable conditional access.</span></span>|
|<span data-ttu-id="1588b-216">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="1588b-216">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="1588b-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="1588b-217">Boolean</span></span>|<span data-ttu-id="1588b-218">Habilite logon único (SSO) com o certificado alternativo.</span><span class="sxs-lookup"><span data-stu-id="1588b-218">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="1588b-219">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="1588b-219">singleSignOnEku</span></span>|[<span data-ttu-id="1588b-220">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="1588b-220">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="1588b-221">Single sign-on chave EKU (uso estendido).</span><span class="sxs-lookup"><span data-stu-id="1588b-221">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="1588b-222">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="1588b-222">singleSignOnIssuerHash</span></span>|<span data-ttu-id="1588b-223">String</span><span class="sxs-lookup"><span data-stu-id="1588b-223">String</span></span>|<span data-ttu-id="1588b-224">Hash de emissor de logon único.</span><span class="sxs-lookup"><span data-stu-id="1588b-224">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="1588b-225">eapXml</span><span class="sxs-lookup"><span data-stu-id="1588b-225">eapXml</span></span>|<span data-ttu-id="1588b-226">Binária</span><span class="sxs-lookup"><span data-stu-id="1588b-226">Binary</span></span>|<span data-ttu-id="1588b-227">Protocolo de autenticação extensível (EAP) XML.</span><span class="sxs-lookup"><span data-stu-id="1588b-227">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="1588b-228">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="1588b-228">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="1588b-229">proxyServer</span><span class="sxs-lookup"><span data-stu-id="1588b-229">proxyServer</span></span>|[<span data-ttu-id="1588b-230">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="1588b-230">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="1588b-231">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="1588b-231">Proxy Server.</span></span>|
|<span data-ttu-id="1588b-232">associatedApps</span><span class="sxs-lookup"><span data-stu-id="1588b-232">associatedApps</span></span>|<span data-ttu-id="1588b-233">coleção [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-233">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="1588b-234">Aplicativos associados.</span><span class="sxs-lookup"><span data-stu-id="1588b-234">Associated Apps.</span></span> <span data-ttu-id="1588b-235">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="1588b-235">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="1588b-236">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="1588b-236">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="1588b-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="1588b-237">Boolean</span></span>|<span data-ttu-id="1588b-238">Apenas os aplicativos associados podem usar a conexão (-app VPN).</span><span class="sxs-lookup"><span data-stu-id="1588b-238">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="1588b-239">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="1588b-239">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="1588b-240">String</span><span class="sxs-lookup"><span data-stu-id="1588b-240">String</span></span>|<span data-ttu-id="1588b-241">Domínio de proteção de informações do Windows (WIP) para associar a essa conexão.</span><span class="sxs-lookup"><span data-stu-id="1588b-241">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="1588b-242">trafficRules</span><span class="sxs-lookup"><span data-stu-id="1588b-242">trafficRules</span></span>|<span data-ttu-id="1588b-243">coleção [vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-243">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="1588b-244">Regras de tráfego.</span><span class="sxs-lookup"><span data-stu-id="1588b-244">Traffic rules.</span></span> <span data-ttu-id="1588b-245">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="1588b-245">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="1588b-246">rotas</span><span class="sxs-lookup"><span data-stu-id="1588b-246">routes</span></span>|<span data-ttu-id="1588b-247">coleção [vpnRoute](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-247">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="1588b-248">Roteia (opcional para provedores de terceiros).</span><span class="sxs-lookup"><span data-stu-id="1588b-248">Routes (optional for third-party providers).</span></span> <span data-ttu-id="1588b-249">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="1588b-249">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="1588b-250">dnsRules</span><span class="sxs-lookup"><span data-stu-id="1588b-250">dnsRules</span></span>|<span data-ttu-id="1588b-251">coleção [vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-251">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="1588b-252">Regras DNS.</span><span class="sxs-lookup"><span data-stu-id="1588b-252">DNS rules.</span></span> <span data-ttu-id="1588b-253">Essa coleção pode conter um máximo de 1000 elementos.</span><span class="sxs-lookup"><span data-stu-id="1588b-253">This collection can contain a maximum of 1000 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1588b-254">Relações</span><span class="sxs-lookup"><span data-stu-id="1588b-254">Relationships</span></span>
|<span data-ttu-id="1588b-255">Relação</span><span class="sxs-lookup"><span data-stu-id="1588b-255">Relationship</span></span>|<span data-ttu-id="1588b-256">Tipo</span><span class="sxs-lookup"><span data-stu-id="1588b-256">Type</span></span>|<span data-ttu-id="1588b-257">Descrição</span><span class="sxs-lookup"><span data-stu-id="1588b-257">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1588b-258">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="1588b-258">groupAssignments</span></span>|<span data-ttu-id="1588b-259">coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-259">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="1588b-260">A lista de atribuições de grupo para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1588b-260">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="1588b-261">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-261">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-262">assignments</span><span class="sxs-lookup"><span data-stu-id="1588b-262">assignments</span></span>|<span data-ttu-id="1588b-263">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-263">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="1588b-264">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1588b-264">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="1588b-265">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-265">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-266">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="1588b-266">deviceStatuses</span></span>|<span data-ttu-id="1588b-267">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-267">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="1588b-268">Status de instalação da configuração do dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1588b-268">Device configuration installation status by device.</span></span> <span data-ttu-id="1588b-269">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-269">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-270">userStatuses</span><span class="sxs-lookup"><span data-stu-id="1588b-270">userStatuses</span></span>|<span data-ttu-id="1588b-271">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-271">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="1588b-272">Status de instalação da configuração de dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="1588b-272">Device configuration installation status by user.</span></span> <span data-ttu-id="1588b-273">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-273">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-274">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="1588b-274">deviceStatusOverview</span></span>|[<span data-ttu-id="1588b-275">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1588b-275">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="1588b-276">Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-276">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-277">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="1588b-277">userStatusOverview</span></span>|[<span data-ttu-id="1588b-278">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="1588b-278">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="1588b-279">Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-279">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-280">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="1588b-280">deviceSettingStateSummaries</span></span>|<span data-ttu-id="1588b-281">Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-281">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="1588b-282">Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1588b-282">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1588b-283">identityCertificate</span><span class="sxs-lookup"><span data-stu-id="1588b-283">identityCertificate</span></span>|[<span data-ttu-id="1588b-284">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="1588b-284">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="1588b-285">Certificado de identidade para autenticação de cliente quando o método de autenticação é o certificado.</span><span class="sxs-lookup"><span data-stu-id="1588b-285">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1588b-286">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1588b-286">JSON Representation</span></span>
<span data-ttu-id="1588b-287">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1588b-287">Here is a JSON representation of the resource.</span></span>
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
      "proxyServerUri": "String"
    }
  ]
}
```





