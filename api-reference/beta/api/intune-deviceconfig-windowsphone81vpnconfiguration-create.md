---
title: Criar windowsPhone81VpnConfiguration
description: Criar um novo objeto windowsPhone81VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b479189f6b27bb1c8cac07ab36b78d757d23d74d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48043532"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="9bed1-103">Criar windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="9bed1-103">Create windowsPhone81VpnConfiguration</span></span>

<span data-ttu-id="9bed1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bed1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bed1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9bed1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bed1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9bed1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bed1-107">Criar um novo objeto [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9bed1-107">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bed1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9bed1-108">Prerequisites</span></span>
<span data-ttu-id="9bed1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bed1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bed1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9bed1-111">Permission type</span></span>|<span data-ttu-id="9bed1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9bed1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bed1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9bed1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9bed1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bed1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9bed1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9bed1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bed1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9bed1-116">Not supported.</span></span>|
|<span data-ttu-id="9bed1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9bed1-117">Application</span></span>|<span data-ttu-id="9bed1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bed1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bed1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9bed1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9bed1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9bed1-120">Request headers</span></span>
|<span data-ttu-id="9bed1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9bed1-121">Header</span></span>|<span data-ttu-id="9bed1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9bed1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bed1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9bed1-123">Authorization</span></span>|<span data-ttu-id="9bed1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9bed1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bed1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9bed1-125">Accept</span></span>|<span data-ttu-id="9bed1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9bed1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bed1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9bed1-127">Request body</span></span>
<span data-ttu-id="9bed1-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9bed1-128">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="9bed1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9bed1-129">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="9bed1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bed1-130">Property</span></span>|<span data-ttu-id="9bed1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bed1-131">Type</span></span>|<span data-ttu-id="9bed1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bed1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bed1-133">id</span><span class="sxs-lookup"><span data-stu-id="9bed1-133">id</span></span>|<span data-ttu-id="9bed1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bed1-134">String</span></span>|<span data-ttu-id="9bed1-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9bed1-135">Key of the entity.</span></span> <span data-ttu-id="9bed1-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9bed1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9bed1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bed1-138">DateTimeOffset</span></span>|<span data-ttu-id="9bed1-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9bed1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9bed1-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9bed1-141">roleScopeTagIds</span></span>|<span data-ttu-id="9bed1-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bed1-142">String collection</span></span>|<span data-ttu-id="9bed1-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="9bed1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9bed1-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9bed1-145">supportsScopeTags</span></span>|<span data-ttu-id="9bed1-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="9bed1-146">Boolean</span></span>|<span data-ttu-id="9bed1-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9bed1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9bed1-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9bed1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9bed1-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9bed1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9bed1-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9bed1-150">This property is read-only.</span></span> <span data-ttu-id="9bed1-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9bed1-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9bed1-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9bed1-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9bed1-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="9bed1-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9bed1-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9bed1-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9bed1-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9bed1-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9bed1-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="9bed1-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9bed1-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9bed1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9bed1-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9bed1-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9bed1-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="9bed1-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9bed1-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9bed1-164">createdDateTime</span></span>|<span data-ttu-id="9bed1-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bed1-165">DateTimeOffset</span></span>|<span data-ttu-id="9bed1-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9bed1-166">DateTime the object was created.</span></span> <span data-ttu-id="9bed1-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-168">description</span><span class="sxs-lookup"><span data-stu-id="9bed1-168">description</span></span>|<span data-ttu-id="9bed1-169">String</span><span class="sxs-lookup"><span data-stu-id="9bed1-169">String</span></span>|<span data-ttu-id="9bed1-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9bed1-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9bed1-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9bed1-172">displayName</span></span>|<span data-ttu-id="9bed1-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bed1-173">String</span></span>|<span data-ttu-id="9bed1-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9bed1-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9bed1-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-176">versão</span><span class="sxs-lookup"><span data-stu-id="9bed1-176">version</span></span>|<span data-ttu-id="9bed1-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9bed1-177">Int32</span></span>|<span data-ttu-id="9bed1-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9bed1-178">Version of the device configuration.</span></span> <span data-ttu-id="9bed1-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="9bed1-180">connectionName</span></span>|<span data-ttu-id="9bed1-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bed1-181">String</span></span>|<span data-ttu-id="9bed1-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="9bed1-182">Connection name displayed to the user.</span></span> <span data-ttu-id="9bed1-183">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-184">servidores</span><span class="sxs-lookup"><span data-stu-id="9bed1-184">servers</span></span>|<span data-ttu-id="9bed1-185">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="9bed1-186">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="9bed1-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="9bed1-187">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="9bed1-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="9bed1-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="9bed1-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="9bed1-189">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-190">customXml</span><span class="sxs-lookup"><span data-stu-id="9bed1-190">customXml</span></span>|<span data-ttu-id="9bed1-191">Binária</span><span class="sxs-lookup"><span data-stu-id="9bed1-191">Binary</span></span>|<span data-ttu-id="9bed1-192">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="9bed1-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="9bed1-193">(Matriz de bytes codificados por UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="9bed1-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="9bed1-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bed1-195">Boolean</span></span>|<span data-ttu-id="9bed1-196">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="9bed1-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="9bed1-197">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9bed1-197">This property is read-only.</span></span> <span data-ttu-id="9bed1-198">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-199">Connection</span><span class="sxs-lookup"><span data-stu-id="9bed1-199">connectionType</span></span>|[<span data-ttu-id="9bed1-200">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="9bed1-200">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="9bed1-201">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="9bed1-201">Connection type.</span></span> <span data-ttu-id="9bed1-202">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9bed1-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="9bed1-203">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="9bed1-203">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="9bed1-204">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="9bed1-204">loginGroupOrDomain</span></span>|<span data-ttu-id="9bed1-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bed1-205">String</span></span>|<span data-ttu-id="9bed1-206">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="9bed1-206">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="9bed1-207">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-207">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-208">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="9bed1-208">enableSplitTunneling</span></span>|<span data-ttu-id="9bed1-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="9bed1-209">Boolean</span></span>|<span data-ttu-id="9bed1-210">Habilitar o tunelamento dividido para a VPN.</span><span class="sxs-lookup"><span data-stu-id="9bed1-210">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="9bed1-211">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-211">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-212">proxyServer</span><span class="sxs-lookup"><span data-stu-id="9bed1-212">proxyServer</span></span>|[<span data-ttu-id="9bed1-213">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="9bed1-213">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="9bed1-214">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="9bed1-214">Proxy Server.</span></span> <span data-ttu-id="9bed1-215">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9bed1-215">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="9bed1-216">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="9bed1-216">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="9bed1-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="9bed1-217">Boolean</span></span>|<span data-ttu-id="9bed1-218">Ignorar VPN no Wi-Fi da empresa.</span><span class="sxs-lookup"><span data-stu-id="9bed1-218">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="9bed1-219">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="9bed1-219">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="9bed1-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="9bed1-220">Boolean</span></span>|<span data-ttu-id="9bed1-221">Ignorar VPN no Wi-Fi domiciliar.</span><span class="sxs-lookup"><span data-stu-id="9bed1-221">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="9bed1-222">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9bed1-222">authenticationMethod</span></span>|[<span data-ttu-id="9bed1-223">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9bed1-223">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="9bed1-224">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="9bed1-224">Authentication method.</span></span> <span data-ttu-id="9bed1-225">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="9bed1-225">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="9bed1-226">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="9bed1-226">rememberUserCredentials</span></span>|<span data-ttu-id="9bed1-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="9bed1-227">Boolean</span></span>|<span data-ttu-id="9bed1-228">Lembrar as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="9bed1-228">Remember user credentials.</span></span>|
|<span data-ttu-id="9bed1-229">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="9bed1-229">dnsSuffixSearchList</span></span>|<span data-ttu-id="9bed1-230">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9bed1-230">String collection</span></span>|<span data-ttu-id="9bed1-231">Lista de pesquisa de sufixo DNS.</span><span class="sxs-lookup"><span data-stu-id="9bed1-231">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="9bed1-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bed1-232">Response</span></span>
<span data-ttu-id="9bed1-233">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9bed1-233">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bed1-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9bed1-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bed1-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bed1-235">Request</span></span>
<span data-ttu-id="9bed1-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bed1-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="9bed1-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bed1-237">Response</span></span>
<span data-ttu-id="9bed1-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9bed1-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






