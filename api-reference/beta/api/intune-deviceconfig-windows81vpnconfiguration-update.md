---
title: Atualizar windows81VpnConfiguration
description: Atualiza as propriedades de um objeto windows81VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a2fbd0efd8e5434e4eb22c22d116c08887d26598
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533064"
---
# <a name="update-windows81vpnconfiguration"></a><span data-ttu-id="10b02-103">Atualizar windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="10b02-103">Update windows81VpnConfiguration</span></span>

> <span data-ttu-id="10b02-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="10b02-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10b02-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10b02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10b02-106">Atualiza as propriedades de um objeto [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="10b02-106">Update the properties of a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10b02-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="10b02-107">Prerequisites</span></span>
<span data-ttu-id="10b02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10b02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10b02-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10b02-110">Permission type</span></span>|<span data-ttu-id="10b02-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="10b02-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10b02-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10b02-112">Delegated (work or school account)</span></span>|<span data-ttu-id="10b02-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10b02-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="10b02-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10b02-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10b02-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10b02-115">Not supported.</span></span>|
|<span data-ttu-id="10b02-116">Application</span><span class="sxs-lookup"><span data-stu-id="10b02-116">Application</span></span>|<span data-ttu-id="10b02-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10b02-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10b02-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10b02-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="10b02-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10b02-119">Request headers</span></span>
|<span data-ttu-id="10b02-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="10b02-120">Header</span></span>|<span data-ttu-id="10b02-121">Valor</span><span class="sxs-lookup"><span data-stu-id="10b02-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10b02-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="10b02-122">Authorization</span></span>|<span data-ttu-id="10b02-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10b02-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10b02-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="10b02-124">Accept</span></span>|<span data-ttu-id="10b02-125">application/json</span><span class="sxs-lookup"><span data-stu-id="10b02-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10b02-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10b02-126">Request body</span></span>
<span data-ttu-id="10b02-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="10b02-127">In the request body, supply a JSON representation for the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="10b02-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="10b02-128">The following table shows the properties that are required when you create the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span>

