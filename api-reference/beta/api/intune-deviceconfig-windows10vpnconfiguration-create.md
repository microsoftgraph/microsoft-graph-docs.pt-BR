---
title: Criar windows10VpnConfiguration
description: Criar um novo objeto windows10VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6200594d95123281f82a06244c5fc64832bb2fbb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962334"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="d92f9-103">Criar windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d92f9-103">Create windows10VpnConfiguration</span></span>

> <span data-ttu-id="d92f9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d92f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d92f9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d92f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d92f9-106">Criar um novo objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d92f9-106">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d92f9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d92f9-107">Prerequisites</span></span>
<span data-ttu-id="d92f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d92f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d92f9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d92f9-110">Permission type</span></span>|<span data-ttu-id="d92f9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d92f9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d92f9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d92f9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d92f9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d92f9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d92f9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d92f9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d92f9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d92f9-115">Not supported.</span></span>|
|<span data-ttu-id="d92f9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d92f9-116">Application</span></span>|<span data-ttu-id="d92f9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d92f9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d92f9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d92f9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d92f9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d92f9-119">Request headers</span></span>
|<span data-ttu-id="d92f9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d92f9-120">Header</span></span>|<span data-ttu-id="d92f9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d92f9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d92f9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d92f9-122">Authorization</span></span>|<span data-ttu-id="d92f9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d92f9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d92f9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d92f9-124">Accept</span></span>|<span data-ttu-id="d92f9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d92f9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d92f9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d92f9-126">Request body</span></span>
<span data-ttu-id="d92f9-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d92f9-127">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="d92f9-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d92f9-128">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="d92f9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d92f9-129">Property</span></span>|<span data-ttu-id="d92f9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d92f9-130">Type</span></span>|<span data-ttu-id="d92f9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d92f9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d92f9-132">id</span><span class="sxs-lookup"><span data-stu-id="d92f9-132">id</span></span>|<span data-ttu-id="d92f9-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d92f9-133">String</span></span>|<span data-ttu-id="d92f9-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d92f9-134">Key of the entity.</span></span> <span data-ttu-id="d92f9-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d92f9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d92f9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d92f9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d92f9-137">DateTimeOffset</span></span>|<span data-ttu-id="d92f9-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d92f9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d92f9-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d92f9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d92f9-140">roleScopeTagIds</span></span>|<span data-ttu-id="d92f9-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d92f9-141">String collection</span></span>|<span data-ttu-id="d92f9-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d92f9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d92f9-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d92f9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d92f9-144">supportsScopeTags</span></span>|<span data-ttu-id="d92f9-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="d92f9-145">Boolean</span></span>|<span data-ttu-id="d92f9-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d92f9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d92f9-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d92f9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d92f9-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d92f9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d92f9-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d92f9-149">This property is read-only.</span></span> <span data-ttu-id="d92f9-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d92f9-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d92f9-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d92f9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d92f9-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d92f9-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="d92f9-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d92f9-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d92f9-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d92f9-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d92f9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d92f9-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d92f9-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="d92f9-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d92f9-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d92f9-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d92f9-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d92f9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d92f9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d92f9-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="d92f9-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d92f9-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d92f9-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d92f9-163">createdDateTime</span></span>|<span data-ttu-id="d92f9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d92f9-164">DateTimeOffset</span></span>|<span data-ttu-id="d92f9-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d92f9-165">DateTime the object was created.</span></span> <span data-ttu-id="d92f9-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d92f9-167">descrição</span><span class="sxs-lookup"><span data-stu-id="d92f9-167">description</span></span>|<span data-ttu-id="d92f9-168">String</span><span class="sxs-lookup"><span data-stu-id="d92f9-168">String</span></span>|<span data-ttu-id="d92f9-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d92f9-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d92f9-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d92f9-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d92f9-171">displayName</span></span>|<span data-ttu-id="d92f9-172">String</span><span class="sxs-lookup"><span data-stu-id="d92f9-172">String</span></span>|<span data-ttu-id="d92f9-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d92f9-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d92f9-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d92f9-175">versão</span><span class="sxs-lookup"><span data-stu-id="d92f9-175">version</span></span>|<span data-ttu-id="d92f9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d92f9-176">Int32</span></span>|<span data-ttu-id="d92f9-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d92f9-177">Version of the device configuration.</span></span> <span data-ttu-id="d92f9-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d92f9-179">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="d92f9-179">connectionName</span></span>|<span data-ttu-id="d92f9-180">String</span><span class="sxs-lookup"><span data-stu-id="d92f9-180">String</span></span>|<span data-ttu-id="d92f9-181">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="d92f9-181">Connection name displayed to the user.</span></span> <span data-ttu-id="d92f9-182">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d92f9-183">servidores</span><span class="sxs-lookup"><span data-stu-id="d92f9-183">servers</span></span>|<span data-ttu-id="d92f9-184">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="d92f9-185">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="d92f9-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="d92f9-186">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="d92f9-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="d92f9-187">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d92f9-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d92f9-188">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d92f9-189">customXml</span><span class="sxs-lookup"><span data-stu-id="d92f9-189">customXml</span></span>|<span data-ttu-id="d92f9-190">Binária</span><span class="sxs-lookup"><span data-stu-id="d92f9-190">Binary</span></span>|<span data-ttu-id="d92f9-191">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="d92f9-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="d92f9-192">(Matriz de bytes codificados por UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d92f9-193">profileTarget</span><span class="sxs-lookup"><span data-stu-id="d92f9-193">profileTarget</span></span>|[<span data-ttu-id="d92f9-194">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="d92f9-194">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="d92f9-195">Tipo de destino do perfil.</span><span class="sxs-lookup"><span data-stu-id="d92f9-195">Profile target type.</span></span> <span data-ttu-id="d92f9-196">Os valores possíveis são: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="d92f9-196">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="d92f9-197">Connection</span><span class="sxs-lookup"><span data-stu-id="d92f9-197">connectionType</span></span>|[<span data-ttu-id="d92f9-198">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="d92f9-198">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="d92f9-199">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="d92f9-199">Connection type.</span></span> <span data-ttu-id="d92f9-200">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="d92f9-200">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="d92f9-201">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="d92f9-201">enableSplitTunneling</span></span>|<span data-ttu-id="d92f9-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="d92f9-202">Boolean</span></span>|<span data-ttu-id="d92f9-203">Habilitar o túnel de divisão.</span><span class="sxs-lookup"><span data-stu-id="d92f9-203">Enable split tunneling.</span></span>|
|<span data-ttu-id="d92f9-204">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="d92f9-204">enableAlwaysOn</span></span>|<span data-ttu-id="d92f9-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="d92f9-205">Boolean</span></span>|<span data-ttu-id="d92f9-206">Habilitar o modo Always on.</span><span class="sxs-lookup"><span data-stu-id="d92f9-206">Enable Always On mode.</span></span>|
|<span data-ttu-id="d92f9-207">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="d92f9-207">enableDeviceTunnel</span></span>|<span data-ttu-id="d92f9-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="d92f9-208">Boolean</span></span>|<span data-ttu-id="d92f9-209">Habilitar o túnel de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d92f9-209">Enable device tunnel.</span></span>|
|<span data-ttu-id="d92f9-210">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="d92f9-210">enableDnsRegistration</span></span>|<span data-ttu-id="d92f9-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="d92f9-211">Boolean</span></span>|<span data-ttu-id="d92f9-212">Habilitar o registro de endereço IP com DNS interno.</span><span class="sxs-lookup"><span data-stu-id="d92f9-212">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="d92f9-213">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="d92f9-213">dnsSuffixes</span></span>|<span data-ttu-id="d92f9-214">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d92f9-214">String collection</span></span>|<span data-ttu-id="d92f9-215">Especifique sufixos DNS para adicionar à lista de pesquisa de DNS para rotear corretamente nomes curtos.</span><span class="sxs-lookup"><span data-stu-id="d92f9-215">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="d92f9-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d92f9-216">authenticationMethod</span></span>|[<span data-ttu-id="d92f9-217">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d92f9-217">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="d92f9-218">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="d92f9-218">Authentication method.</span></span> <span data-ttu-id="d92f9-219">Os valores possíveis são: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="d92f9-219">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="d92f9-220">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="d92f9-220">rememberUserCredentials</span></span>|<span data-ttu-id="d92f9-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="d92f9-221">Boolean</span></span>|<span data-ttu-id="d92f9-222">Lembrar as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="d92f9-222">Remember user credentials.</span></span>|
|<span data-ttu-id="d92f9-223">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="d92f9-223">enableConditionalAccess</span></span>|<span data-ttu-id="d92f9-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="d92f9-224">Boolean</span></span>|<span data-ttu-id="d92f9-225">Habilitar o acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="d92f9-225">Enable conditional access.</span></span>|
|<span data-ttu-id="d92f9-226">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="d92f9-226">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="d92f9-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="d92f9-227">Boolean</span></span>|<span data-ttu-id="d92f9-228">Habilitar o logon único (SSO) com certificado alternativo.</span><span class="sxs-lookup"><span data-stu-id="d92f9-228">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="d92f9-229">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="d92f9-229">singleSignOnEku</span></span>|[<span data-ttu-id="d92f9-230">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="d92f9-230">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="d92f9-231">Uso de chave estendida (EKU) de logon único.</span><span class="sxs-lookup"><span data-stu-id="d92f9-231">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="d92f9-232">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="d92f9-232">singleSignOnIssuerHash</span></span>|<span data-ttu-id="d92f9-233">String</span><span class="sxs-lookup"><span data-stu-id="d92f9-233">String</span></span>|<span data-ttu-id="d92f9-234">Hash do emissor de logon único.</span><span class="sxs-lookup"><span data-stu-id="d92f9-234">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="d92f9-235">eapXml</span><span class="sxs-lookup"><span data-stu-id="d92f9-235">eapXml</span></span>|<span data-ttu-id="d92f9-236">Binária</span><span class="sxs-lookup"><span data-stu-id="d92f9-236">Binary</span></span>|<span data-ttu-id="d92f9-237">XML EAP (Extensible Authentication Protocol).</span><span class="sxs-lookup"><span data-stu-id="d92f9-237">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="d92f9-238">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="d92f9-238">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="d92f9-239">proxyServer</span><span class="sxs-lookup"><span data-stu-id="d92f9-239">proxyServer</span></span>|[<span data-ttu-id="d92f9-240">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="d92f9-240">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="d92f9-241">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="d92f9-241">Proxy Server.</span></span>|
|<span data-ttu-id="d92f9-242">associatedApps</span><span class="sxs-lookup"><span data-stu-id="d92f9-242">associatedApps</span></span>|<span data-ttu-id="d92f9-243">coleção [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-243">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="d92f9-244">Aplicativos associados.</span><span class="sxs-lookup"><span data-stu-id="d92f9-244">Associated Apps.</span></span> <span data-ttu-id="d92f9-245">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d92f9-245">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d92f9-246">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="d92f9-246">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="d92f9-247">Booliano</span><span class="sxs-lookup"><span data-stu-id="d92f9-247">Boolean</span></span>|<span data-ttu-id="d92f9-248">Somente os aplicativos associados podem usar Connection (VPN por aplicativo).</span><span class="sxs-lookup"><span data-stu-id="d92f9-248">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="d92f9-249">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="d92f9-249">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="d92f9-250">String</span><span class="sxs-lookup"><span data-stu-id="d92f9-250">String</span></span>|<span data-ttu-id="d92f9-251">Domínio de proteção de informações do Windows (WIP) a ser associado a essa conexão.</span><span class="sxs-lookup"><span data-stu-id="d92f9-251">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="d92f9-252">trafficRules</span><span class="sxs-lookup"><span data-stu-id="d92f9-252">trafficRules</span></span>|<span data-ttu-id="d92f9-253">coleção [vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-253">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="d92f9-254">Regras de tráfego.</span><span class="sxs-lookup"><span data-stu-id="d92f9-254">Traffic rules.</span></span> <span data-ttu-id="d92f9-255">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d92f9-255">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="d92f9-256">roteie</span><span class="sxs-lookup"><span data-stu-id="d92f9-256">routes</span></span>|<span data-ttu-id="d92f9-257">coleção [vpnRoute](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-257">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="d92f9-258">Rotas (opcionais para provedores de terceiros).</span><span class="sxs-lookup"><span data-stu-id="d92f9-258">Routes (optional for third-party providers).</span></span> <span data-ttu-id="d92f9-259">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d92f9-259">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="d92f9-260">dnsRules</span><span class="sxs-lookup"><span data-stu-id="d92f9-260">dnsRules</span></span>|<span data-ttu-id="d92f9-261">coleção [vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="d92f9-261">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="d92f9-262">Regras de DNS.</span><span class="sxs-lookup"><span data-stu-id="d92f9-262">DNS rules.</span></span> <span data-ttu-id="d92f9-263">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d92f9-263">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="d92f9-264">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="d92f9-264">trustedNetworkDomains</span></span>|<span data-ttu-id="d92f9-265">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d92f9-265">String collection</span></span>|<span data-ttu-id="d92f9-266">Domínios de rede confiáveis</span><span class="sxs-lookup"><span data-stu-id="d92f9-266">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="d92f9-267">Resposta</span><span class="sxs-lookup"><span data-stu-id="d92f9-267">Response</span></span>
<span data-ttu-id="d92f9-268">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d92f9-268">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d92f9-269">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d92f9-269">Example</span></span>

### <a name="request"></a><span data-ttu-id="d92f9-270">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d92f9-270">Request</span></span>
<span data-ttu-id="d92f9-271">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d92f9-271">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4160

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="d92f9-272">Resposta</span><span class="sxs-lookup"><span data-stu-id="d92f9-272">Response</span></span>
<span data-ttu-id="d92f9-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d92f9-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4332

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
  ]
}
```





