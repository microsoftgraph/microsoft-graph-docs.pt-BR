---
title: tipo de recurso windows10VpnConfiguration
description: Ao fornecer as configurações neste perfil, você pode instruir o dispositivo Windows 10 (desktop ou celular) a se conectar ao ponto de extremidade VPN desejado. Especificando o método de autenticação e os tipos de segurança esperados pelo ponto de extremidade da VPN, você pode tornar a conexão VPN perfeita para o usuário final.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76defe09de427d6c49e1081d37f91813b4ab2444
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729600"
---
# <a name="windows10vpnconfiguration-resource-type"></a><span data-ttu-id="64aef-104">tipo de recurso windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="64aef-104">windows10VpnConfiguration resource type</span></span>

<span data-ttu-id="64aef-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64aef-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64aef-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64aef-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64aef-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64aef-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64aef-108">Ao fornecer as configurações neste perfil, você pode instruir o dispositivo Windows 10 (desktop ou celular) a se conectar ao ponto de extremidade VPN desejado.</span><span class="sxs-lookup"><span data-stu-id="64aef-108">By providing the configurations in this profile you can instruct the Windows 10 device (desktop or mobile) to connect to desired VPN endpoint.</span></span> <span data-ttu-id="64aef-109">Especificando o método de autenticação e os tipos de segurança esperados pelo ponto de extremidade da VPN, você pode tornar a conexão VPN perfeita para o usuário final.</span><span class="sxs-lookup"><span data-stu-id="64aef-109">By specifying the authentication method and security types expected by VPN endpoint you can make the VPN connection seamless for end user.</span></span>


