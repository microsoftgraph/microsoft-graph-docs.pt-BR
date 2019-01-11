---
title: Atualizar androidForWorkVpnConfiguration
description: Atualize as propriedades de um objeto androidForWorkVpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7f6c96abc8dde322972fdebd63c539b7f2f310d3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813850"
---
# <a name="update-androidforworkvpnconfiguration"></a><span data-ttu-id="db021-103">Atualizar androidForWorkVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="db021-103">Update androidForWorkVpnConfiguration</span></span>

> <span data-ttu-id="db021-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="db021-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db021-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="db021-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="db021-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="db021-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db021-107">Atualize as propriedades de um objeto [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="db021-107">Update the properties of a [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="db021-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="db021-108">Prerequisites</span></span>
<span data-ttu-id="db021-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db021-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db021-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db021-111">Permission type</span></span>|<span data-ttu-id="db021-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="db021-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db021-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db021-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db021-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db021-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db021-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db021-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db021-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db021-116">Not supported.</span></span>|
|<span data-ttu-id="db021-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db021-117">Application</span></span>|<span data-ttu-id="db021-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db021-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db021-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db021-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="db021-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db021-120">Request headers</span></span>
|<span data-ttu-id="db021-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db021-121">Header</span></span>|<span data-ttu-id="db021-122">Valor</span><span class="sxs-lookup"><span data-stu-id="db021-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db021-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="db021-123">Authorization</span></span>|<span data-ttu-id="db021-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db021-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db021-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="db021-125">Accept</span></span>|<span data-ttu-id="db021-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db021-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db021-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db021-127">Request body</span></span>
<span data-ttu-id="db021-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="db021-128">In the request body, supply a JSON representation for the [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

<span data-ttu-id="db021-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db021-129">The following table shows the properties that are required when you create the [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md).</span></span>

|<span data-ttu-id="db021-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db021-130">Property</span></span>|<span data-ttu-id="db021-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="db021-131">Type</span></span>|<span data-ttu-id="db021-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="db021-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db021-133">id</span><span class="sxs-lookup"><span data-stu-id="db021-133">id</span></span>|<span data-ttu-id="db021-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db021-134">String</span></span>|<span data-ttu-id="db021-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="db021-135">Key of the entity.</span></span> <span data-ttu-id="db021-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db021-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db021-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db021-137">lastModifiedDateTime</span></span>|<span data-ttu-id="db021-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db021-138">DateTimeOffset</span></span>|<span data-ttu-id="db021-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="db021-139">DateTime the object was last modified.</span></span> <span data-ttu-id="db021-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db021-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db021-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="db021-141">roleScopeTagIds</span></span>|<span data-ttu-id="db021-142">String collection</span><span class="sxs-lookup"><span data-stu-id="db021-142">String collection</span></span>|<span data-ttu-id="db021-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="db021-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="db021-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db021-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db021-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="db021-145">supportsScopeTags</span></span>|<span data-ttu-id="db021-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="db021-146">Boolean</span></span>|<span data-ttu-id="db021-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="db021-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="db021-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="db021-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="db021-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="db021-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="db021-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="db021-150">This property is read-only.</span></span> <span data-ttu-id="db021-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db021-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db021-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db021-152">createdDateTime</span></span>|<span data-ttu-id="db021-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db021-153">DateTimeOffset</span></span>|<span data-ttu-id="db021-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="db021-154">DateTime the object was created.</span></span> <span data-ttu-id="db021-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db021-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db021-156">description</span><span class="sxs-lookup"><span data-stu-id="db021-156">description</span></span>|<span data-ttu-id="db021-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db021-157">String</span></span>|<span data-ttu-id="db021-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db021-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="db021-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db021-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db021-160">displayName</span><span class="sxs-lookup"><span data-stu-id="db021-160">displayName</span></span>|<span data-ttu-id="db021-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db021-161">String</span></span>|<span data-ttu-id="db021-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db021-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="db021-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db021-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db021-164">version</span><span class="sxs-lookup"><span data-stu-id="db021-164">version</span></span>|<span data-ttu-id="db021-165">Int32</span><span class="sxs-lookup"><span data-stu-id="db021-165">Int32</span></span>|<span data-ttu-id="db021-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db021-166">Version of the device configuration.</span></span> <span data-ttu-id="db021-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db021-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db021-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="db021-168">connectionName</span></span>|<span data-ttu-id="db021-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db021-169">String</span></span>|<span data-ttu-id="db021-170">Nome da Conexão exibida para o usuário.</span><span class="sxs-lookup"><span data-stu-id="db021-170">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="db021-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="db021-171">connectionType</span></span>|[<span data-ttu-id="db021-172">androidForWorkVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="db021-172">androidForWorkVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|<span data-ttu-id="db021-173">Tipo de Conexão.</span><span class="sxs-lookup"><span data-stu-id="db021-173">Connection type.</span></span> <span data-ttu-id="db021-174">Os possíveis valores são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="db021-174">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="db021-175">role</span><span class="sxs-lookup"><span data-stu-id="db021-175">role</span></span>|<span data-ttu-id="db021-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db021-176">String</span></span>|<span data-ttu-id="db021-177">Função quando o tipo de conexão está definida como pulso seguro.</span><span class="sxs-lookup"><span data-stu-id="db021-177">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="db021-178">território</span><span class="sxs-lookup"><span data-stu-id="db021-178">realm</span></span>|<span data-ttu-id="db021-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db021-179">String</span></span>|<span data-ttu-id="db021-180">Território quando o tipo de conexão está definida como pulso seguro.</span><span class="sxs-lookup"><span data-stu-id="db021-180">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="db021-181">servidores</span><span class="sxs-lookup"><span data-stu-id="db021-181">servers</span></span>|<span data-ttu-id="db021-182">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="db021-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="db021-183">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="db021-183">List of VPN Servers on the network.</span></span> <span data-ttu-id="db021-184">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="db021-184">Make sure end users can access these network locations.</span></span> <span data-ttu-id="db021-185">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="db021-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="db021-186">impressão digital</span><span class="sxs-lookup"><span data-stu-id="db021-186">fingerprint</span></span>|<span data-ttu-id="db021-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db021-187">String</span></span>|<span data-ttu-id="db021-188">Impressão digital é uma cadeia de caracteres que será usada para verificar se o servidor VPN pode ser confiável, que só é aplicável quando o tipo de conexão é verificar Point Cápsula VPN.</span><span class="sxs-lookup"><span data-stu-id="db021-188">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="db021-189">customData</span><span class="sxs-lookup"><span data-stu-id="db021-189">customData</span></span>|<span data-ttu-id="db021-190">coleção [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="db021-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="db021-191">Dados personalizados quando o tipo de conexão está definida como Citrix.</span><span class="sxs-lookup"><span data-stu-id="db021-191">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="db021-192">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="db021-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="db021-193">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="db021-193">customKeyValueData</span></span>|<span data-ttu-id="db021-194">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="db021-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="db021-195">Dados personalizados quando o tipo de conexão está definida como Citrix.</span><span class="sxs-lookup"><span data-stu-id="db021-195">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="db021-196">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="db021-196">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="db021-197">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="db021-197">authenticationMethod</span></span>|[<span data-ttu-id="db021-198">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="db021-198">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="db021-199">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="db021-199">Authentication method.</span></span> <span data-ttu-id="db021-200">Os valores possíveis são: `certificate` e `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="db021-200">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="db021-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="db021-201">Response</span></span>
<span data-ttu-id="db021-202">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db021-202">If successful, this method returns a `200 OK` response code and an updated [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db021-203">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db021-203">Example</span></span>
### <a name="request"></a><span data-ttu-id="db021-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db021-204">Request</span></span>
<span data-ttu-id="db021-205">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db021-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 980

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
  "connectionType": "pulseSecure",
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "authenticationMethod": "usernameAndPassword"
}
```

### <a name="response"></a><span data-ttu-id="db021-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="db021-206">Response</span></span>
<span data-ttu-id="db021-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db021-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1157

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
  "id": "2cf4c52c-c52c-2cf4-2cc5-f42c2cc5f42c",
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
  "connectionType": "pulseSecure",
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "authenticationMethod": "usernameAndPassword"
}
```





