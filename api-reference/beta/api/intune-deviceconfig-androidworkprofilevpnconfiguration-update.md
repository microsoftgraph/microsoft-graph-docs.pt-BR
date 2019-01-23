---
title: Atualizar androidWorkProfileVpnConfiguration
description: Atualize as propriedades de um objeto androidWorkProfileVpnConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7b37241b3b810bc93a67631d834f5e39da9d20ab
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416682"
---
# <a name="update-androidworkprofilevpnconfiguration"></a><span data-ttu-id="80d8d-103">Atualizar androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="80d8d-103">Update androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="80d8d-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="80d8d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="80d8d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="80d8d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80d8d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="80d8d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80d8d-107">Atualize as propriedades de um objeto [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="80d8d-107">Update the properties of a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80d8d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80d8d-108">Prerequisites</span></span>
<span data-ttu-id="80d8d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="80d8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="80d8d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80d8d-111">Permission type</span></span>|<span data-ttu-id="80d8d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="80d8d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80d8d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80d8d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80d8d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80d8d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80d8d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80d8d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80d8d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80d8d-116">Not supported.</span></span>|
|<span data-ttu-id="80d8d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80d8d-117">Application</span></span>|<span data-ttu-id="80d8d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80d8d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80d8d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80d8d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="80d8d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80d8d-120">Request headers</span></span>
|<span data-ttu-id="80d8d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80d8d-121">Header</span></span>|<span data-ttu-id="80d8d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="80d8d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80d8d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="80d8d-123">Authorization</span></span>|<span data-ttu-id="80d8d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80d8d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80d8d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="80d8d-125">Accept</span></span>|<span data-ttu-id="80d8d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80d8d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80d8d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80d8d-127">Request body</span></span>
<span data-ttu-id="80d8d-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="80d8d-128">In the request body, supply a JSON representation for the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

<span data-ttu-id="80d8d-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80d8d-129">The following table shows the properties that are required when you create the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>

