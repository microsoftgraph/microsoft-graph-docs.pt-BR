---
title: Atualizar windows81VpnConfiguration
description: Atualiza as propriedades de um objeto windows81VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d7051b38acdd33af09d94f492be87290cc6ad9cd
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39946949"
---
# <a name="update-windows81vpnconfiguration"></a><span data-ttu-id="9e3ba-103">Atualizar windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e3ba-103">Update windows81VpnConfiguration</span></span>

> <span data-ttu-id="9e3ba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e3ba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e3ba-106">Atualiza as propriedades de um objeto [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9e3ba-106">Update the properties of a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e3ba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e3ba-107">Prerequisites</span></span>
<span data-ttu-id="9e3ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e3ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e3ba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e3ba-110">Permission type</span></span>|<span data-ttu-id="9e3ba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e3ba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e3ba-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e3ba-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e3ba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e3ba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-115">Not supported.</span></span>|
|<span data-ttu-id="9e3ba-116">Application</span><span class="sxs-lookup"><span data-stu-id="9e3ba-116">Application</span></span>|<span data-ttu-id="9e3ba-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e3ba-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e3ba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e3ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9e3ba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e3ba-119">Request headers</span></span>
|<span data-ttu-id="9e3ba-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e3ba-120">Header</span></span>|<span data-ttu-id="9e3ba-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9e3ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e3ba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e3ba-122">Authorization</span></span>|<span data-ttu-id="9e3ba-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e3ba-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9e3ba-124">Accept</span></span>|<span data-ttu-id="9e3ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e3ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e3ba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e3ba-126">Request body</span></span>
<span data-ttu-id="9e3ba-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9e3ba-127">In the request body, supply a JSON representation for the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="9e3ba-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e3ba-128">The following table shows the properties that are required when you create the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span>

|<span data-ttu-id="9e3ba-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e3ba-129">Property</span></span>|<span data-ttu-id="9e3ba-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e3ba-130">Type</span></span>|<span data-ttu-id="9e3ba-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e3ba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e3ba-132">id</span><span class="sxs-lookup"><span data-stu-id="9e3ba-132">id</span></span>|<span data-ttu-id="9e3ba-133">String</span><span class="sxs-lookup"><span data-stu-id="9e3ba-133">String</span></span>|<span data-ttu-id="9e3ba-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-134">Key of the entity.</span></span> <span data-ttu-id="9e3ba-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e3ba-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e3ba-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9e3ba-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e3ba-137">DateTimeOffset</span></span>|<span data-ttu-id="9e3ba-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9e3ba-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e3ba-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9e3ba-140">roleScopeTagIds</span></span>|<span data-ttu-id="9e3ba-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e3ba-141">String collection</span></span>|<span data-ttu-id="9e3ba-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9e3ba-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e3ba-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9e3ba-144">supportsScopeTags</span></span>|<span data-ttu-id="9e3ba-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e3ba-145">Boolean</span></span>|<span data-ttu-id="9e3ba-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9e3ba-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9e3ba-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9e3ba-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-149">This property is read-only.</span></span> <span data-ttu-id="9e3ba-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e3ba-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9e3ba-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9e3ba-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9e3ba-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9e3ba-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9e3ba-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e3ba-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9e3ba-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9e3ba-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9e3ba-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9e3ba-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9e3ba-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e3ba-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9e3ba-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9e3ba-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9e3ba-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9e3ba-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9e3ba-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e3ba-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e3ba-163">createdDateTime</span></span>|<span data-ttu-id="9e3ba-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e3ba-164">DateTimeOffset</span></span>|<span data-ttu-id="9e3ba-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-165">DateTime the object was created.</span></span> <span data-ttu-id="9e3ba-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e3ba-167">description</span><span class="sxs-lookup"><span data-stu-id="9e3ba-167">description</span></span>|<span data-ttu-id="9e3ba-168">String</span><span class="sxs-lookup"><span data-stu-id="9e3ba-168">String</span></span>|<span data-ttu-id="9e3ba-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9e3ba-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e3ba-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9e3ba-171">displayName</span></span>|<span data-ttu-id="9e3ba-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e3ba-172">String</span></span>|<span data-ttu-id="9e3ba-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9e3ba-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e3ba-175">versão</span><span class="sxs-lookup"><span data-stu-id="9e3ba-175">version</span></span>|<span data-ttu-id="9e3ba-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9e3ba-176">Int32</span></span>|<span data-ttu-id="9e3ba-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-177">Version of the device configuration.</span></span> <span data-ttu-id="9e3ba-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e3ba-179">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="9e3ba-179">connectionName</span></span>|<span data-ttu-id="9e3ba-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="9e3ba-180">String</span></span>|<span data-ttu-id="9e3ba-181">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-181">Connection name displayed to the user.</span></span> <span data-ttu-id="9e3ba-182">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="9e3ba-183">servidores</span><span class="sxs-lookup"><span data-stu-id="9e3ba-183">servers</span></span>|<span data-ttu-id="9e3ba-184">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="9e3ba-185">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="9e3ba-186">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="9e3ba-187">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="9e3ba-188">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="9e3ba-189">customXml</span><span class="sxs-lookup"><span data-stu-id="9e3ba-189">customXml</span></span>|<span data-ttu-id="9e3ba-190">Binária</span><span class="sxs-lookup"><span data-stu-id="9e3ba-190">Binary</span></span>|<span data-ttu-id="9e3ba-191">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="9e3ba-192">(Matriz de bytes codificados por UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e3ba-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="9e3ba-193">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="9e3ba-193">applyOnlyToWindows81</span></span>|<span data-ttu-id="9e3ba-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e3ba-194">Boolean</span></span>|<span data-ttu-id="9e3ba-195">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-195">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="9e3ba-196">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-196">This property is read-only.</span></span>|
|<span data-ttu-id="9e3ba-197">Connection</span><span class="sxs-lookup"><span data-stu-id="9e3ba-197">connectionType</span></span>|[<span data-ttu-id="9e3ba-198">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="9e3ba-198">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="9e3ba-199">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-199">Connection type.</span></span> <span data-ttu-id="9e3ba-200">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-200">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="9e3ba-201">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="9e3ba-201">loginGroupOrDomain</span></span>|<span data-ttu-id="9e3ba-202">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="9e3ba-202">String</span></span>|<span data-ttu-id="9e3ba-203">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-203">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="9e3ba-204">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="9e3ba-204">enableSplitTunneling</span></span>|<span data-ttu-id="9e3ba-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e3ba-205">Boolean</span></span>|<span data-ttu-id="9e3ba-206">Habilitar o tunelamento dividido para a VPN.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-206">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="9e3ba-207">proxyServer</span><span class="sxs-lookup"><span data-stu-id="9e3ba-207">proxyServer</span></span>|[<span data-ttu-id="9e3ba-208">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="9e3ba-208">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="9e3ba-209">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-209">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="9e3ba-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e3ba-210">Response</span></span>
<span data-ttu-id="9e3ba-211">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-211">If successful, this method returns a `200 OK` response code and an updated [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e3ba-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e3ba-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e3ba-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e3ba-213">Request</span></span>
<span data-ttu-id="9e3ba-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1788

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="9e3ba-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e3ba-215">Response</span></span>
<span data-ttu-id="9e3ba-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e3ba-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1960

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "id": "6aa07da3-7da3-6aa0-a37d-a06aa37da06a",
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
  }
}
```





