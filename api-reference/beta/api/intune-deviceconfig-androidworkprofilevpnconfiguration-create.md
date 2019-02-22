---
title: Criar androidWorkProfileVpnConfiguration
description: Criar um novo objeto androidWorkProfileVpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aabfed08848f0c3e68fadb557051afa48596e80f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140765"
---
# <a name="create-androidworkprofilevpnconfiguration"></a><span data-ttu-id="73bf7-103">Criar androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="73bf7-103">Create androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="73bf7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73bf7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73bf7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73bf7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73bf7-106">Criar um novo objeto [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="73bf7-106">Create a new [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73bf7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73bf7-107">Prerequisites</span></span>
<span data-ttu-id="73bf7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="73bf7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="73bf7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73bf7-110">Permission type</span></span>|<span data-ttu-id="73bf7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="73bf7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73bf7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73bf7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73bf7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73bf7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73bf7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73bf7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73bf7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73bf7-115">Not supported.</span></span>|
|<span data-ttu-id="73bf7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73bf7-116">Application</span></span>|<span data-ttu-id="73bf7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73bf7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73bf7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73bf7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="73bf7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73bf7-119">Request headers</span></span>
|<span data-ttu-id="73bf7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73bf7-120">Header</span></span>|<span data-ttu-id="73bf7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="73bf7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73bf7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="73bf7-122">Authorization</span></span>|<span data-ttu-id="73bf7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73bf7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73bf7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73bf7-124">Accept</span></span>|<span data-ttu-id="73bf7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73bf7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73bf7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73bf7-126">Request body</span></span>
<span data-ttu-id="73bf7-127">No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfileVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="73bf7-127">In the request body, supply a JSON representation for the androidWorkProfileVpnConfiguration object.</span></span>

<span data-ttu-id="73bf7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWorkProfileVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="73bf7-128">The following table shows the properties that are required when you create the androidWorkProfileVpnConfiguration.</span></span>

