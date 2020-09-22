---
title: Criar windows81VpnConfiguration
description: Criar um novo objeto windows81VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 42f65ab940158536420c335d7416484d52a4365c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48047914"
---
# <a name="create-windows81vpnconfiguration"></a><span data-ttu-id="c4759-103">Criar windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c4759-103">Create windows81VpnConfiguration</span></span>

<span data-ttu-id="c4759-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4759-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4759-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4759-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4759-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4759-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4759-107">Criar um novo objeto [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c4759-107">Create a new [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4759-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4759-108">Prerequisites</span></span>
<span data-ttu-id="c4759-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4759-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4759-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4759-111">Permission type</span></span>|<span data-ttu-id="c4759-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c4759-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4759-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4759-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c4759-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4759-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c4759-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4759-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4759-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4759-116">Not supported.</span></span>|
|<span data-ttu-id="c4759-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4759-117">Application</span></span>|<span data-ttu-id="c4759-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4759-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4759-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4759-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c4759-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4759-120">Request headers</span></span>
|<span data-ttu-id="c4759-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4759-121">Header</span></span>|<span data-ttu-id="c4759-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c4759-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4759-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4759-123">Authorization</span></span>|<span data-ttu-id="c4759-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4759-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4759-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4759-125">Accept</span></span>|<span data-ttu-id="c4759-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4759-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4759-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4759-127">Request body</span></span>
<span data-ttu-id="c4759-128">No corpo da solicitação, forneça uma representação JSON do objeto windows81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c4759-128">In the request body, supply a JSON representation for the windows81VpnConfiguration object.</span></span>

<span data-ttu-id="c4759-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c4759-129">The following table shows the properties that are required when you create the windows81VpnConfiguration.</span></span>

|<span data-ttu-id="c4759-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4759-130">Property</span></span>|<span data-ttu-id="c4759-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4759-131">Type</span></span>|<span data-ttu-id="c4759-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4759-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4759-133">id</span><span class="sxs-lookup"><span data-stu-id="c4759-133">id</span></span>|<span data-ttu-id="c4759-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4759-134">String</span></span>|<span data-ttu-id="c4759-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c4759-135">Key of the entity.</span></span> <span data-ttu-id="c4759-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4759-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4759-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4759-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c4759-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4759-138">DateTimeOffset</span></span>|<span data-ttu-id="c4759-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c4759-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c4759-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4759-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4759-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c4759-141">roleScopeTagIds</span></span>|<span data-ttu-id="c4759-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4759-142">String collection</span></span>|<span data-ttu-id="c4759-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c4759-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c4759-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4759-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4759-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c4759-145">supportsScopeTags</span></span>|<span data-ttu-id="c4759-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="c4759-146">Boolean</span></span>|<span data-ttu-id="c4759-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c4759-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c4759-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c4759-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c4759-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c4759-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c4759-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c4759-150">This property is read-only.</span></span> <span data-ttu-id="c4759-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4759-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4759-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c4759-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c4759-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c4759-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c4759-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="c4759-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c4759-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4759-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4759-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c4759-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c4759-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c4759-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c4759-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="c4759-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c4759-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4759-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4759-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c4759-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c4759-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c4759-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c4759-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="c4759-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c4759-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4759-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4759-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c4759-164">createdDateTime</span></span>|<span data-ttu-id="c4759-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4759-165">DateTimeOffset</span></span>|<span data-ttu-id="c4759-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c4759-166">DateTime the object was created.</span></span> <span data-ttu-id="c4759-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4759-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4759-168">description</span><span class="sxs-lookup"><span data-stu-id="c4759-168">description</span></span>|<span data-ttu-id="c4759-169">String</span><span class="sxs-lookup"><span data-stu-id="c4759-169">String</span></span>|<span data-ttu-id="c4759-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c4759-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c4759-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4759-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4759-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c4759-172">displayName</span></span>|<span data-ttu-id="c4759-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4759-173">String</span></span>|<span data-ttu-id="c4759-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c4759-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c4759-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4759-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4759-176">versão</span><span class="sxs-lookup"><span data-stu-id="c4759-176">version</span></span>|<span data-ttu-id="c4759-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c4759-177">Int32</span></span>|<span data-ttu-id="c4759-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c4759-178">Version of the device configuration.</span></span> <span data-ttu-id="c4759-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4759-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c4759-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="c4759-180">connectionName</span></span>|<span data-ttu-id="c4759-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4759-181">String</span></span>|<span data-ttu-id="c4759-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="c4759-182">Connection name displayed to the user.</span></span> <span data-ttu-id="c4759-183">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4759-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c4759-184">servidores</span><span class="sxs-lookup"><span data-stu-id="c4759-184">servers</span></span>|<span data-ttu-id="c4759-185">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="c4759-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="c4759-186">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="c4759-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="c4759-187">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="c4759-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="c4759-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c4759-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="c4759-189">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4759-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c4759-190">customXml</span><span class="sxs-lookup"><span data-stu-id="c4759-190">customXml</span></span>|<span data-ttu-id="c4759-191">Binária</span><span class="sxs-lookup"><span data-stu-id="c4759-191">Binary</span></span>|<span data-ttu-id="c4759-192">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="c4759-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="c4759-193">(Matriz de bytes codificados por UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c4759-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="c4759-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="c4759-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="c4759-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c4759-195">Boolean</span></span>|<span data-ttu-id="c4759-196">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="c4759-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="c4759-197">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c4759-197">This property is read-only.</span></span>|
|<span data-ttu-id="c4759-198">Connection</span><span class="sxs-lookup"><span data-stu-id="c4759-198">connectionType</span></span>|[<span data-ttu-id="c4759-199">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="c4759-199">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="c4759-200">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="c4759-200">Connection type.</span></span> <span data-ttu-id="c4759-201">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="c4759-201">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="c4759-202">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="c4759-202">loginGroupOrDomain</span></span>|<span data-ttu-id="c4759-203">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4759-203">String</span></span>|<span data-ttu-id="c4759-204">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="c4759-204">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="c4759-205">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="c4759-205">enableSplitTunneling</span></span>|<span data-ttu-id="c4759-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="c4759-206">Boolean</span></span>|<span data-ttu-id="c4759-207">Habilitar o tunelamento dividido para a VPN.</span><span class="sxs-lookup"><span data-stu-id="c4759-207">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="c4759-208">proxyServer</span><span class="sxs-lookup"><span data-stu-id="c4759-208">proxyServer</span></span>|[<span data-ttu-id="c4759-209">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="c4759-209">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="c4759-210">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="c4759-210">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="c4759-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4759-211">Response</span></span>
<span data-ttu-id="c4759-212">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4759-212">If successful, this method returns a `201 Created` response code and a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4759-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4759-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4759-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4759-214">Request</span></span>
<span data-ttu-id="c4759-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4759-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="c4759-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4759-216">Response</span></span>
<span data-ttu-id="c4759-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4759-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






