---
title: Atualizar windowsPhone81VpnConfiguration
description: Atualiza as propriedades de um objeto windowsPhone81VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f02fd9ff1e7821cdff099971ffa04127717537b6
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122760"
---
# <a name="update-windowsphone81vpnconfiguration"></a><span data-ttu-id="c4ad0-103">Atualizar windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c4ad0-103">Update windowsPhone81VpnConfiguration</span></span>

<span data-ttu-id="c4ad0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4ad0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4ad0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4ad0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4ad0-107">Atualiza as propriedades de um objeto [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c4ad0-107">Update the properties of a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4ad0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4ad0-108">Prerequisites</span></span>
<span data-ttu-id="c4ad0-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c4ad0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4ad0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4ad0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4ad0-111">Permission type</span></span>|<span data-ttu-id="c4ad0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4ad0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4ad0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4ad0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4ad0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4ad0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-116">Not supported.</span></span>|
|<span data-ttu-id="c4ad0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4ad0-117">Application</span></span>|<span data-ttu-id="c4ad0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4ad0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4ad0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4ad0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c4ad0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ad0-120">Request headers</span></span>
|<span data-ttu-id="c4ad0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4ad0-121">Header</span></span>|<span data-ttu-id="c4ad0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c4ad0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4ad0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4ad0-123">Authorization</span></span>|<span data-ttu-id="c4ad0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4ad0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4ad0-125">Accept</span></span>|<span data-ttu-id="c4ad0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4ad0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4ad0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ad0-127">Request body</span></span>
<span data-ttu-id="c4ad0-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c4ad0-128">In the request body, supply a JSON representation for the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="c4ad0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4ad0-129">The following table shows the properties that are required when you create the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>

|<span data-ttu-id="c4ad0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4ad0-130">Property</span></span>|<span data-ttu-id="c4ad0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4ad0-131">Type</span></span>|<span data-ttu-id="c4ad0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4ad0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4ad0-133">id</span><span class="sxs-lookup"><span data-stu-id="c4ad0-133">id</span></span>|<span data-ttu-id="c4ad0-134">String</span><span class="sxs-lookup"><span data-stu-id="c4ad0-134">String</span></span>|<span data-ttu-id="c4ad0-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-135">Key of the entity.</span></span> <span data-ttu-id="c4ad0-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4ad0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c4ad0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4ad0-138">DateTimeOffset</span></span>|<span data-ttu-id="c4ad0-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c4ad0-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c4ad0-141">roleScopeTagIds</span></span>|<span data-ttu-id="c4ad0-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4ad0-142">String collection</span></span>|<span data-ttu-id="c4ad0-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c4ad0-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c4ad0-145">supportsScopeTags</span></span>|<span data-ttu-id="c4ad0-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="c4ad0-146">Boolean</span></span>|<span data-ttu-id="c4ad0-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c4ad0-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c4ad0-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c4ad0-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-150">This property is read-only.</span></span> <span data-ttu-id="c4ad0-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c4ad0-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c4ad0-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c4ad0-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c4ad0-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c4ad0-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c4ad0-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c4ad0-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c4ad0-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c4ad0-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c4ad0-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c4ad0-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c4ad0-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c4ad0-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c4ad0-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c4ad0-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4ad0-164">createdDateTime</span></span>|<span data-ttu-id="c4ad0-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4ad0-165">DateTimeOffset</span></span>|<span data-ttu-id="c4ad0-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-166">DateTime the object was created.</span></span> <span data-ttu-id="c4ad0-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-168">descrição</span><span class="sxs-lookup"><span data-stu-id="c4ad0-168">description</span></span>|<span data-ttu-id="c4ad0-169">String</span><span class="sxs-lookup"><span data-stu-id="c4ad0-169">String</span></span>|<span data-ttu-id="c4ad0-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c4ad0-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c4ad0-172">displayName</span></span>|<span data-ttu-id="c4ad0-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4ad0-173">String</span></span>|<span data-ttu-id="c4ad0-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c4ad0-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-176">versão</span><span class="sxs-lookup"><span data-stu-id="c4ad0-176">version</span></span>|<span data-ttu-id="c4ad0-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c4ad0-177">Int32</span></span>|<span data-ttu-id="c4ad0-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-178">Version of the device configuration.</span></span> <span data-ttu-id="c4ad0-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="c4ad0-180">connectionName</span></span>|<span data-ttu-id="c4ad0-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4ad0-181">String</span></span>|<span data-ttu-id="c4ad0-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-182">Connection name displayed to the user.</span></span> <span data-ttu-id="c4ad0-183">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-184">servidores</span><span class="sxs-lookup"><span data-stu-id="c4ad0-184">servers</span></span>|<span data-ttu-id="c4ad0-185">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="c4ad0-186">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="c4ad0-187">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="c4ad0-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c4ad0-189">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-190">customXml</span><span class="sxs-lookup"><span data-stu-id="c4ad0-190">customXml</span></span>|<span data-ttu-id="c4ad0-191">Binária</span><span class="sxs-lookup"><span data-stu-id="c4ad0-191">Binary</span></span>|<span data-ttu-id="c4ad0-192">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="c4ad0-193">(Matriz de bytes codificados por UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="c4ad0-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="c4ad0-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4ad0-195">Boolean</span></span>|<span data-ttu-id="c4ad0-196">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="c4ad0-197">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-197">This property is read-only.</span></span> <span data-ttu-id="c4ad0-198">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-199">Connection</span><span class="sxs-lookup"><span data-stu-id="c4ad0-199">connectionType</span></span>|[<span data-ttu-id="c4ad0-200">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="c4ad0-200">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="c4ad0-201">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-201">Connection type.</span></span> <span data-ttu-id="c4ad0-202">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c4ad0-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="c4ad0-203">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-203">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="c4ad0-204">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="c4ad0-204">loginGroupOrDomain</span></span>|<span data-ttu-id="c4ad0-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4ad0-205">String</span></span>|<span data-ttu-id="c4ad0-206">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-206">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="c4ad0-207">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-207">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-208">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="c4ad0-208">enableSplitTunneling</span></span>|<span data-ttu-id="c4ad0-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="c4ad0-209">Boolean</span></span>|<span data-ttu-id="c4ad0-210">Habilitar o tunelamento dividido para a VPN.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-210">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="c4ad0-211">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-211">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-212">proxyServer</span><span class="sxs-lookup"><span data-stu-id="c4ad0-212">proxyServer</span></span>|[<span data-ttu-id="c4ad0-213">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="c4ad0-213">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="c4ad0-214">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-214">Proxy Server.</span></span> <span data-ttu-id="c4ad0-215">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4ad0-215">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="c4ad0-216">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="c4ad0-216">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="c4ad0-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="c4ad0-217">Boolean</span></span>|<span data-ttu-id="c4ad0-218">Ignorar VPN no Wi-Fi da empresa.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-218">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="c4ad0-219">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="c4ad0-219">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="c4ad0-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="c4ad0-220">Boolean</span></span>|<span data-ttu-id="c4ad0-221">Ignorar VPN no Wi-Fi domiciliar.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-221">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="c4ad0-222">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c4ad0-222">authenticationMethod</span></span>|[<span data-ttu-id="c4ad0-223">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c4ad0-223">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="c4ad0-224">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-224">Authentication method.</span></span> <span data-ttu-id="c4ad0-225">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-225">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="c4ad0-226">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="c4ad0-226">rememberUserCredentials</span></span>|<span data-ttu-id="c4ad0-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="c4ad0-227">Boolean</span></span>|<span data-ttu-id="c4ad0-228">Lembrar as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-228">Remember user credentials.</span></span>|
|<span data-ttu-id="c4ad0-229">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="c4ad0-229">dnsSuffixSearchList</span></span>|<span data-ttu-id="c4ad0-230">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4ad0-230">String collection</span></span>|<span data-ttu-id="c4ad0-231">Lista de pesquisa de sufixo DNS.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-231">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="c4ad0-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4ad0-232">Response</span></span>
<span data-ttu-id="c4ad0-233">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-233">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4ad0-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4ad0-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4ad0-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ad0-235">Request</span></span>
<span data-ttu-id="c4ad0-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-236">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c4ad0-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4ad0-237">Response</span></span>
<span data-ttu-id="c4ad0-238">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-238">Here is an example of the response.</span></span> <span data-ttu-id="c4ad0-239">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-239">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c4ad0-240">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c4ad0-240">All of the properties will be returned from an actual call.</span></span>
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



