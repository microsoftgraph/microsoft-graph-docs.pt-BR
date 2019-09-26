---
title: Atualizar windowsPhone81VpnConfiguration
description: Atualiza as propriedades de um objeto windowsPhone81VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d4097e9f5965782eecc6aa9c73c00df9c9dbb56e
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37181494"
---
# <a name="update-windowsphone81vpnconfiguration"></a><span data-ttu-id="91f3f-103">Atualizar windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="91f3f-103">Update windowsPhone81VpnConfiguration</span></span>

> <span data-ttu-id="91f3f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="91f3f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91f3f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91f3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91f3f-106">Atualiza as propriedades de um objeto [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="91f3f-106">Update the properties of a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91f3f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91f3f-107">Prerequisites</span></span>
<span data-ttu-id="91f3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91f3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91f3f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91f3f-110">Permission type</span></span>|<span data-ttu-id="91f3f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="91f3f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91f3f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91f3f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91f3f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91f3f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="91f3f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91f3f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91f3f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91f3f-115">Not supported.</span></span>|
|<span data-ttu-id="91f3f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91f3f-116">Application</span></span>|<span data-ttu-id="91f3f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91f3f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91f3f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91f3f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="91f3f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91f3f-119">Request headers</span></span>
|<span data-ttu-id="91f3f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91f3f-120">Header</span></span>|<span data-ttu-id="91f3f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="91f3f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91f3f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="91f3f-122">Authorization</span></span>|<span data-ttu-id="91f3f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91f3f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91f3f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="91f3f-124">Accept</span></span>|<span data-ttu-id="91f3f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="91f3f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91f3f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91f3f-126">Request body</span></span>
<span data-ttu-id="91f3f-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="91f3f-127">In the request body, supply a JSON representation for the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="91f3f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91f3f-128">The following table shows the properties that are required when you create the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>

