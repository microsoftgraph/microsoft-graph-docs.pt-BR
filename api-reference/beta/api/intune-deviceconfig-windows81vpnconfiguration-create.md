---
title: Criar windows81VpnConfiguration
description: Crie um novo objeto de windows81VpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e036ac960cf90d11987f88a19137b443dd4e178c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975908"
---
# <a name="create-windows81vpnconfiguration"></a><span data-ttu-id="a994f-103">Criar windows81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="a994f-103">Create windows81VpnConfiguration</span></span>

> <span data-ttu-id="a994f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a994f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a994f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a994f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a994f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a994f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a994f-107">Crie um novo objeto de [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a994f-107">Create a new [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a994f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a994f-108">Prerequisites</span></span>
<span data-ttu-id="a994f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a994f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a994f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a994f-111">Permission type</span></span>|<span data-ttu-id="a994f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a994f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a994f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a994f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a994f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a994f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a994f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a994f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a994f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a994f-116">Not supported.</span></span>|
|<span data-ttu-id="a994f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a994f-117">Application</span></span>|<span data-ttu-id="a994f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a994f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a994f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a994f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a994f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a994f-120">Request headers</span></span>
|<span data-ttu-id="a994f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a994f-121">Header</span></span>|<span data-ttu-id="a994f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a994f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a994f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a994f-123">Authorization</span></span>|<span data-ttu-id="a994f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a994f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a994f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a994f-125">Accept</span></span>|<span data-ttu-id="a994f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a994f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a994f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a994f-127">Request body</span></span>
<span data-ttu-id="a994f-128">No corpo da solicitação, fornece uma representação JSON para o objeto windows81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a994f-128">In the request body, supply a JSON representation for the windows81VpnConfiguration object.</span></span>

<span data-ttu-id="a994f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windows81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a994f-129">The following table shows the properties that are required when you create the windows81VpnConfiguration.</span></span>

|<span data-ttu-id="a994f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a994f-130">Property</span></span>|<span data-ttu-id="a994f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a994f-131">Type</span></span>|<span data-ttu-id="a994f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a994f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a994f-133">id</span><span class="sxs-lookup"><span data-stu-id="a994f-133">id</span></span>|<span data-ttu-id="a994f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a994f-134">String</span></span>|<span data-ttu-id="a994f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a994f-135">Key of the entity.</span></span> <span data-ttu-id="a994f-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a994f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a994f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a994f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a994f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a994f-138">DateTimeOffset</span></span>|<span data-ttu-id="a994f-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a994f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a994f-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a994f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a994f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a994f-141">roleScopeTagIds</span></span>|<span data-ttu-id="a994f-142">String collection</span><span class="sxs-lookup"><span data-stu-id="a994f-142">String collection</span></span>|<span data-ttu-id="a994f-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="a994f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a994f-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a994f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a994f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a994f-145">supportsScopeTags</span></span>|<span data-ttu-id="a994f-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="a994f-146">Boolean</span></span>|<span data-ttu-id="a994f-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a994f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a994f-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a994f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a994f-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="a994f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a994f-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a994f-150">This property is read-only.</span></span> <span data-ttu-id="a994f-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a994f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a994f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a994f-152">createdDateTime</span></span>|<span data-ttu-id="a994f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a994f-153">DateTimeOffset</span></span>|<span data-ttu-id="a994f-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a994f-154">DateTime the object was created.</span></span> <span data-ttu-id="a994f-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a994f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a994f-156">descrição</span><span class="sxs-lookup"><span data-stu-id="a994f-156">description</span></span>|<span data-ttu-id="a994f-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a994f-157">String</span></span>|<span data-ttu-id="a994f-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a994f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a994f-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a994f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a994f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a994f-160">displayName</span></span>|<span data-ttu-id="a994f-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a994f-161">String</span></span>|<span data-ttu-id="a994f-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a994f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a994f-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a994f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a994f-164">version</span><span class="sxs-lookup"><span data-stu-id="a994f-164">version</span></span>|<span data-ttu-id="a994f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a994f-165">Int32</span></span>|<span data-ttu-id="a994f-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a994f-166">Version of the device configuration.</span></span> <span data-ttu-id="a994f-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a994f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a994f-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="a994f-168">connectionName</span></span>|<span data-ttu-id="a994f-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a994f-169">String</span></span>|<span data-ttu-id="a994f-170">Nome da Conexão exibida para o usuário.</span><span class="sxs-lookup"><span data-stu-id="a994f-170">Connection name displayed to the user.</span></span> <span data-ttu-id="a994f-171">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a994f-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a994f-172">servidores</span><span class="sxs-lookup"><span data-stu-id="a994f-172">servers</span></span>|<span data-ttu-id="a994f-173">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="a994f-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="a994f-174">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="a994f-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="a994f-175">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="a994f-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="a994f-176">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="a994f-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a994f-177">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a994f-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a994f-178">customXml</span><span class="sxs-lookup"><span data-stu-id="a994f-178">customXml</span></span>|<span data-ttu-id="a994f-179">Binária</span><span class="sxs-lookup"><span data-stu-id="a994f-179">Binary</span></span>|<span data-ttu-id="a994f-180">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="a994f-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="a994f-181">(Array de byte codificado UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a994f-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="a994f-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="a994f-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="a994f-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="a994f-183">Boolean</span></span>|<span data-ttu-id="a994f-184">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="a994f-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="a994f-185">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a994f-185">This property is read-only.</span></span>|
|<span data-ttu-id="a994f-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="a994f-186">connectionType</span></span>|[<span data-ttu-id="a994f-187">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="a994f-187">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="a994f-188">Tipo de Conexão.</span><span class="sxs-lookup"><span data-stu-id="a994f-188">Connection type.</span></span> <span data-ttu-id="a994f-189">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="a994f-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="a994f-190">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="a994f-190">loginGroupOrDomain</span></span>|<span data-ttu-id="a994f-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a994f-191">String</span></span>|<span data-ttu-id="a994f-192">Grupo de login ou domínio quando o tipo de conexão está definida como Dell SonicWALL Mobile Conexão.</span><span class="sxs-lookup"><span data-stu-id="a994f-192">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span>|
|<span data-ttu-id="a994f-193">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="a994f-193">enableSplitTunneling</span></span>|<span data-ttu-id="a994f-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="a994f-194">Boolean</span></span>|<span data-ttu-id="a994f-195">Habilite o túnel em divisão da VPN.</span><span class="sxs-lookup"><span data-stu-id="a994f-195">Enable split tunneling for the VPN.</span></span>|
|<span data-ttu-id="a994f-196">proxyServer</span><span class="sxs-lookup"><span data-stu-id="a994f-196">proxyServer</span></span>|[<span data-ttu-id="a994f-197">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="a994f-197">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="a994f-198">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="a994f-198">Proxy Server.</span></span>|



## <a name="response"></a><span data-ttu-id="a994f-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="a994f-199">Response</span></span>
<span data-ttu-id="a994f-200">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a994f-200">If successful, this method returns a `201 Created` response code and a [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a994f-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a994f-201">Example</span></span>
### <a name="request"></a><span data-ttu-id="a994f-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a994f-202">Request</span></span>
<span data-ttu-id="a994f-203">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a994f-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1079

{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="a994f-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="a994f-204">Response</span></span>
<span data-ttu-id="a994f-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a994f-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