<span data-ttu-id="64aef-110">Herda de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-110">Inherits from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="64aef-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="64aef-111">Methods</span></span>
|<span data-ttu-id="64aef-112">Método</span><span class="sxs-lookup"><span data-stu-id="64aef-112">Method</span></span>|<span data-ttu-id="64aef-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="64aef-113">Return Type</span></span>|<span data-ttu-id="64aef-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="64aef-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="64aef-115">Listar windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="64aef-115">List windows10VpnConfigurations</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|<span data-ttu-id="64aef-116">coleção [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-116">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) collection</span></span>|<span data-ttu-id="64aef-117">Listar Propriedades e relações dos objetos [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="64aef-117">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="64aef-118">Obter windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="64aef-118">Get windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[<span data-ttu-id="64aef-119">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="64aef-119">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="64aef-120">Leia as propriedades e as relações do objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="64aef-120">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="64aef-121">Criar windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="64aef-121">Create windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[<span data-ttu-id="64aef-122">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="64aef-122">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="64aef-123">Criar um novo objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="64aef-123">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|
|[<span data-ttu-id="64aef-124">Excluir windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="64aef-124">Delete windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|<span data-ttu-id="64aef-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64aef-125">None</span></span>|<span data-ttu-id="64aef-126">Exclui [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="64aef-126">Deletes a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md).</span></span>|
|[<span data-ttu-id="64aef-127">Atualizar windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="64aef-127">Update windows10VpnConfiguration</span></span>](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[<span data-ttu-id="64aef-128">windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="64aef-128">windows10VpnConfiguration</span></span>](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|<span data-ttu-id="64aef-129">Atualiza as propriedades de um objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="64aef-129">Update the properties of a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="64aef-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64aef-130">Properties</span></span>
|<span data-ttu-id="64aef-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64aef-131">Property</span></span>|<span data-ttu-id="64aef-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="64aef-132">Type</span></span>|<span data-ttu-id="64aef-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="64aef-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64aef-134">id</span><span class="sxs-lookup"><span data-stu-id="64aef-134">id</span></span>|<span data-ttu-id="64aef-135">String</span><span class="sxs-lookup"><span data-stu-id="64aef-135">String</span></span>|<span data-ttu-id="64aef-136">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="64aef-136">Key of the entity.</span></span> <span data-ttu-id="64aef-137">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-137">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64aef-138">lastModifiedDateTime</span></span>|<span data-ttu-id="64aef-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64aef-139">DateTimeOffset</span></span>|<span data-ttu-id="64aef-140">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="64aef-140">DateTime the object was last modified.</span></span> <span data-ttu-id="64aef-141">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-141">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-142">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="64aef-142">roleScopeTagIds</span></span>|<span data-ttu-id="64aef-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="64aef-143">String collection</span></span>|<span data-ttu-id="64aef-144">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="64aef-144">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="64aef-145">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-145">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-146">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="64aef-146">supportsScopeTags</span></span>|<span data-ttu-id="64aef-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="64aef-147">Boolean</span></span>|<span data-ttu-id="64aef-148">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="64aef-148">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="64aef-149">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="64aef-149">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="64aef-150">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="64aef-150">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="64aef-151">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="64aef-151">This property is read-only.</span></span> <span data-ttu-id="64aef-152">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-152">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="64aef-153">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="64aef-154">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="64aef-154">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="64aef-155">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="64aef-155">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="64aef-156">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-156">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="64aef-157">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="64aef-158">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="64aef-158">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="64aef-159">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="64aef-159">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="64aef-160">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-160">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="64aef-161">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="64aef-162">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="64aef-162">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="64aef-163">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="64aef-163">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="64aef-164">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-164">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-165">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64aef-165">createdDateTime</span></span>|<span data-ttu-id="64aef-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64aef-166">DateTimeOffset</span></span>|<span data-ttu-id="64aef-167">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="64aef-167">DateTime the object was created.</span></span> <span data-ttu-id="64aef-168">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-168">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-169">description</span><span class="sxs-lookup"><span data-stu-id="64aef-169">description</span></span>|<span data-ttu-id="64aef-170">String</span><span class="sxs-lookup"><span data-stu-id="64aef-170">String</span></span>|<span data-ttu-id="64aef-171">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64aef-171">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="64aef-172">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-172">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-173">displayName</span><span class="sxs-lookup"><span data-stu-id="64aef-173">displayName</span></span>|<span data-ttu-id="64aef-174">String</span><span class="sxs-lookup"><span data-stu-id="64aef-174">String</span></span>|<span data-ttu-id="64aef-175">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64aef-175">Admin provided name of the device configuration.</span></span> <span data-ttu-id="64aef-176">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-176">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-177">versão</span><span class="sxs-lookup"><span data-stu-id="64aef-177">version</span></span>|<span data-ttu-id="64aef-178">Int32</span><span class="sxs-lookup"><span data-stu-id="64aef-178">Int32</span></span>|<span data-ttu-id="64aef-179">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64aef-179">Version of the device configuration.</span></span> <span data-ttu-id="64aef-180">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-180">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-181">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="64aef-181">connectionName</span></span>|<span data-ttu-id="64aef-182">String</span><span class="sxs-lookup"><span data-stu-id="64aef-182">String</span></span>|<span data-ttu-id="64aef-183">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="64aef-183">Connection name displayed to the user.</span></span> <span data-ttu-id="64aef-184">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-184">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-185">servidores</span><span class="sxs-lookup"><span data-stu-id="64aef-185">servers</span></span>|<span data-ttu-id="64aef-186">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-186">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="64aef-187">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="64aef-187">List of VPN Servers on the network.</span></span> <span data-ttu-id="64aef-188">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="64aef-188">Make sure end users can access these network locations.</span></span> <span data-ttu-id="64aef-189">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="64aef-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="64aef-190">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-190">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-191">customXml</span><span class="sxs-lookup"><span data-stu-id="64aef-191">customXml</span></span>|<span data-ttu-id="64aef-192">Binária</span><span class="sxs-lookup"><span data-stu-id="64aef-192">Binary</span></span>|<span data-ttu-id="64aef-193">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="64aef-193">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="64aef-194">(Matriz de bytes codificados por UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-194">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-195">profileTarget</span><span class="sxs-lookup"><span data-stu-id="64aef-195">profileTarget</span></span>|[<span data-ttu-id="64aef-196">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="64aef-196">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="64aef-197">Tipo de destino do perfil.</span><span class="sxs-lookup"><span data-stu-id="64aef-197">Profile target type.</span></span> <span data-ttu-id="64aef-198">Os valores possíveis são: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="64aef-198">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="64aef-199">Connection</span><span class="sxs-lookup"><span data-stu-id="64aef-199">connectionType</span></span>|[<span data-ttu-id="64aef-200">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="64aef-200">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="64aef-201">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="64aef-201">Connection type.</span></span> <span data-ttu-id="64aef-202">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="64aef-202">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="64aef-203">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="64aef-203">enableSplitTunneling</span></span>|<span data-ttu-id="64aef-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="64aef-204">Boolean</span></span>|<span data-ttu-id="64aef-205">Habilitar o túnel de divisão.</span><span class="sxs-lookup"><span data-stu-id="64aef-205">Enable split tunneling.</span></span>|
|<span data-ttu-id="64aef-206">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="64aef-206">enableAlwaysOn</span></span>|<span data-ttu-id="64aef-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="64aef-207">Boolean</span></span>|<span data-ttu-id="64aef-208">Habilitar o modo Always on.</span><span class="sxs-lookup"><span data-stu-id="64aef-208">Enable Always On mode.</span></span>|
|<span data-ttu-id="64aef-209">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="64aef-209">enableDeviceTunnel</span></span>|<span data-ttu-id="64aef-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="64aef-210">Boolean</span></span>|<span data-ttu-id="64aef-211">Habilitar o túnel de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64aef-211">Enable device tunnel.</span></span>|
|<span data-ttu-id="64aef-212">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="64aef-212">enableDnsRegistration</span></span>|<span data-ttu-id="64aef-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="64aef-213">Boolean</span></span>|<span data-ttu-id="64aef-214">Habilitar o registro de endereço IP com DNS interno.</span><span class="sxs-lookup"><span data-stu-id="64aef-214">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="64aef-215">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="64aef-215">dnsSuffixes</span></span>|<span data-ttu-id="64aef-216">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="64aef-216">String collection</span></span>|<span data-ttu-id="64aef-217">Especifique sufixos DNS para adicionar à lista de pesquisa de DNS para rotear corretamente nomes curtos.</span><span class="sxs-lookup"><span data-stu-id="64aef-217">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="64aef-218">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="64aef-218">authenticationMethod</span></span>|[<span data-ttu-id="64aef-219">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="64aef-219">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="64aef-220">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="64aef-220">Authentication method.</span></span> <span data-ttu-id="64aef-221">Os valores possíveis são: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="64aef-221">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span></span>|
|<span data-ttu-id="64aef-222">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="64aef-222">rememberUserCredentials</span></span>|<span data-ttu-id="64aef-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="64aef-223">Boolean</span></span>|<span data-ttu-id="64aef-224">Lembrar as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="64aef-224">Remember user credentials.</span></span>|
|<span data-ttu-id="64aef-225">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="64aef-225">enableConditionalAccess</span></span>|<span data-ttu-id="64aef-226">Booliano</span><span class="sxs-lookup"><span data-stu-id="64aef-226">Boolean</span></span>|<span data-ttu-id="64aef-227">Habilitar o acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="64aef-227">Enable conditional access.</span></span>|
|<span data-ttu-id="64aef-228">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="64aef-228">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="64aef-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="64aef-229">Boolean</span></span>|<span data-ttu-id="64aef-230">Habilitar o logon único (SSO) com certificado alternativo.</span><span class="sxs-lookup"><span data-stu-id="64aef-230">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="64aef-231">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="64aef-231">singleSignOnEku</span></span>|[<span data-ttu-id="64aef-232">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="64aef-232">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="64aef-233">Uso de chave estendida (EKU) de logon único.</span><span class="sxs-lookup"><span data-stu-id="64aef-233">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="64aef-234">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="64aef-234">singleSignOnIssuerHash</span></span>|<span data-ttu-id="64aef-235">String</span><span class="sxs-lookup"><span data-stu-id="64aef-235">String</span></span>|<span data-ttu-id="64aef-236">Hash do emissor de logon único.</span><span class="sxs-lookup"><span data-stu-id="64aef-236">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="64aef-237">eapXml</span><span class="sxs-lookup"><span data-stu-id="64aef-237">eapXml</span></span>|<span data-ttu-id="64aef-238">Binária</span><span class="sxs-lookup"><span data-stu-id="64aef-238">Binary</span></span>|<span data-ttu-id="64aef-239">XML EAP (Extensible Authentication Protocol).</span><span class="sxs-lookup"><span data-stu-id="64aef-239">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="64aef-240">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="64aef-240">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="64aef-241">proxyServer</span><span class="sxs-lookup"><span data-stu-id="64aef-241">proxyServer</span></span>|[<span data-ttu-id="64aef-242">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="64aef-242">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="64aef-243">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="64aef-243">Proxy Server.</span></span>|
|<span data-ttu-id="64aef-244">associatedApps</span><span class="sxs-lookup"><span data-stu-id="64aef-244">associatedApps</span></span>|<span data-ttu-id="64aef-245">coleção [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-245">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="64aef-246">Aplicativos associados.</span><span class="sxs-lookup"><span data-stu-id="64aef-246">Associated Apps.</span></span> <span data-ttu-id="64aef-247">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="64aef-247">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="64aef-248">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="64aef-248">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="64aef-249">Booliano</span><span class="sxs-lookup"><span data-stu-id="64aef-249">Boolean</span></span>|<span data-ttu-id="64aef-250">Somente os aplicativos associados podem usar Connection (VPN por aplicativo).</span><span class="sxs-lookup"><span data-stu-id="64aef-250">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="64aef-251">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="64aef-251">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="64aef-252">String</span><span class="sxs-lookup"><span data-stu-id="64aef-252">String</span></span>|<span data-ttu-id="64aef-253">Domínio de proteção de informações do Windows (WIP) a ser associado a essa conexão.</span><span class="sxs-lookup"><span data-stu-id="64aef-253">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="64aef-254">trafficRules</span><span class="sxs-lookup"><span data-stu-id="64aef-254">trafficRules</span></span>|<span data-ttu-id="64aef-255">coleção [vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-255">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="64aef-256">Regras de tráfego.</span><span class="sxs-lookup"><span data-stu-id="64aef-256">Traffic rules.</span></span> <span data-ttu-id="64aef-257">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="64aef-257">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="64aef-258">roteie</span><span class="sxs-lookup"><span data-stu-id="64aef-258">routes</span></span>|<span data-ttu-id="64aef-259">coleção [vpnRoute](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-259">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="64aef-260">Rotas (opcionais para provedores de terceiros).</span><span class="sxs-lookup"><span data-stu-id="64aef-260">Routes (optional for third-party providers).</span></span> <span data-ttu-id="64aef-261">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="64aef-261">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="64aef-262">dnsRules</span><span class="sxs-lookup"><span data-stu-id="64aef-262">dnsRules</span></span>|<span data-ttu-id="64aef-263">coleção [vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-263">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="64aef-264">Regras de DNS.</span><span class="sxs-lookup"><span data-stu-id="64aef-264">DNS rules.</span></span> <span data-ttu-id="64aef-265">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="64aef-265">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="64aef-266">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="64aef-266">trustedNetworkDomains</span></span>|<span data-ttu-id="64aef-267">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="64aef-267">String collection</span></span>|<span data-ttu-id="64aef-268">Domínios de rede confiáveis</span><span class="sxs-lookup"><span data-stu-id="64aef-268">Trusted Network Domains</span></span>|
|<span data-ttu-id="64aef-269">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="64aef-269">cryptographySuite</span></span>|[<span data-ttu-id="64aef-270">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="64aef-270">cryptographySuite</span></span>](../resources/intune-deviceconfig-cryptographysuite.md)|<span data-ttu-id="64aef-271">Configurações de segurança do pacote de criptografia para VPN IKEv2 no Windows10 e superior</span><span class="sxs-lookup"><span data-stu-id="64aef-271">Cryptography Suite security settings for IKEv2 VPN in Windows10 and above</span></span> |

## <a name="relationships"></a><span data-ttu-id="64aef-272">Relações</span><span class="sxs-lookup"><span data-stu-id="64aef-272">Relationships</span></span>
|<span data-ttu-id="64aef-273">Relação</span><span class="sxs-lookup"><span data-stu-id="64aef-273">Relationship</span></span>|<span data-ttu-id="64aef-274">Tipo</span><span class="sxs-lookup"><span data-stu-id="64aef-274">Type</span></span>|<span data-ttu-id="64aef-275">Descrição</span><span class="sxs-lookup"><span data-stu-id="64aef-275">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64aef-276">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="64aef-276">groupAssignments</span></span>|<span data-ttu-id="64aef-277">coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-277">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="64aef-278">A lista de atribuições de grupo para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64aef-278">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="64aef-279">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-279">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-280">assignments</span><span class="sxs-lookup"><span data-stu-id="64aef-280">assignments</span></span>|<span data-ttu-id="64aef-281">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-281">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="64aef-282">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64aef-282">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="64aef-283">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-283">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-284">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="64aef-284">deviceStatuses</span></span>|<span data-ttu-id="64aef-285">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-285">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="64aef-286">Status da instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="64aef-286">Device configuration installation status by device.</span></span> <span data-ttu-id="64aef-287">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-287">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-288">userStatuses</span><span class="sxs-lookup"><span data-stu-id="64aef-288">userStatuses</span></span>|<span data-ttu-id="64aef-289">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-289">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="64aef-290">Status de instalação da configuração do dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="64aef-290">Device configuration installation status by user.</span></span> <span data-ttu-id="64aef-291">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-291">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-292">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="64aef-292">deviceStatusOverview</span></span>|[<span data-ttu-id="64aef-293">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="64aef-293">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="64aef-294">Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-294">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-295">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="64aef-295">userStatusOverview</span></span>|[<span data-ttu-id="64aef-296">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="64aef-296">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="64aef-297">Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-297">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-298">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="64aef-298">deviceSettingStateSummaries</span></span>|<span data-ttu-id="64aef-299">Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-299">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="64aef-300">Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="64aef-300">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64aef-301">identityCertificate</span><span class="sxs-lookup"><span data-stu-id="64aef-301">identityCertificate</span></span>|[<span data-ttu-id="64aef-302">windowsCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="64aef-302">windowsCertificateProfileBase</span></span>](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|<span data-ttu-id="64aef-303">Certificado de identidade para autenticação de cliente quando o método de autenticação é certificado.</span><span class="sxs-lookup"><span data-stu-id="64aef-303">Identity certificate for client authentication when authentication method is certificate.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64aef-304">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64aef-304">JSON Representation</span></span>
<span data-ttu-id="64aef-305">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64aef-305">Here is a JSON representation of the resource.</span></span>
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
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
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
  ],
  "cryptographySuite": {
    "@odata.type": "microsoft.graph.cryptographySuite",
    "encryptionMethod": "String",
    "integrityCheckMethod": "String",
    "dhGroup": "String",
    "cipherTransformConstants": "String",
    "authenticationTransformConstants": "String",
    "pfsGroup": "String"
  }
}
```





