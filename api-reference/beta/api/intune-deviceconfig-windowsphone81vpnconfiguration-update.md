---
title: Atualizar windowsPhone81VpnConfiguration
description: Atualiza as propriedades de um objeto windowsPhone81VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d9d83c5494b963af474d46aac810b8842f0c12bd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728806"
---
# <a name="update-windowsphone81vpnconfiguration"></a><span data-ttu-id="99b83-103">Atualizar windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="99b83-103">Update windowsPhone81VpnConfiguration</span></span>

<span data-ttu-id="99b83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99b83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99b83-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99b83-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99b83-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99b83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99b83-107">Atualiza as propriedades de um objeto [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="99b83-107">Update the properties of a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99b83-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99b83-108">Prerequisites</span></span>
<span data-ttu-id="99b83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99b83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99b83-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99b83-111">Permission type</span></span>|<span data-ttu-id="99b83-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="99b83-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99b83-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99b83-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99b83-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99b83-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="99b83-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99b83-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99b83-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99b83-116">Not supported.</span></span>|
|<span data-ttu-id="99b83-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99b83-117">Application</span></span>|<span data-ttu-id="99b83-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99b83-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99b83-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99b83-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="99b83-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99b83-120">Request headers</span></span>
|<span data-ttu-id="99b83-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99b83-121">Header</span></span>|<span data-ttu-id="99b83-122">Valor</span><span class="sxs-lookup"><span data-stu-id="99b83-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99b83-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="99b83-123">Authorization</span></span>|<span data-ttu-id="99b83-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99b83-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99b83-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="99b83-125">Accept</span></span>|<span data-ttu-id="99b83-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99b83-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99b83-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99b83-127">Request body</span></span>
<span data-ttu-id="99b83-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="99b83-128">In the request body, supply a JSON representation for the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="99b83-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99b83-129">The following table shows the properties that are required when you create the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md).</span></span>

|<span data-ttu-id="99b83-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99b83-130">Property</span></span>|<span data-ttu-id="99b83-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="99b83-131">Type</span></span>|<span data-ttu-id="99b83-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="99b83-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99b83-133">id</span><span class="sxs-lookup"><span data-stu-id="99b83-133">id</span></span>|<span data-ttu-id="99b83-134">String</span><span class="sxs-lookup"><span data-stu-id="99b83-134">String</span></span>|<span data-ttu-id="99b83-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="99b83-135">Key of the entity.</span></span> <span data-ttu-id="99b83-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99b83-137">lastModifiedDateTime</span></span>|<span data-ttu-id="99b83-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99b83-138">DateTimeOffset</span></span>|<span data-ttu-id="99b83-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="99b83-139">DateTime the object was last modified.</span></span> <span data-ttu-id="99b83-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="99b83-141">roleScopeTagIds</span></span>|<span data-ttu-id="99b83-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="99b83-142">String collection</span></span>|<span data-ttu-id="99b83-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="99b83-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="99b83-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="99b83-145">supportsScopeTags</span></span>|<span data-ttu-id="99b83-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="99b83-146">Boolean</span></span>|<span data-ttu-id="99b83-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="99b83-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="99b83-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="99b83-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="99b83-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="99b83-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="99b83-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="99b83-150">This property is read-only.</span></span> <span data-ttu-id="99b83-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="99b83-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="99b83-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="99b83-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="99b83-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="99b83-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="99b83-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="99b83-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="99b83-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="99b83-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="99b83-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="99b83-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="99b83-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="99b83-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="99b83-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="99b83-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="99b83-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="99b83-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="99b83-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99b83-164">createdDateTime</span></span>|<span data-ttu-id="99b83-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99b83-165">DateTimeOffset</span></span>|<span data-ttu-id="99b83-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="99b83-166">DateTime the object was created.</span></span> <span data-ttu-id="99b83-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-168">description</span><span class="sxs-lookup"><span data-stu-id="99b83-168">description</span></span>|<span data-ttu-id="99b83-169">String</span><span class="sxs-lookup"><span data-stu-id="99b83-169">String</span></span>|<span data-ttu-id="99b83-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="99b83-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="99b83-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-172">displayName</span><span class="sxs-lookup"><span data-stu-id="99b83-172">displayName</span></span>|<span data-ttu-id="99b83-173">String</span><span class="sxs-lookup"><span data-stu-id="99b83-173">String</span></span>|<span data-ttu-id="99b83-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="99b83-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="99b83-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-176">versão</span><span class="sxs-lookup"><span data-stu-id="99b83-176">version</span></span>|<span data-ttu-id="99b83-177">Int32</span><span class="sxs-lookup"><span data-stu-id="99b83-177">Int32</span></span>|<span data-ttu-id="99b83-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="99b83-178">Version of the device configuration.</span></span> <span data-ttu-id="99b83-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="99b83-180">connectionName</span></span>|<span data-ttu-id="99b83-181">String</span><span class="sxs-lookup"><span data-stu-id="99b83-181">String</span></span>|<span data-ttu-id="99b83-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="99b83-182">Connection name displayed to the user.</span></span> <span data-ttu-id="99b83-183">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-184">servidores</span><span class="sxs-lookup"><span data-stu-id="99b83-184">servers</span></span>|<span data-ttu-id="99b83-185">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="99b83-186">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="99b83-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="99b83-187">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="99b83-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="99b83-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="99b83-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="99b83-189">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-190">customXml</span><span class="sxs-lookup"><span data-stu-id="99b83-190">customXml</span></span>|<span data-ttu-id="99b83-191">Binária</span><span class="sxs-lookup"><span data-stu-id="99b83-191">Binary</span></span>|<span data-ttu-id="99b83-192">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="99b83-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="99b83-193">(Matriz de bytes codificados por UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="99b83-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="99b83-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="99b83-195">Boolean</span></span>|<span data-ttu-id="99b83-196">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="99b83-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="99b83-197">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="99b83-197">This property is read-only.</span></span> <span data-ttu-id="99b83-198">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-199">Connection</span><span class="sxs-lookup"><span data-stu-id="99b83-199">connectionType</span></span>|[<span data-ttu-id="99b83-200">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="99b83-200">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="99b83-201">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="99b83-201">Connection type.</span></span> <span data-ttu-id="99b83-202">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="99b83-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="99b83-203">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="99b83-203">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="99b83-204">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="99b83-204">loginGroupOrDomain</span></span>|<span data-ttu-id="99b83-205">String</span><span class="sxs-lookup"><span data-stu-id="99b83-205">String</span></span>|<span data-ttu-id="99b83-206">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="99b83-206">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="99b83-207">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-207">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-208">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="99b83-208">enableSplitTunneling</span></span>|<span data-ttu-id="99b83-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="99b83-209">Boolean</span></span>|<span data-ttu-id="99b83-210">Habilitar o tunelamento dividido para a VPN.</span><span class="sxs-lookup"><span data-stu-id="99b83-210">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="99b83-211">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-211">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-212">proxyServer</span><span class="sxs-lookup"><span data-stu-id="99b83-212">proxyServer</span></span>|[<span data-ttu-id="99b83-213">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="99b83-213">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="99b83-214">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="99b83-214">Proxy Server.</span></span> <span data-ttu-id="99b83-215">Herdado de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="99b83-215">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="99b83-216">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="99b83-216">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="99b83-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="99b83-217">Boolean</span></span>|<span data-ttu-id="99b83-218">Ignorar VPN no Wi-Fi da empresa.</span><span class="sxs-lookup"><span data-stu-id="99b83-218">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="99b83-219">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="99b83-219">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="99b83-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="99b83-220">Boolean</span></span>|<span data-ttu-id="99b83-221">Ignorar VPN no Wi-Fi domiciliar.</span><span class="sxs-lookup"><span data-stu-id="99b83-221">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="99b83-222">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="99b83-222">authenticationMethod</span></span>|[<span data-ttu-id="99b83-223">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="99b83-223">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="99b83-224">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="99b83-224">Authentication method.</span></span> <span data-ttu-id="99b83-225">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="99b83-225">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="99b83-226">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="99b83-226">rememberUserCredentials</span></span>|<span data-ttu-id="99b83-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="99b83-227">Boolean</span></span>|<span data-ttu-id="99b83-228">Lembrar as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="99b83-228">Remember user credentials.</span></span>|
|<span data-ttu-id="99b83-229">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="99b83-229">dnsSuffixSearchList</span></span>|<span data-ttu-id="99b83-230">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="99b83-230">String collection</span></span>|<span data-ttu-id="99b83-231">Lista de pesquisa de sufixo DNS.</span><span class="sxs-lookup"><span data-stu-id="99b83-231">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="99b83-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="99b83-232">Response</span></span>
<span data-ttu-id="99b83-233">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99b83-233">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99b83-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99b83-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="99b83-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99b83-235">Request</span></span>
<span data-ttu-id="99b83-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99b83-236">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="99b83-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="99b83-237">Response</span></span>
<span data-ttu-id="99b83-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99b83-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





