---
title: Atualizar androidWorkProfileVpnConfiguration
description: Atualize as propriedades de um objeto androidWorkProfileVpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6c1ff2e73ce14568d1ce7c725db1ffc3ae206d64
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868891"
---
# <a name="update-androidworkprofilevpnconfiguration"></a><span data-ttu-id="543bf-103">Atualizar androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="543bf-103">Update androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="543bf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="543bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="543bf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="543bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="543bf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="543bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="543bf-107">Atualize as propriedades de um objeto [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="543bf-107">Update the properties of a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="543bf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="543bf-108">Prerequisites</span></span>
<span data-ttu-id="543bf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="543bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="543bf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="543bf-111">Permission type</span></span>|<span data-ttu-id="543bf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="543bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="543bf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="543bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="543bf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="543bf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="543bf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="543bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="543bf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="543bf-116">Not supported.</span></span>|
|<span data-ttu-id="543bf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="543bf-117">Application</span></span>|<span data-ttu-id="543bf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="543bf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="543bf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="543bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="543bf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="543bf-120">Request headers</span></span>
|<span data-ttu-id="543bf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="543bf-121">Header</span></span>|<span data-ttu-id="543bf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="543bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="543bf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="543bf-123">Authorization</span></span>|<span data-ttu-id="543bf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="543bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="543bf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="543bf-125">Accept</span></span>|<span data-ttu-id="543bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="543bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="543bf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="543bf-127">Request body</span></span>
<span data-ttu-id="543bf-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="543bf-128">In the request body, supply a JSON representation for the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

<span data-ttu-id="543bf-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="543bf-129">The following table shows the properties that are required when you create the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>

