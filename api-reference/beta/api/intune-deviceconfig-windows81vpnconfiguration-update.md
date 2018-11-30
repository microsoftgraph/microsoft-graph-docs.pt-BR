---
title: Atualizar windows81VpnConfiguration
description: Atualize as propriedades de um objeto windows81VpnConfiguration.
ms.openlocfilehash: 19f24a03880987e65ccdfd8ccfe6015031a6fac0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038796"
---
# <a name="update-windows81vpnconfiguration"></a><span data-ttu-id="45f32-103">Atualizar windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="45f32-103">Update windows81VpnConfiguration</span></span>

> <span data-ttu-id="45f32-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="45f32-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45f32-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="45f32-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45f32-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="45f32-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45f32-107">Atualize as propriedades de um objeto [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="45f32-107">Update the properties of a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45f32-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45f32-108">Prerequisites</span></span>
<span data-ttu-id="45f32-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45f32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45f32-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45f32-111">Permission type</span></span>|<span data-ttu-id="45f32-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45f32-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45f32-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45f32-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45f32-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45f32-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="45f32-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45f32-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45f32-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45f32-116">Not supported.</span></span>|
|<span data-ttu-id="45f32-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45f32-117">Application</span></span>|<span data-ttu-id="45f32-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45f32-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45f32-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45f32-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="45f32-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45f32-120">Request headers</span></span>
|<span data-ttu-id="45f32-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45f32-121">Header</span></span>|<span data-ttu-id="45f32-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45f32-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45f32-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45f32-123">Authorization</span></span>|<span data-ttu-id="45f32-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45f32-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45f32-125">Accept</span><span class="sxs-lookup"><span data-stu-id="45f32-125">Accept</span></span>|<span data-ttu-id="45f32-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45f32-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45f32-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45f32-127">Request body</span></span>
<span data-ttu-id="45f32-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="45f32-128">In the request body, supply a JSON representation for the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

<span data-ttu-id="45f32-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="45f32-129">The following table shows the properties that are required when you create the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span>

