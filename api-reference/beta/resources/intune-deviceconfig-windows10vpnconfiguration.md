---
title: tipo de recurso de windows10VpnConfiguration
description: Fornecendo as configurações neste perfil, você poderá instruir o dispositivo Windows 10 (área de trabalho ou celular) para se conectar ao ponto de extremidade VPN desejado. Especificando os tipos de segurança e o método de autenticação esperado pelo ponto de extremidade VPN que você pode fazer a conexão VPN perfeita para usuário final.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 75710eb8d969f4bfc751405ecf6eca50ced6cfe1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406966"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="d5f33-104">tipo de recurso de windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5f33-104">windows10VpnConfiguration resource type</span></span>

> <span data-ttu-id="d5f33-105">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="d5f33-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d5f33-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d5f33-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5f33-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="d5f33-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5f33-108">Fornecendo as configurações neste perfil, você poderá instruir o dispositivo Windows 10 (área de trabalho ou celular) para se conectar ao ponto de extremidade VPN desejado.</span><span class="sxs-lookup"><span data-stu-id="d5f33-108">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="d5f33-109">Especificando os tipos de segurança e o método de autenticação esperado pelo ponto de extremidade VPN que você pode fazer a conexão VPN perfeita para usuário final.</span><span class="sxs-lookup"><span data-stu-id="d5f33-109">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="d5f33-110">Herda de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-110">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d5f33-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="d5f33-111">Methods</span></span>
|<span data-ttu-id="d5f33-112">Método</span><span class="sxs-lookup"><span data-stu-id="d5f33-112">Method</span></span>|<span data-ttu-id="d5f33-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d5f33-113">Return Type</span></span>|<span data-ttu-id="d5f33-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5f33-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d5f33-115">Lista windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="d5f33-115">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="d5f33-116">coleção [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="d5f33-117">Lista as propriedades e os relacionamentos dos objetos [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d5f33-117">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="d5f33-118">Obter windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5f33-118">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="d5f33-119">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5f33-119">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="d5f33-120">Leia as propriedades e os relacionamentos do objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d5f33-120">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d5f33-121">Criar windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5f33-121">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="d5f33-122">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5f33-122">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="d5f33-123">Crie um novo objeto de [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d5f33-123">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d5f33-124">Excluir windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5f33-124">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="d5f33-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5f33-125">None</span></span>|<span data-ttu-id="d5f33-126">Exclui um [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d5f33-126">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="d5f33-127">Atualizar windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5f33-127">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="d5f33-128">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5f33-128">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="d5f33-129">Atualize as propriedades de um objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d5f33-129">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d5f33-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5f33-130">Properties</span></span>
|<span data-ttu-id="d5f33-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5f33-131">Property</span></span>|<span data-ttu-id="d5f33-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5f33-132">Type</span></span>|<span data-ttu-id="d5f33-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5f33-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5f33-134">id</span><span class="sxs-lookup"><span data-stu-id="d5f33-134">id</span></span>|<span data-ttu-id="d5f33-135">String</span><span class="sxs-lookup"><span data-stu-id="d5f33-135">String</span></span>|<span data-ttu-id="d5f33-136">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d5f33-136">Key of the entity.</span></span> <span data-ttu-id="d5f33-137">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-137">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5f33-138">lastModifiedDateTime</span></span>|<span data-ttu-id="d5f33-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5f33-139">DateTimeOffset</span></span>|<span data-ttu-id="d5f33-140">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d5f33-140">DateTime the object was last modified.</span></span> <span data-ttu-id="d5f33-141">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d5f33-142">roleScopeTagIds</span></span>|<span data-ttu-id="d5f33-143">String collection</span><span class="sxs-lookup"><span data-stu-id="d5f33-143">String collection</span></span>|<span data-ttu-id="d5f33-144">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="d5f33-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d5f33-145">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-145">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-146">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d5f33-146">supportsScopeTags</span></span>|<span data-ttu-id="d5f33-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5f33-147">Boolean</span></span>|<span data-ttu-id="d5f33-148">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d5f33-148">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d5f33-149">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d5f33-149">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d5f33-150">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="d5f33-150">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d5f33-151">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d5f33-151">This property is read-only.</span></span> <span data-ttu-id="d5f33-152">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-152">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5f33-153">createdDateTime</span></span>|<span data-ttu-id="d5f33-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5f33-154">DateTimeOffset</span></span>|<span data-ttu-id="d5f33-155">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d5f33-155">DateTime the object was created.</span></span> <span data-ttu-id="d5f33-156">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-156">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-157">description</span><span class="sxs-lookup"><span data-stu-id="d5f33-157">description</span></span>|<span data-ttu-id="d5f33-158">String</span><span class="sxs-lookup"><span data-stu-id="d5f33-158">String</span></span>|<span data-ttu-id="d5f33-159">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5f33-159">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d5f33-160">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-160">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-161">displayName</span><span class="sxs-lookup"><span data-stu-id="d5f33-161">displayName</span></span>|<span data-ttu-id="d5f33-162">String</span><span class="sxs-lookup"><span data-stu-id="d5f33-162">String</span></span>|<span data-ttu-id="d5f33-163">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5f33-163">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d5f33-164">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-164">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-165">version</span><span class="sxs-lookup"><span data-stu-id="d5f33-165">version</span></span>|<span data-ttu-id="d5f33-166">Int32</span><span class="sxs-lookup"><span data-stu-id="d5f33-166">Int32</span></span>|<span data-ttu-id="d5f33-167">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5f33-167">Version of the device configuration.</span></span> <span data-ttu-id="d5f33-168">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-168">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-169">connectionName</span><span class="sxs-lookup"><span data-stu-id="d5f33-169">connectionName</span></span>|<span data-ttu-id="d5f33-170">String</span><span class="sxs-lookup"><span data-stu-id="d5f33-170">String</span></span>|<span data-ttu-id="d5f33-171">Nome da Conexão exibida para o usuário.</span><span class="sxs-lookup"><span data-stu-id="d5f33-171">Connection name displayed to the user.</span></span> <span data-ttu-id="d5f33-172">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-172">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-173">servidores</span><span class="sxs-lookup"><span data-stu-id="d5f33-173">servers</span></span>|<span data-ttu-id="d5f33-174">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-174">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="d5f33-175">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="d5f33-175">List of VPN Servers on the network.</span></span> <span data-ttu-id="d5f33-176">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="d5f33-176">Make sure end users can access these network locations.</span></span> <span data-ttu-id="d5f33-177">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d5f33-177">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d5f33-178">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-178">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-179">customXml</span><span class="sxs-lookup"><span data-stu-id="d5f33-179">customXml</span></span>|<span data-ttu-id="d5f33-180">Binária</span><span class="sxs-lookup"><span data-stu-id="d5f33-180">Binary</span></span>|<span data-ttu-id="d5f33-181">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="d5f33-181">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="d5f33-182">(Array de byte codificado UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-182">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-183">profileTarget</span><span class="sxs-lookup"><span data-stu-id="d5f33-183">profileTarget</span></span>|[<span data-ttu-id="d5f33-184">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="d5f33-184">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="d5f33-185">Tipo de perfil de destino.</span><span class="sxs-lookup"><span data-stu-id="d5f33-185">Profile target type.</span></span> <span data-ttu-id="d5f33-186">Os valores possíveis são: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="d5f33-186">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="d5f33-187">connectionType</span><span class="sxs-lookup"><span data-stu-id="d5f33-187">connectionType</span></span>|[<span data-ttu-id="d5f33-188">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="d5f33-188">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="d5f33-189">Tipo de Conexão.</span><span class="sxs-lookup"><span data-stu-id="d5f33-189">Connection type.</span></span> <span data-ttu-id="d5f33-190">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="d5f33-190">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="d5f33-191">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="d5f33-191">enableSplitTunneling</span></span>|<span data-ttu-id="d5f33-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5f33-192">Boolean</span></span>|<span data-ttu-id="d5f33-193">Habilite o túnel em divisão.</span><span class="sxs-lookup"><span data-stu-id="d5f33-193">Enable split tunneling.</span></span>|
|<span data-ttu-id="d5f33-194">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="d5f33-194">enableAlwaysOn</span></span>|<span data-ttu-id="d5f33-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5f33-195">Boolean</span></span>|<span data-ttu-id="d5f33-196">Habilite o modo Always On.</span><span class="sxs-lookup"><span data-stu-id="d5f33-196">Enable Always On mode.</span></span>|
|<span data-ttu-id="d5f33-197">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="d5f33-197">enableDeviceTunnel</span></span>|<span data-ttu-id="d5f33-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5f33-198">Boolean</span></span>|<span data-ttu-id="d5f33-199">Habilite o túnel de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5f33-199">Enable device tunnel.</span></span>|
|<span data-ttu-id="d5f33-200">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="d5f33-200">enableDnsRegistration</span></span>|<span data-ttu-id="d5f33-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5f33-201">Boolean</span></span>|<span data-ttu-id="d5f33-202">Habilite o registro de endereço IP com DNS interno.</span><span class="sxs-lookup"><span data-stu-id="d5f33-202">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="d5f33-203">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="d5f33-203">dnsSuffixes</span></span>|<span data-ttu-id="d5f33-204">String collection</span><span class="sxs-lookup"><span data-stu-id="d5f33-204">String collection</span></span>|<span data-ttu-id="d5f33-205">Especifica os sufixos DNS para adicionar à lista de pesquisa de DNS para rotear corretamente nomes curtos.</span><span class="sxs-lookup"><span data-stu-id="d5f33-205">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="d5f33-206">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d5f33-206">authenticationMethod</span></span>|[<span data-ttu-id="d5f33-207">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d5f33-207">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="d5f33-208">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="d5f33-208">Authentication method.</span></span> <span data-ttu-id="d5f33-209">Os valores possíveis são: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="d5f33-209">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="d5f33-210">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="d5f33-210">rememberUserCredentials</span></span>|<span data-ttu-id="d5f33-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5f33-211">Boolean</span></span>|<span data-ttu-id="d5f33-212">Lembre-se as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="d5f33-212">Remember user credentials.</span></span>|
|<span data-ttu-id="d5f33-213">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="d5f33-213">enableConditionalAccess</span></span>|<span data-ttu-id="d5f33-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5f33-214">Boolean</span></span>|<span data-ttu-id="d5f33-215">Habilite o acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="d5f33-215">Enable conditional access.</span></span>|
|<span data-ttu-id="d5f33-216">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="d5f33-216">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="d5f33-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5f33-217">Boolean</span></span>|<span data-ttu-id="d5f33-218">Habilite logon único (SSO) com o certificado alternativo.</span><span class="sxs-lookup"><span data-stu-id="d5f33-218">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="d5f33-219">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="d5f33-219">singleSignOnEku</span></span>|[<span data-ttu-id="d5f33-220">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="d5f33-220">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="d5f33-221">Single sign-on chave EKU (uso estendido).</span><span class="sxs-lookup"><span data-stu-id="d5f33-221">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="d5f33-222">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="d5f33-222">singleSignOnIssuerHash</span></span>|<span data-ttu-id="d5f33-223">String</span><span class="sxs-lookup"><span data-stu-id="d5f33-223">String</span></span>|<span data-ttu-id="d5f33-224">Hash de emissor de logon único.</span><span class="sxs-lookup"><span data-stu-id="d5f33-224">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="d5f33-225">eapXml</span><span class="sxs-lookup"><span data-stu-id="d5f33-225">eapXml</span></span>|<span data-ttu-id="d5f33-226">Binária</span><span class="sxs-lookup"><span data-stu-id="d5f33-226">Binary</span></span>|<span data-ttu-id="d5f33-227">Protocolo de autenticação extensível (EAP) XML.</span><span class="sxs-lookup"><span data-stu-id="d5f33-227">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="d5f33-228">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="d5f33-228">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="d5f33-229">proxyServer</span><span class="sxs-lookup"><span data-stu-id="d5f33-229">proxyServer</span></span>|[<span data-ttu-id="d5f33-230">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="d5f33-230">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="d5f33-231">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="d5f33-231">Proxy Server.</span></span>|
|<span data-ttu-id="d5f33-232">associatedApps</span><span class="sxs-lookup"><span data-stu-id="d5f33-232">associatedApps</span></span>|<span data-ttu-id="d5f33-233">coleção [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-233">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="d5f33-234">Aplicativos associados.</span><span class="sxs-lookup"><span data-stu-id="d5f33-234">Associated Apps.</span></span> <span data-ttu-id="d5f33-235">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d5f33-235">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d5f33-236">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="d5f33-236">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="d5f33-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5f33-237">Boolean</span></span>|<span data-ttu-id="d5f33-238">Apenas os aplicativos associados podem usar a conexão (-app VPN).</span><span class="sxs-lookup"><span data-stu-id="d5f33-238">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="d5f33-239">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="d5f33-239">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="d5f33-240">String</span><span class="sxs-lookup"><span data-stu-id="d5f33-240">String</span></span>|<span data-ttu-id="d5f33-241">Domínio de proteção de informações do Windows (WIP) para associar a essa conexão.</span><span class="sxs-lookup"><span data-stu-id="d5f33-241">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="d5f33-242">trafficRules</span><span class="sxs-lookup"><span data-stu-id="d5f33-242">trafficRules</span></span>|<span data-ttu-id="d5f33-243">coleção [vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-243">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="d5f33-244">Regras de tráfego.</span><span class="sxs-lookup"><span data-stu-id="d5f33-244">Traffic rules.</span></span> <span data-ttu-id="d5f33-245">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d5f33-245">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="d5f33-246">rotas</span><span class="sxs-lookup"><span data-stu-id="d5f33-246">routes</span></span>|<span data-ttu-id="d5f33-247">coleção [vpnRoute](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-247">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="d5f33-248">Roteia (opcional para provedores de terceiros).</span><span class="sxs-lookup"><span data-stu-id="d5f33-248">Routes (optional for third-party providers).</span></span> <span data-ttu-id="d5f33-249">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d5f33-249">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="d5f33-250">dnsRules</span><span class="sxs-lookup"><span data-stu-id="d5f33-250">dnsRules</span></span>|<span data-ttu-id="d5f33-251">coleção [vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-251">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="d5f33-252">Regras DNS.</span><span class="sxs-lookup"><span data-stu-id="d5f33-252">DNS rules.</span></span> <span data-ttu-id="d5f33-253">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d5f33-253">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="d5f33-254">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="d5f33-254">trustedNetworkDomains</span></span>|<span data-ttu-id="d5f33-255">String collection</span><span class="sxs-lookup"><span data-stu-id="d5f33-255">String collection</span></span>|<span data-ttu-id="d5f33-256">Domínios de rede de perímetro</span><span class="sxs-lookup"><span data-stu-id="d5f33-256">Trusted Network Domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5f33-257">Relações</span><span class="sxs-lookup"><span data-stu-id="d5f33-257">Relationships</span></span>
|<span data-ttu-id="d5f33-258">Relação</span><span class="sxs-lookup"><span data-stu-id="d5f33-258">Relationship</span></span>|<span data-ttu-id="d5f33-259">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5f33-259">Type</span></span>|<span data-ttu-id="d5f33-260">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5f33-260">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5f33-261">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="d5f33-261">groupAssignments</span></span>|<span data-ttu-id="d5f33-262">coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-262">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="d5f33-263">A lista de atribuições de grupo para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5f33-263">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="d5f33-264">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-264">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-265">assignments</span><span class="sxs-lookup"><span data-stu-id="d5f33-265">assignments</span></span>|<span data-ttu-id="d5f33-266">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-266">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d5f33-267">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5f33-267">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="d5f33-268">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-268">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-269">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="d5f33-269">deviceStatuses</span></span>|<span data-ttu-id="d5f33-270">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-270">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="d5f33-271">Status de instalação da configuração do dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5f33-271">Device configuration installation status by device.</span></span> <span data-ttu-id="d5f33-272">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-272">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-273">userStatuses</span><span class="sxs-lookup"><span data-stu-id="d5f33-273">userStatuses</span></span>|<span data-ttu-id="d5f33-274">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-274">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="d5f33-275">Status de instalação da configuração de dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="d5f33-275">Device configuration installation status by user.</span></span> <span data-ttu-id="d5f33-276">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-276">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-277">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="d5f33-277">deviceStatusOverview</span></span>|[<span data-ttu-id="d5f33-278">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d5f33-278">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="d5f33-279">Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-279">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-280">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="d5f33-280">userStatusOverview</span></span>|[<span data-ttu-id="d5f33-281">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="d5f33-281">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="d5f33-282">Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-282">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-283">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="d5f33-283">deviceSettingStateSummaries</span></span>|<span data-ttu-id="d5f33-284">Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-284">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="d5f33-285">Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d5f33-285">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d5f33-286">identityCertificate</span><span class="sxs-lookup"><span data-stu-id="d5f33-286">identityCertificate</span></span>|[<span data-ttu-id="d5f33-287">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="d5f33-287">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="d5f33-288">Certificado de identidade para autenticação de cliente quando o método de autenticação é o certificado.</span><span class="sxs-lookup"><span data-stu-id="d5f33-288">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5f33-289">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5f33-289">JSON Representation</span></span>
<span data-ttu-id="d5f33-290">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5f33-290">Here is a JSON representation of the resource.</span></span>
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