|<span data-ttu-id="91f3f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91f3f-129">Property</span></span>|<span data-ttu-id="91f3f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="91f3f-130">Type</span></span>|<span data-ttu-id="91f3f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="91f3f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91f3f-132">id</span><span class="sxs-lookup"><span data-stu-id="91f3f-132">id</span></span>|<span data-ttu-id="91f3f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91f3f-133">String</span></span>|<span data-ttu-id="91f3f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="91f3f-134">Key of the entity.</span></span> <span data-ttu-id="91f3f-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91f3f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="91f3f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91f3f-137">DateTimeOffset</span></span>|<span data-ttu-id="91f3f-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="91f3f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="91f3f-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="91f3f-140">roleScopeTagIds</span></span>|<span data-ttu-id="91f3f-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="91f3f-141">String collection</span></span>|<span data-ttu-id="91f3f-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="91f3f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="91f3f-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="91f3f-144">supportsScopeTags</span></span>|<span data-ttu-id="91f3f-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="91f3f-145">Boolean</span></span>|<span data-ttu-id="91f3f-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="91f3f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="91f3f-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="91f3f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="91f3f-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="91f3f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="91f3f-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="91f3f-149">This property is read-only.</span></span> <span data-ttu-id="91f3f-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="91f3f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="91f3f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="91f3f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="91f3f-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="91f3f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="91f3f-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="91f3f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="91f3f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="91f3f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="91f3f-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="91f3f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="91f3f-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="91f3f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="91f3f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="91f3f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="91f3f-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="91f3f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="91f3f-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91f3f-163">createdDateTime</span></span>|<span data-ttu-id="91f3f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91f3f-164">DateTimeOffset</span></span>|<span data-ttu-id="91f3f-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="91f3f-165">DateTime the object was created.</span></span> <span data-ttu-id="91f3f-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-167">descrição</span><span class="sxs-lookup"><span data-stu-id="91f3f-167">description</span></span>|<span data-ttu-id="91f3f-168">String</span><span class="sxs-lookup"><span data-stu-id="91f3f-168">String</span></span>|<span data-ttu-id="91f3f-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="91f3f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="91f3f-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="91f3f-171">displayName</span></span>|<span data-ttu-id="91f3f-172">String</span><span class="sxs-lookup"><span data-stu-id="91f3f-172">String</span></span>|<span data-ttu-id="91f3f-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="91f3f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="91f3f-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-175">versão</span><span class="sxs-lookup"><span data-stu-id="91f3f-175">version</span></span>|<span data-ttu-id="91f3f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="91f3f-176">Int32</span></span>|<span data-ttu-id="91f3f-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="91f3f-177">Version of the device configuration.</span></span> <span data-ttu-id="91f3f-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-179">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="91f3f-179">connectionName</span></span>|<span data-ttu-id="91f3f-180">String</span><span class="sxs-lookup"><span data-stu-id="91f3f-180">String</span></span>|<span data-ttu-id="91f3f-181">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="91f3f-181">Connection name displayed to the user.</span></span> <span data-ttu-id="91f3f-182">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-183">servidores</span><span class="sxs-lookup"><span data-stu-id="91f3f-183">servers</span></span>|<span data-ttu-id="91f3f-184">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="91f3f-185">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="91f3f-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="91f3f-186">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="91f3f-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="91f3f-187">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="91f3f-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="91f3f-188">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-189">customXml</span><span class="sxs-lookup"><span data-stu-id="91f3f-189">customXml</span></span>|<span data-ttu-id="91f3f-190">Binária</span><span class="sxs-lookup"><span data-stu-id="91f3f-190">Binary</span></span>|<span data-ttu-id="91f3f-191">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="91f3f-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="91f3f-192">(Matriz de bytes codificados por UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-193">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="91f3f-193">applyOnlyToWindows81</span></span>|<span data-ttu-id="91f3f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="91f3f-194">Boolean</span></span>|<span data-ttu-id="91f3f-195">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="91f3f-195">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="91f3f-196">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="91f3f-196">This property is read-only.</span></span> <span data-ttu-id="91f3f-197">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-197">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-198">Connection</span><span class="sxs-lookup"><span data-stu-id="91f3f-198">connectionType</span></span>|[<span data-ttu-id="91f3f-199">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="91f3f-199">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="91f3f-200">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="91f3f-200">Connection type.</span></span> <span data-ttu-id="91f3f-201">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91f3f-201">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="91f3f-202">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="91f3f-202">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="91f3f-203">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="91f3f-203">loginGroupOrDomain</span></span>|<span data-ttu-id="91f3f-204">String</span><span class="sxs-lookup"><span data-stu-id="91f3f-204">String</span></span>|<span data-ttu-id="91f3f-205">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="91f3f-205">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="91f3f-206">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-206">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-207">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="91f3f-207">enableSplitTunneling</span></span>|<span data-ttu-id="91f3f-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="91f3f-208">Boolean</span></span>|<span data-ttu-id="91f3f-209">Habilitar o tunelamento dividido para a VPN.</span><span class="sxs-lookup"><span data-stu-id="91f3f-209">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="91f3f-210">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-210">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-211">proxyServer</span><span class="sxs-lookup"><span data-stu-id="91f3f-211">proxyServer</span></span>|[<span data-ttu-id="91f3f-212">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="91f3f-212">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="91f3f-213">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="91f3f-213">Proxy Server.</span></span> <span data-ttu-id="91f3f-214">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="91f3f-214">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="91f3f-215">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="91f3f-215">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="91f3f-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="91f3f-216">Boolean</span></span>|<span data-ttu-id="91f3f-217">Ignorar VPN no Wi-Fi da empresa.</span><span class="sxs-lookup"><span data-stu-id="91f3f-217">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="91f3f-218">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="91f3f-218">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="91f3f-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="91f3f-219">Boolean</span></span>|<span data-ttu-id="91f3f-220">Ignorar VPN no Wi-Fi domiciliar.</span><span class="sxs-lookup"><span data-stu-id="91f3f-220">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="91f3f-221">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="91f3f-221">authenticationMethod</span></span>|[<span data-ttu-id="91f3f-222">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="91f3f-222">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="91f3f-223">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="91f3f-223">Authentication method.</span></span> <span data-ttu-id="91f3f-224">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="91f3f-224">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="91f3f-225">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="91f3f-225">rememberUserCredentials</span></span>|<span data-ttu-id="91f3f-226">Booliano</span><span class="sxs-lookup"><span data-stu-id="91f3f-226">Boolean</span></span>|<span data-ttu-id="91f3f-227">Lembrar as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="91f3f-227">Remember user credentials.</span></span>|
|<span data-ttu-id="91f3f-228">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="91f3f-228">dnsSuffixSearchList</span></span>|<span data-ttu-id="91f3f-229">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="91f3f-229">String collection</span></span>|<span data-ttu-id="91f3f-230">Lista de pesquisa de sufixo DNS.</span><span class="sxs-lookup"><span data-stu-id="91f3f-230">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="91f3f-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="91f3f-231">Response</span></span>
<span data-ttu-id="91f3f-232">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91f3f-232">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91f3f-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91f3f-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="91f3f-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91f3f-234">Request</span></span>
<span data-ttu-id="91f3f-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91f3f-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2016

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="91f3f-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="91f3f-236">Response</span></span>
<span data-ttu-id="91f3f-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91f3f-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2188

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "id": "7cecc0db-c0db-7cec-dbc0-ec7cdbc0ec7c",
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