|<span data-ttu-id="80d8d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80d8d-130">Property</span></span>|<span data-ttu-id="80d8d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="80d8d-131">Type</span></span>|<span data-ttu-id="80d8d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="80d8d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80d8d-133">id</span><span class="sxs-lookup"><span data-stu-id="80d8d-133">id</span></span>|<span data-ttu-id="80d8d-134">String</span><span class="sxs-lookup"><span data-stu-id="80d8d-134">String</span></span>|<span data-ttu-id="80d8d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="80d8d-135">Key of the entity.</span></span> <span data-ttu-id="80d8d-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80d8d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d8d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80d8d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="80d8d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80d8d-138">DateTimeOffset</span></span>|<span data-ttu-id="80d8d-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="80d8d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="80d8d-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80d8d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d8d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="80d8d-141">roleScopeTagIds</span></span>|<span data-ttu-id="80d8d-142">String collection</span><span class="sxs-lookup"><span data-stu-id="80d8d-142">String collection</span></span>|<span data-ttu-id="80d8d-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="80d8d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="80d8d-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80d8d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d8d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="80d8d-145">supportsScopeTags</span></span>|<span data-ttu-id="80d8d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="80d8d-146">Boolean</span></span>|<span data-ttu-id="80d8d-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="80d8d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="80d8d-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="80d8d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="80d8d-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="80d8d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="80d8d-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80d8d-150">This property is read-only.</span></span> <span data-ttu-id="80d8d-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80d8d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d8d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80d8d-152">createdDateTime</span></span>|<span data-ttu-id="80d8d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80d8d-153">DateTimeOffset</span></span>|<span data-ttu-id="80d8d-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="80d8d-154">DateTime the object was created.</span></span> <span data-ttu-id="80d8d-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80d8d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d8d-156">description</span><span class="sxs-lookup"><span data-stu-id="80d8d-156">description</span></span>|<span data-ttu-id="80d8d-157">String</span><span class="sxs-lookup"><span data-stu-id="80d8d-157">String</span></span>|<span data-ttu-id="80d8d-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80d8d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="80d8d-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80d8d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d8d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="80d8d-160">displayName</span></span>|<span data-ttu-id="80d8d-161">String</span><span class="sxs-lookup"><span data-stu-id="80d8d-161">String</span></span>|<span data-ttu-id="80d8d-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80d8d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="80d8d-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80d8d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d8d-164">version</span><span class="sxs-lookup"><span data-stu-id="80d8d-164">version</span></span>|<span data-ttu-id="80d8d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="80d8d-165">Int32</span></span>|<span data-ttu-id="80d8d-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80d8d-166">Version of the device configuration.</span></span> <span data-ttu-id="80d8d-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80d8d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80d8d-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="80d8d-168">connectionName</span></span>|<span data-ttu-id="80d8d-169">String</span><span class="sxs-lookup"><span data-stu-id="80d8d-169">String</span></span>|<span data-ttu-id="80d8d-170">Nome da Conexão exibida para o usuário.</span><span class="sxs-lookup"><span data-stu-id="80d8d-170">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="80d8d-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="80d8d-171">connectionType</span></span>|[<span data-ttu-id="80d8d-172">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="80d8d-172">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="80d8d-173">Tipo de Conexão.</span><span class="sxs-lookup"><span data-stu-id="80d8d-173">Connection type.</span></span> <span data-ttu-id="80d8d-174">Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="80d8d-174">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="80d8d-175">role</span><span class="sxs-lookup"><span data-stu-id="80d8d-175">role</span></span>|<span data-ttu-id="80d8d-176">String</span><span class="sxs-lookup"><span data-stu-id="80d8d-176">String</span></span>|<span data-ttu-id="80d8d-177">Função quando o tipo de conexão está definida como pulso seguro.</span><span class="sxs-lookup"><span data-stu-id="80d8d-177">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="80d8d-178">território</span><span class="sxs-lookup"><span data-stu-id="80d8d-178">realm</span></span>|<span data-ttu-id="80d8d-179">String</span><span class="sxs-lookup"><span data-stu-id="80d8d-179">String</span></span>|<span data-ttu-id="80d8d-180">Território quando o tipo de conexão está definida como pulso seguro.</span><span class="sxs-lookup"><span data-stu-id="80d8d-180">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="80d8d-181">servidores</span><span class="sxs-lookup"><span data-stu-id="80d8d-181">servers</span></span>|<span data-ttu-id="80d8d-182">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="80d8d-182">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="80d8d-183">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="80d8d-183">List of VPN Servers on the network.</span></span> <span data-ttu-id="80d8d-184">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="80d8d-184">Make sure end users can access these network locations.</span></span> <span data-ttu-id="80d8d-185">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="80d8d-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="80d8d-186">impressão digital</span><span class="sxs-lookup"><span data-stu-id="80d8d-186">fingerprint</span></span>|<span data-ttu-id="80d8d-187">String</span><span class="sxs-lookup"><span data-stu-id="80d8d-187">String</span></span>|<span data-ttu-id="80d8d-188">Impressão digital é uma cadeia de caracteres que será usada para verificar se o servidor VPN pode ser confiável, que só é aplicável quando o tipo de conexão é verificar Point Cápsula VPN.</span><span class="sxs-lookup"><span data-stu-id="80d8d-188">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="80d8d-189">customData</span><span class="sxs-lookup"><span data-stu-id="80d8d-189">customData</span></span>|<span data-ttu-id="80d8d-190">coleção [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="80d8d-190">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="80d8d-191">Dados personalizados quando o tipo de conexão está definida como Citrix.</span><span class="sxs-lookup"><span data-stu-id="80d8d-191">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="80d8d-192">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="80d8d-192">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="80d8d-193">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="80d8d-193">customKeyValueData</span></span>|<span data-ttu-id="80d8d-194">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="80d8d-194">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="80d8d-195">Dados personalizados quando o tipo de conexão está definida como Citrix.</span><span class="sxs-lookup"><span data-stu-id="80d8d-195">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="80d8d-196">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="80d8d-196">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="80d8d-197">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="80d8d-197">authenticationMethod</span></span>|[<span data-ttu-id="80d8d-198">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="80d8d-198">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="80d8d-199">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="80d8d-199">Authentication method.</span></span> <span data-ttu-id="80d8d-200">Os valores possíveis são: `certificate` e `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="80d8d-200">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="80d8d-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="80d8d-201">Response</span></span>
<span data-ttu-id="80d8d-202">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80d8d-202">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80d8d-203">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80d8d-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="80d8d-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80d8d-204">Request</span></span>
<span data-ttu-id="80d8d-205">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80d8d-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="80d8d-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="80d8d-206">Response</span></span>
<span data-ttu-id="80d8d-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80d8d-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