|<span data-ttu-id="45f32-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45f32-130">Property</span></span>|<span data-ttu-id="45f32-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="45f32-131">Type</span></span>|<span data-ttu-id="45f32-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="45f32-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45f32-133">id</span><span class="sxs-lookup"><span data-stu-id="45f32-133">id</span></span>|<span data-ttu-id="45f32-134">String</span><span class="sxs-lookup"><span data-stu-id="45f32-134">String</span></span>|<span data-ttu-id="45f32-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="45f32-135">Key of the entity.</span></span> <span data-ttu-id="45f32-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45f32-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45f32-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45f32-137">lastModifiedDateTime</span></span>|<span data-ttu-id="45f32-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45f32-138">DateTimeOffset</span></span>|<span data-ttu-id="45f32-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="45f32-139">DateTime the object was last modified.</span></span> <span data-ttu-id="45f32-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45f32-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45f32-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="45f32-141">roleScopeTagIds</span></span>|<span data-ttu-id="45f32-142">String collection</span><span class="sxs-lookup"><span data-stu-id="45f32-142">String collection</span></span>|<span data-ttu-id="45f32-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="45f32-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="45f32-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45f32-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45f32-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="45f32-145">supportsScopeTags</span></span>|<span data-ttu-id="45f32-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="45f32-146">Boolean</span></span>|<span data-ttu-id="45f32-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="45f32-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="45f32-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="45f32-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="45f32-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="45f32-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="45f32-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45f32-150">This property is read-only.</span></span> <span data-ttu-id="45f32-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45f32-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45f32-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45f32-152">createdDateTime</span></span>|<span data-ttu-id="45f32-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45f32-153">DateTimeOffset</span></span>|<span data-ttu-id="45f32-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="45f32-154">DateTime the object was created.</span></span> <span data-ttu-id="45f32-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45f32-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45f32-156">description</span><span class="sxs-lookup"><span data-stu-id="45f32-156">description</span></span>|<span data-ttu-id="45f32-157">String</span><span class="sxs-lookup"><span data-stu-id="45f32-157">String</span></span>|<span data-ttu-id="45f32-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45f32-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="45f32-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45f32-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45f32-160">displayName</span><span class="sxs-lookup"><span data-stu-id="45f32-160">displayName</span></span>|<span data-ttu-id="45f32-161">String</span><span class="sxs-lookup"><span data-stu-id="45f32-161">String</span></span>|<span data-ttu-id="45f32-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45f32-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="45f32-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45f32-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45f32-164">version</span><span class="sxs-lookup"><span data-stu-id="45f32-164">version</span></span>|<span data-ttu-id="45f32-165">Int32</span><span class="sxs-lookup"><span data-stu-id="45f32-165">Int32</span></span>|<span data-ttu-id="45f32-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45f32-166">Version of the device configuration.</span></span> <span data-ttu-id="45f32-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45f32-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45f32-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="45f32-168">connectionName</span></span>|<span data-ttu-id="45f32-169">String</span><span class="sxs-lookup"><span data-stu-id="45f32-169">String</span></span>|<span data-ttu-id="45f32-170">Nome da Conexão exibida para o usuário.</span><span class="sxs-lookup"><span data-stu-id="45f32-170">Connection name displayed to the user.</span></span> <span data-ttu-id="45f32-171">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45f32-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="45f32-172">servidores</span><span class="sxs-lookup"><span data-stu-id="45f32-172">servers</span></span>|<span data-ttu-id="45f32-173">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="45f32-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="45f32-174">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="45f32-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="45f32-175">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="45f32-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="45f32-176">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="45f32-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="45f32-177">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45f32-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="45f32-178">customXml</span><span class="sxs-lookup"><span data-stu-id="45f32-178">customXml</span></span>|<span data-ttu-id="45f32-179">Binário</span><span class="sxs-lookup"><span data-stu-id="45f32-179">Binary</span></span>|<span data-ttu-id="45f32-180">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="45f32-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="45f32-181">(Array de byte codificado UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45f32-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="45f32-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="45f32-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="45f32-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="45f32-183">Boolean</span></span>|<span data-ttu-id="45f32-184">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="45f32-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="45f32-185">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45f32-185">This property is read-only.</span></span>|
|<span data-ttu-id="45f32-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="45f32-186">connectionType</span></span>|[<span data-ttu-id="45f32-187">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="45f32-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="45f32-188">Tipo de Conexão.</span><span class="sxs-lookup"><span data-stu-id="45f32-188">Connection type.</span></span> <span data-ttu-id="45f32-189">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="45f32-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="45f32-190">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="45f32-190">loginGroupOrDomain</span></span>|<span data-ttu-id="45f32-191">String</span><span class="sxs-lookup"><span data-stu-id="45f32-191">String</span></span>|<span data-ttu-id="45f32-192">Grupo de login ou domínio quando o tipo de conexão está definida como Dell SonicWALL Mobile Conexão.</span><span class="sxs-lookup"><span data-stu-id="45f32-192">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="45f32-193">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="45f32-193">enableSplitTunneling</span></span>|<span data-ttu-id="45f32-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="45f32-194">Boolean</span></span>|<span data-ttu-id="45f32-195">Habilite o túnel em divisão da VPN.</span><span class="sxs-lookup"><span data-stu-id="45f32-195">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="45f32-196">proxyServer</span><span class="sxs-lookup"><span data-stu-id="45f32-196">proxyServer</span></span>|[<span data-ttu-id="45f32-197">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="45f32-197">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="45f32-198">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="45f32-198">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="45f32-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="45f32-199">Response</span></span>
<span data-ttu-id="45f32-200">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45f32-200">If successful, this method returns a `200 OK` response code and an updated [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45f32-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45f32-201">Example</span></span>
### <a name="request"></a><span data-ttu-id="45f32-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45f32-202">Request</span></span>
<span data-ttu-id="45f32-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45f32-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1015

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="45f32-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="45f32-204">Response</span></span>
<span data-ttu-id="45f32-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45f32-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1187

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
  "id": "6aa07da3-7da3-6aa0-a37d-a06aa37da06a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