|<span data-ttu-id="73bf7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73bf7-129">Property</span></span>|<span data-ttu-id="73bf7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="73bf7-130">Type</span></span>|<span data-ttu-id="73bf7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="73bf7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73bf7-132">id</span><span class="sxs-lookup"><span data-stu-id="73bf7-132">id</span></span>|<span data-ttu-id="73bf7-133">String</span><span class="sxs-lookup"><span data-stu-id="73bf7-133">String</span></span>|<span data-ttu-id="73bf7-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="73bf7-134">Key of the entity.</span></span> <span data-ttu-id="73bf7-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73bf7-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73bf7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73bf7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="73bf7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73bf7-137">DateTimeOffset</span></span>|<span data-ttu-id="73bf7-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="73bf7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="73bf7-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73bf7-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73bf7-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="73bf7-140">roleScopeTagIds</span></span>|<span data-ttu-id="73bf7-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="73bf7-141">String collection</span></span>|<span data-ttu-id="73bf7-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="73bf7-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="73bf7-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73bf7-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73bf7-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="73bf7-144">supportsScopeTags</span></span>|<span data-ttu-id="73bf7-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="73bf7-145">Boolean</span></span>|<span data-ttu-id="73bf7-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="73bf7-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="73bf7-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="73bf7-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="73bf7-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="73bf7-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="73bf7-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73bf7-149">This property is read-only.</span></span> <span data-ttu-id="73bf7-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73bf7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73bf7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73bf7-151">createdDateTime</span></span>|<span data-ttu-id="73bf7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73bf7-152">DateTimeOffset</span></span>|<span data-ttu-id="73bf7-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="73bf7-153">DateTime the object was created.</span></span> <span data-ttu-id="73bf7-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73bf7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73bf7-155">description</span><span class="sxs-lookup"><span data-stu-id="73bf7-155">description</span></span>|<span data-ttu-id="73bf7-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73bf7-156">String</span></span>|<span data-ttu-id="73bf7-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73bf7-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="73bf7-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73bf7-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73bf7-159">displayName</span><span class="sxs-lookup"><span data-stu-id="73bf7-159">displayName</span></span>|<span data-ttu-id="73bf7-160">String</span><span class="sxs-lookup"><span data-stu-id="73bf7-160">String</span></span>|<span data-ttu-id="73bf7-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73bf7-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="73bf7-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73bf7-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73bf7-163">version</span><span class="sxs-lookup"><span data-stu-id="73bf7-163">version</span></span>|<span data-ttu-id="73bf7-164">Int32</span><span class="sxs-lookup"><span data-stu-id="73bf7-164">Int32</span></span>|<span data-ttu-id="73bf7-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73bf7-165">Version of the device configuration.</span></span> <span data-ttu-id="73bf7-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="73bf7-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="73bf7-167">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="73bf7-167">connectionName</span></span>|<span data-ttu-id="73bf7-168">String</span><span class="sxs-lookup"><span data-stu-id="73bf7-168">String</span></span>|<span data-ttu-id="73bf7-169">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="73bf7-169">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="73bf7-170">Connection</span><span class="sxs-lookup"><span data-stu-id="73bf7-170">connectionType</span></span>|[<span data-ttu-id="73bf7-171">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="73bf7-171">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="73bf7-172">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="73bf7-172">Connection type.</span></span> <span data-ttu-id="73bf7-173">Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="73bf7-173">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="73bf7-174">role</span><span class="sxs-lookup"><span data-stu-id="73bf7-174">role</span></span>|<span data-ttu-id="73bf7-175">String</span><span class="sxs-lookup"><span data-stu-id="73bf7-175">String</span></span>|<span data-ttu-id="73bf7-176">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="73bf7-176">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="73bf7-177">esfera</span><span class="sxs-lookup"><span data-stu-id="73bf7-177">realm</span></span>|<span data-ttu-id="73bf7-178">String</span><span class="sxs-lookup"><span data-stu-id="73bf7-178">String</span></span>|<span data-ttu-id="73bf7-179">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="73bf7-179">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="73bf7-180">servidores</span><span class="sxs-lookup"><span data-stu-id="73bf7-180">servers</span></span>|<span data-ttu-id="73bf7-181">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="73bf7-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="73bf7-182">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="73bf7-182">List of VPN Servers on the network.</span></span> <span data-ttu-id="73bf7-183">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="73bf7-183">Make sure end users can access these network locations.</span></span> <span data-ttu-id="73bf7-184">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="73bf7-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="73bf7-185">digitais</span><span class="sxs-lookup"><span data-stu-id="73bf7-185">fingerprint</span></span>|<span data-ttu-id="73bf7-186">String</span><span class="sxs-lookup"><span data-stu-id="73bf7-186">String</span></span>|<span data-ttu-id="73bf7-187">A impressão digital é uma cadeia de caracteres que será usada para verificar se o servidor VPN pode ser confiável, o que só é aplicável quando o tipo de conexão é VPN cápsula de ponto de verificação.</span><span class="sxs-lookup"><span data-stu-id="73bf7-187">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="73bf7-188">customData</span><span class="sxs-lookup"><span data-stu-id="73bf7-188">customData</span></span>|<span data-ttu-id="73bf7-189">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="73bf7-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="73bf7-190">Dados personalizados quando o tipo de conexão é definido como Citrix.</span><span class="sxs-lookup"><span data-stu-id="73bf7-190">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="73bf7-191">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="73bf7-191">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="73bf7-192">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="73bf7-192">customKeyValueData</span></span>|<span data-ttu-id="73bf7-193">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="73bf7-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="73bf7-194">Dados personalizados quando o tipo de conexão é definido como Citrix.</span><span class="sxs-lookup"><span data-stu-id="73bf7-194">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="73bf7-195">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="73bf7-195">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="73bf7-196">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="73bf7-196">authenticationMethod</span></span>|[<span data-ttu-id="73bf7-197">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="73bf7-197">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="73bf7-198">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="73bf7-198">Authentication method.</span></span> <span data-ttu-id="73bf7-199">Os valores possíveis são: `certificate` e `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="73bf7-199">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="73bf7-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="73bf7-200">Response</span></span>
<span data-ttu-id="73bf7-201">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73bf7-201">If successful, this method returns a `201 Created` response code and a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73bf7-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73bf7-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="73bf7-203">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73bf7-203">Request</span></span>
<span data-ttu-id="73bf7-204">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73bf7-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 989

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="73bf7-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="73bf7-205">Response</span></span>
<span data-ttu-id="73bf7-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73bf7-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




