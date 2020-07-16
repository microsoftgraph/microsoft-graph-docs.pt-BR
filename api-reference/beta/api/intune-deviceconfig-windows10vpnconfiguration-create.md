---
title: Criar windows10VpnConfiguration
description: Criar um novo objeto windows10VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 05eb4933fa63e04010f65c563bc3265ac1a5b92f
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122830"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="942f7-103">Criar windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="942f7-103">Create windows10VpnConfiguration</span></span>

<span data-ttu-id="942f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="942f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="942f7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="942f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="942f7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="942f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="942f7-107">Criar um novo objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="942f7-107">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="942f7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="942f7-108">Prerequisites</span></span>
<span data-ttu-id="942f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="942f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="942f7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="942f7-111">Permission type</span></span>|<span data-ttu-id="942f7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="942f7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="942f7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="942f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="942f7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="942f7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="942f7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="942f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="942f7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="942f7-116">Not supported.</span></span>|
|<span data-ttu-id="942f7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="942f7-117">Application</span></span>|<span data-ttu-id="942f7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="942f7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="942f7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="942f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="942f7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="942f7-120">Request headers</span></span>
|<span data-ttu-id="942f7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="942f7-121">Header</span></span>|<span data-ttu-id="942f7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="942f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="942f7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="942f7-123">Authorization</span></span>|<span data-ttu-id="942f7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="942f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="942f7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="942f7-125">Accept</span></span>|<span data-ttu-id="942f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="942f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="942f7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="942f7-127">Request body</span></span>
<span data-ttu-id="942f7-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="942f7-128">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="942f7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="942f7-129">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="942f7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="942f7-130">Property</span></span>|<span data-ttu-id="942f7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="942f7-131">Type</span></span>|<span data-ttu-id="942f7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="942f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="942f7-133">id</span><span class="sxs-lookup"><span data-stu-id="942f7-133">id</span></span>|<span data-ttu-id="942f7-134">String</span><span class="sxs-lookup"><span data-stu-id="942f7-134">String</span></span>|<span data-ttu-id="942f7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="942f7-135">Key of the entity.</span></span> <span data-ttu-id="942f7-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="942f7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="942f7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="942f7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="942f7-138">DateTimeOffset</span></span>|<span data-ttu-id="942f7-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="942f7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="942f7-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="942f7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="942f7-141">roleScopeTagIds</span></span>|<span data-ttu-id="942f7-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="942f7-142">String collection</span></span>|<span data-ttu-id="942f7-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="942f7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="942f7-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="942f7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="942f7-145">supportsScopeTags</span></span>|<span data-ttu-id="942f7-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="942f7-146">Boolean</span></span>|<span data-ttu-id="942f7-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="942f7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="942f7-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="942f7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="942f7-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="942f7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="942f7-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="942f7-150">This property is read-only.</span></span> <span data-ttu-id="942f7-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="942f7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="942f7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="942f7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="942f7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="942f7-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="942f7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="942f7-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="942f7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="942f7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="942f7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="942f7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="942f7-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="942f7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="942f7-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="942f7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="942f7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="942f7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="942f7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="942f7-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="942f7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="942f7-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="942f7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="942f7-164">createdDateTime</span></span>|<span data-ttu-id="942f7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="942f7-165">DateTimeOffset</span></span>|<span data-ttu-id="942f7-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="942f7-166">DateTime the object was created.</span></span> <span data-ttu-id="942f7-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="942f7-168">descrição</span><span class="sxs-lookup"><span data-stu-id="942f7-168">description</span></span>|<span data-ttu-id="942f7-169">String</span><span class="sxs-lookup"><span data-stu-id="942f7-169">String</span></span>|<span data-ttu-id="942f7-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="942f7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="942f7-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="942f7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="942f7-172">displayName</span></span>|<span data-ttu-id="942f7-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="942f7-173">String</span></span>|<span data-ttu-id="942f7-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="942f7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="942f7-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="942f7-176">versão</span><span class="sxs-lookup"><span data-stu-id="942f7-176">version</span></span>|<span data-ttu-id="942f7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="942f7-177">Int32</span></span>|<span data-ttu-id="942f7-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="942f7-178">Version of the device configuration.</span></span> <span data-ttu-id="942f7-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="942f7-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="942f7-180">connectionName</span></span>|<span data-ttu-id="942f7-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="942f7-181">String</span></span>|<span data-ttu-id="942f7-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="942f7-182">Connection name displayed to the user.</span></span> <span data-ttu-id="942f7-183">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="942f7-184">servidores</span><span class="sxs-lookup"><span data-stu-id="942f7-184">servers</span></span>|<span data-ttu-id="942f7-185">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="942f7-186">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="942f7-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="942f7-187">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="942f7-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="942f7-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="942f7-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="942f7-189">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="942f7-190">customXml</span><span class="sxs-lookup"><span data-stu-id="942f7-190">customXml</span></span>|<span data-ttu-id="942f7-191">Binária</span><span class="sxs-lookup"><span data-stu-id="942f7-191">Binary</span></span>|<span data-ttu-id="942f7-192">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="942f7-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="942f7-193">(Matriz de bytes codificados por UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="942f7-194">profileTarget</span><span class="sxs-lookup"><span data-stu-id="942f7-194">profileTarget</span></span>|[<span data-ttu-id="942f7-195">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="942f7-195">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="942f7-196">Tipo de destino do perfil.</span><span class="sxs-lookup"><span data-stu-id="942f7-196">Profile target type.</span></span> <span data-ttu-id="942f7-197">Os valores possíveis são: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="942f7-197">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="942f7-198">Connection</span><span class="sxs-lookup"><span data-stu-id="942f7-198">connectionType</span></span>|[<span data-ttu-id="942f7-199">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="942f7-199">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="942f7-200">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="942f7-200">Connection type.</span></span> <span data-ttu-id="942f7-201">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="942f7-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="942f7-202">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="942f7-202">enableSplitTunneling</span></span>|<span data-ttu-id="942f7-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="942f7-203">Boolean</span></span>|<span data-ttu-id="942f7-204">Habilitar o túnel de divisão.</span><span class="sxs-lookup"><span data-stu-id="942f7-204">Enable split tunneling.</span></span>|
|<span data-ttu-id="942f7-205">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="942f7-205">enableAlwaysOn</span></span>|<span data-ttu-id="942f7-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="942f7-206">Boolean</span></span>|<span data-ttu-id="942f7-207">Habilitar o modo Always on.</span><span class="sxs-lookup"><span data-stu-id="942f7-207">Enable Always On mode.</span></span>|
|<span data-ttu-id="942f7-208">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="942f7-208">enableDeviceTunnel</span></span>|<span data-ttu-id="942f7-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="942f7-209">Boolean</span></span>|<span data-ttu-id="942f7-210">Habilitar o túnel de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="942f7-210">Enable device tunnel.</span></span>|
|<span data-ttu-id="942f7-211">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="942f7-211">enableDnsRegistration</span></span>|<span data-ttu-id="942f7-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="942f7-212">Boolean</span></span>|<span data-ttu-id="942f7-213">Habilitar o registro de endereço IP com DNS interno.</span><span class="sxs-lookup"><span data-stu-id="942f7-213">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="942f7-214">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="942f7-214">dnsSuffixes</span></span>|<span data-ttu-id="942f7-215">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="942f7-215">String collection</span></span>|<span data-ttu-id="942f7-216">Especifique sufixos DNS para adicionar à lista de pesquisa de DNS para rotear corretamente nomes curtos.</span><span class="sxs-lookup"><span data-stu-id="942f7-216">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="942f7-217">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="942f7-217">authenticationMethod</span></span>|[<span data-ttu-id="942f7-218">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="942f7-218">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="942f7-219">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="942f7-219">Authentication method.</span></span> <span data-ttu-id="942f7-220">Os valores possíveis são: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="942f7-220">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`, `derivedCredential`.</span></span>|
|<span data-ttu-id="942f7-221">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="942f7-221">rememberUserCredentials</span></span>|<span data-ttu-id="942f7-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="942f7-222">Boolean</span></span>|<span data-ttu-id="942f7-223">Lembrar as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="942f7-223">Remember user credentials.</span></span>|
|<span data-ttu-id="942f7-224">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="942f7-224">enableConditionalAccess</span></span>|<span data-ttu-id="942f7-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="942f7-225">Boolean</span></span>|<span data-ttu-id="942f7-226">Habilitar o acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="942f7-226">Enable conditional access.</span></span>|
|<span data-ttu-id="942f7-227">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="942f7-227">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="942f7-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="942f7-228">Boolean</span></span>|<span data-ttu-id="942f7-229">Habilitar o logon único (SSO) com certificado alternativo.</span><span class="sxs-lookup"><span data-stu-id="942f7-229">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="942f7-230">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="942f7-230">singleSignOnEku</span></span>|[<span data-ttu-id="942f7-231">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="942f7-231">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="942f7-232">Uso de chave estendida (EKU) de logon único.</span><span class="sxs-lookup"><span data-stu-id="942f7-232">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="942f7-233">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="942f7-233">singleSignOnIssuerHash</span></span>|<span data-ttu-id="942f7-234">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="942f7-234">String</span></span>|<span data-ttu-id="942f7-235">Hash do emissor de logon único.</span><span class="sxs-lookup"><span data-stu-id="942f7-235">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="942f7-236">eapXml</span><span class="sxs-lookup"><span data-stu-id="942f7-236">eapXml</span></span>|<span data-ttu-id="942f7-237">Binária</span><span class="sxs-lookup"><span data-stu-id="942f7-237">Binary</span></span>|<span data-ttu-id="942f7-238">XML EAP (Extensible Authentication Protocol).</span><span class="sxs-lookup"><span data-stu-id="942f7-238">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="942f7-239">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="942f7-239">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="942f7-240">proxyServer</span><span class="sxs-lookup"><span data-stu-id="942f7-240">proxyServer</span></span>|[<span data-ttu-id="942f7-241">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="942f7-241">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="942f7-242">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="942f7-242">Proxy Server.</span></span>|
|<span data-ttu-id="942f7-243">associatedApps</span><span class="sxs-lookup"><span data-stu-id="942f7-243">associatedApps</span></span>|<span data-ttu-id="942f7-244">coleção [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-244">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="942f7-245">Aplicativos associados.</span><span class="sxs-lookup"><span data-stu-id="942f7-245">Associated Apps.</span></span> <span data-ttu-id="942f7-246">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="942f7-246">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="942f7-247">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="942f7-247">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="942f7-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="942f7-248">Boolean</span></span>|<span data-ttu-id="942f7-249">Somente os aplicativos associados podem usar Connection (VPN por aplicativo).</span><span class="sxs-lookup"><span data-stu-id="942f7-249">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="942f7-250">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="942f7-250">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="942f7-251">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="942f7-251">String</span></span>|<span data-ttu-id="942f7-252">Domínio de proteção de informações do Windows (WIP) a ser associado a essa conexão.</span><span class="sxs-lookup"><span data-stu-id="942f7-252">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="942f7-253">trafficRules</span><span class="sxs-lookup"><span data-stu-id="942f7-253">trafficRules</span></span>|<span data-ttu-id="942f7-254">coleção [vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-254">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="942f7-255">Regras de tráfego.</span><span class="sxs-lookup"><span data-stu-id="942f7-255">Traffic rules.</span></span> <span data-ttu-id="942f7-256">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="942f7-256">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="942f7-257">roteie</span><span class="sxs-lookup"><span data-stu-id="942f7-257">routes</span></span>|<span data-ttu-id="942f7-258">coleção [vpnRoute](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-258">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="942f7-259">Rotas (opcionais para provedores de terceiros).</span><span class="sxs-lookup"><span data-stu-id="942f7-259">Routes (optional for third-party providers).</span></span> <span data-ttu-id="942f7-260">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="942f7-260">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="942f7-261">dnsRules</span><span class="sxs-lookup"><span data-stu-id="942f7-261">dnsRules</span></span>|<span data-ttu-id="942f7-262">coleção [vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="942f7-262">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="942f7-263">Regras de DNS.</span><span class="sxs-lookup"><span data-stu-id="942f7-263">DNS rules.</span></span> <span data-ttu-id="942f7-264">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="942f7-264">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="942f7-265">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="942f7-265">trustedNetworkDomains</span></span>|<span data-ttu-id="942f7-266">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="942f7-266">String collection</span></span>|<span data-ttu-id="942f7-267">Domínios de rede confiáveis</span><span class="sxs-lookup"><span data-stu-id="942f7-267">Trusted Network Domains</span></span>|
|<span data-ttu-id="942f7-268">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="942f7-268">cryptographySuite</span></span>|[<span data-ttu-id="942f7-269">cryptographySuite</span><span class="sxs-lookup"><span data-stu-id="942f7-269">cryptographySuite</span></span>](../resources/intune-deviceconfig-cryptographysuite.md)|<span data-ttu-id="942f7-270">Configurações de segurança do pacote de criptografia para VPN IKEv2 no Windows10 e superior</span><span class="sxs-lookup"><span data-stu-id="942f7-270">Cryptography Suite security settings for IKEv2 VPN in Windows10 and above</span></span> |



## <a name="response"></a><span data-ttu-id="942f7-271">Resposta</span><span class="sxs-lookup"><span data-stu-id="942f7-271">Response</span></span>
<span data-ttu-id="942f7-272">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="942f7-272">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="942f7-273">Exemplo</span><span class="sxs-lookup"><span data-stu-id="942f7-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="942f7-274">Solicitação</span><span class="sxs-lookup"><span data-stu-id="942f7-274">Request</span></span>
<span data-ttu-id="942f7-275">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="942f7-275">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4463

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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
  ],
  "cryptographySuite": {
    "@odata.type": "microsoft.graph.cryptographySuite",
    "encryptionMethod": "des",
    "integrityCheckMethod": "sha1_96",
    "dhGroup": "group2",
    "cipherTransformConstants": "des",
    "authenticationTransformConstants": "sha1_96",
    "pfsGroup": "pfs2"
  }
}
```

### <a name="response"></a><span data-ttu-id="942f7-276">Resposta</span><span class="sxs-lookup"><span data-stu-id="942f7-276">Response</span></span>
<span data-ttu-id="942f7-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="942f7-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4635

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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
  ],
  "cryptographySuite": {
    "@odata.type": "microsoft.graph.cryptographySuite",
    "encryptionMethod": "des",
    "integrityCheckMethod": "sha1_96",
    "dhGroup": "group2",
    "cipherTransformConstants": "des",
    "authenticationTransformConstants": "sha1_96",
    "pfsGroup": "pfs2"
  }
}
```