|<span data-ttu-id="543bf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="543bf-130">Property</span></span>|<span data-ttu-id="543bf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="543bf-131">Type</span></span>|<span data-ttu-id="543bf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="543bf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="543bf-133">id</span><span class="sxs-lookup"><span data-stu-id="543bf-133">id</span></span>|<span data-ttu-id="543bf-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="543bf-134">String</span></span>|<span data-ttu-id="543bf-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="543bf-135">Key of the entity.</span></span> <span data-ttu-id="543bf-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="543bf-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="543bf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="543bf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="543bf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="543bf-138">DateTimeOffset</span></span>|<span data-ttu-id="543bf-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="543bf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="543bf-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="543bf-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="543bf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="543bf-141">roleScopeTagIds</span></span>|<span data-ttu-id="543bf-142">String collection</span><span class="sxs-lookup"><span data-stu-id="543bf-142">String collection</span></span>|<span data-ttu-id="543bf-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="543bf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="543bf-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="543bf-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="543bf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="543bf-145">supportsScopeTags</span></span>|<span data-ttu-id="543bf-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="543bf-146">Boolean</span></span>|<span data-ttu-id="543bf-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="543bf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="543bf-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="543bf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="543bf-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="543bf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="543bf-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="543bf-150">This property is read-only.</span></span> <span data-ttu-id="543bf-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="543bf-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="543bf-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="543bf-152">createdDateTime</span></span>|<span data-ttu-id="543bf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="543bf-153">DateTimeOffset</span></span>|<span data-ttu-id="543bf-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="543bf-154">DateTime the object was created.</span></span> <span data-ttu-id="543bf-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="543bf-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="543bf-156">description</span><span class="sxs-lookup"><span data-stu-id="543bf-156">description</span></span>|<span data-ttu-id="543bf-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="543bf-157">String</span></span>|<span data-ttu-id="543bf-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="543bf-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="543bf-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="543bf-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="543bf-160">displayName</span><span class="sxs-lookup"><span data-stu-id="543bf-160">displayName</span></span>|<span data-ttu-id="543bf-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="543bf-161">String</span></span>|<span data-ttu-id="543bf-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="543bf-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="543bf-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="543bf-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="543bf-164">version</span><span class="sxs-lookup"><span data-stu-id="543bf-164">version</span></span>|<span data-ttu-id="543bf-165">Int32</span><span class="sxs-lookup"><span data-stu-id="543bf-165">Int32</span></span>|<span data-ttu-id="543bf-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="543bf-166">Version of the device configuration.</span></span> <span data-ttu-id="543bf-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="543bf-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="543bf-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="543bf-168">connectionName</span></span>|<span data-ttu-id="543bf-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="543bf-169">String</span></span>|<span data-ttu-id="543bf-170">Nome da Conexão exibida para o usuário.</span><span class="sxs-lookup"><span data-stu-id="543bf-170">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="543bf-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="543bf-171">connectionType</span></span>|[<span data-ttu-id="543bf-172">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="543bf-172">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="543bf-173">Tipo de Conexão.</span><span class="sxs-lookup"><span data-stu-id="543bf-173">Connection type.</span></span> <span data-ttu-id="543bf-174">Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="543bf-174">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="543bf-175">role</span><span class="sxs-lookup"><span data-stu-id="543bf-175">role</span></span>|<span data-ttu-id="543bf-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="543bf-176">String</span></span>|<span data-ttu-id="543bf-177">Função quando o tipo de conexão está definida como pulso seguro.</span><span class="sxs-lookup"><span data-stu-id="543bf-177">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="543bf-178">território</span><span class="sxs-lookup"><span data-stu-id="543bf-178">realm</span></span>|<span data-ttu-id="543bf-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="543bf-179">String</span></span>|<span data-ttu-id="543bf-180">Território quando o tipo de conexão está definida como pulso seguro.</span><span class="sxs-lookup"><span data-stu-id="543bf-180">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="543bf-181">servidores</span><span class="sxs-lookup"><span data-stu-id="543bf-181">servers</span></span>|<span data-ttu-id="543bf-182">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="543bf-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="543bf-183">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="543bf-183">List of VPN Servers on the network.</span></span> <span data-ttu-id="543bf-184">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="543bf-184">Make sure end users can access these network locations.</span></span> <span data-ttu-id="543bf-185">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="543bf-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="543bf-186">impressão digital</span><span class="sxs-lookup"><span data-stu-id="543bf-186">fingerprint</span></span>|<span data-ttu-id="543bf-187">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="543bf-187">String</span></span>|<span data-ttu-id="543bf-188">Impressão digital é uma cadeia de caracteres que será usada para verificar se o servidor VPN pode ser confiável, que só é aplicável quando o tipo de conexão é verificar Point Cápsula VPN.</span><span class="sxs-lookup"><span data-stu-id="543bf-188">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="543bf-189">customData</span><span class="sxs-lookup"><span data-stu-id="543bf-189">customData</span></span>|<span data-ttu-id="543bf-190">coleção [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="543bf-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="543bf-191">Dados personalizados quando o tipo de conexão está definida como Citrix.</span><span class="sxs-lookup"><span data-stu-id="543bf-191">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="543bf-192">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="543bf-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="543bf-193">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="543bf-193">customKeyValueData</span></span>|<span data-ttu-id="543bf-194">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="543bf-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="543bf-195">Dados personalizados quando o tipo de conexão está definida como Citrix.</span><span class="sxs-lookup"><span data-stu-id="543bf-195">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="543bf-196">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="543bf-196">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="543bf-197">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="543bf-197">authenticationMethod</span></span>|[<span data-ttu-id="543bf-198">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="543bf-198">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="543bf-199">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="543bf-199">Authentication method.</span></span> <span data-ttu-id="543bf-200">Os valores possíveis são: `certificate` e `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="543bf-200">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="543bf-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="543bf-201">Response</span></span>
<span data-ttu-id="543bf-202">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="543bf-202">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="543bf-203">Exemplo</span><span class="sxs-lookup"><span data-stu-id="543bf-203">Example</span></span>
### <a name="request"></a><span data-ttu-id="543bf-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="543bf-204">Request</span></span>
<span data-ttu-id="543bf-205">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="543bf-205">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="543bf-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="543bf-206">Response</span></span>
<span data-ttu-id="543bf-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="543bf-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1161

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
  "id": "32910378-0378-3291-7803-913278039132",
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