|<span data-ttu-id="10b02-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10b02-129">Property</span></span>|<span data-ttu-id="10b02-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="10b02-130">Type</span></span>|<span data-ttu-id="10b02-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="10b02-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10b02-132">id</span><span class="sxs-lookup"><span data-stu-id="10b02-132">id</span></span>|<span data-ttu-id="10b02-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10b02-133">String</span></span>|<span data-ttu-id="10b02-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="10b02-134">Key of the entity.</span></span> <span data-ttu-id="10b02-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10b02-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10b02-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10b02-136">lastModifiedDateTime</span></span>|<span data-ttu-id="10b02-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10b02-137">DateTimeOffset</span></span>|<span data-ttu-id="10b02-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="10b02-138">DateTime the object was last modified.</span></span> <span data-ttu-id="10b02-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10b02-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10b02-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="10b02-140">roleScopeTagIds</span></span>|<span data-ttu-id="10b02-141">String collection</span><span class="sxs-lookup"><span data-stu-id="10b02-141">String collection</span></span>|<span data-ttu-id="10b02-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="10b02-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="10b02-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10b02-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10b02-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="10b02-144">supportsScopeTags</span></span>|<span data-ttu-id="10b02-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="10b02-145">Boolean</span></span>|<span data-ttu-id="10b02-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="10b02-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="10b02-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="10b02-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="10b02-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="10b02-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="10b02-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="10b02-149">This property is read-only.</span></span> <span data-ttu-id="10b02-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10b02-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10b02-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="10b02-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="10b02-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="10b02-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="10b02-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="10b02-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="10b02-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10b02-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10b02-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="10b02-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="10b02-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="10b02-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="10b02-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="10b02-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="10b02-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10b02-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10b02-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="10b02-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="10b02-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="10b02-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="10b02-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="10b02-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="10b02-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10b02-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10b02-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10b02-163">createdDateTime</span></span>|<span data-ttu-id="10b02-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10b02-164">DateTimeOffset</span></span>|<span data-ttu-id="10b02-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="10b02-165">DateTime the object was created.</span></span> <span data-ttu-id="10b02-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10b02-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10b02-167">description</span><span class="sxs-lookup"><span data-stu-id="10b02-167">description</span></span>|<span data-ttu-id="10b02-168">String</span><span class="sxs-lookup"><span data-stu-id="10b02-168">String</span></span>|<span data-ttu-id="10b02-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="10b02-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="10b02-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10b02-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10b02-171">displayName</span><span class="sxs-lookup"><span data-stu-id="10b02-171">displayName</span></span>|<span data-ttu-id="10b02-172">String</span><span class="sxs-lookup"><span data-stu-id="10b02-172">String</span></span>|<span data-ttu-id="10b02-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="10b02-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="10b02-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10b02-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10b02-175">versão</span><span class="sxs-lookup"><span data-stu-id="10b02-175">version</span></span>|<span data-ttu-id="10b02-176">Int32</span><span class="sxs-lookup"><span data-stu-id="10b02-176">Int32</span></span>|<span data-ttu-id="10b02-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="10b02-177">Version of the device configuration.</span></span> <span data-ttu-id="10b02-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10b02-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10b02-179">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="10b02-179">connectionName</span></span>|<span data-ttu-id="10b02-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10b02-180">String</span></span>|<span data-ttu-id="10b02-181">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="10b02-181">Connection name displayed to the user.</span></span> <span data-ttu-id="10b02-182">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10b02-182">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="10b02-183">servidores</span><span class="sxs-lookup"><span data-stu-id="10b02-183">servers</span></span>|<span data-ttu-id="10b02-184">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="10b02-184">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="10b02-185">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="10b02-185">List of VPN Servers on the network.</span></span> <span data-ttu-id="10b02-186">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="10b02-186">Make sure end users can access these network locations.</span></span> <span data-ttu-id="10b02-187">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="10b02-187">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="10b02-188">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10b02-188">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="10b02-189">customXml</span><span class="sxs-lookup"><span data-stu-id="10b02-189">customXml</span></span>|<span data-ttu-id="10b02-190">Binária</span><span class="sxs-lookup"><span data-stu-id="10b02-190">Binary</span></span>|<span data-ttu-id="10b02-191">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="10b02-191">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="10b02-192">(Matriz de bytes codificados por UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10b02-192">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="10b02-193">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="10b02-193">applyOnlyToWindows81</span></span>|<span data-ttu-id="10b02-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="10b02-194">Boolean</span></span>|<span data-ttu-id="10b02-195">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="10b02-195">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="10b02-196">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="10b02-196">This property is read-only.</span></span>|
|<span data-ttu-id="10b02-197">Connection</span><span class="sxs-lookup"><span data-stu-id="10b02-197">connectionType</span></span>|[<span data-ttu-id="10b02-198">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="10b02-198">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="10b02-199">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="10b02-199">Connection type.</span></span> <span data-ttu-id="10b02-200">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="10b02-200">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="10b02-201">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="10b02-201">loginGroupOrDomain</span></span>|<span data-ttu-id="10b02-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10b02-202">String</span></span>|<span data-ttu-id="10b02-203">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="10b02-203">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="10b02-204">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="10b02-204">enableSplitTunneling</span></span>|<span data-ttu-id="10b02-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="10b02-205">Boolean</span></span>|<span data-ttu-id="10b02-206">Habilitar o tunelamento dividido para a VPN.</span><span class="sxs-lookup"><span data-stu-id="10b02-206">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="10b02-207">proxyServer</span><span class="sxs-lookup"><span data-stu-id="10b02-207">proxyServer</span></span>|[<span data-ttu-id="10b02-208">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="10b02-208">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="10b02-209">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="10b02-209">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="10b02-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="10b02-210">Response</span></span>
<span data-ttu-id="10b02-211">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10b02-211">If successful, this method returns a `200 OK` response code and an updated [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10b02-212">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10b02-212">Example</span></span>

### <a name="request"></a><span data-ttu-id="10b02-213">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10b02-213">Request</span></span>
<span data-ttu-id="10b02-214">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10b02-214">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="10b02-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="10b02-215">Response</span></span>
<span data-ttu-id="10b02-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10b02-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






