---
title: Atualizar androidDeviceOwnerVpnConfiguration
description: Atualiza as propriedades de um objeto androidDeviceOwnerVpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2d9366eb8ec6792fe89c5e75c7c45cb55df45ea0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444025"
---
# <a name="update-androiddeviceownervpnconfiguration"></a><span data-ttu-id="47651-103">Atualizar androidDeviceOwnerVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="47651-103">Update androidDeviceOwnerVpnConfiguration</span></span>

<span data-ttu-id="47651-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="47651-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47651-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="47651-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47651-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47651-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47651-107">Atualiza as propriedades de um objeto [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="47651-107">Update the properties of a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47651-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47651-108">Prerequisites</span></span>
<span data-ttu-id="47651-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47651-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47651-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47651-111">Permission type</span></span>|<span data-ttu-id="47651-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="47651-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47651-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47651-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47651-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47651-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47651-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47651-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47651-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47651-116">Not supported.</span></span>|
|<span data-ttu-id="47651-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47651-117">Application</span></span>|<span data-ttu-id="47651-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47651-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47651-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47651-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="47651-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47651-120">Request headers</span></span>
|<span data-ttu-id="47651-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47651-121">Header</span></span>|<span data-ttu-id="47651-122">Valor</span><span class="sxs-lookup"><span data-stu-id="47651-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47651-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="47651-123">Authorization</span></span>|<span data-ttu-id="47651-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47651-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47651-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="47651-125">Accept</span></span>|<span data-ttu-id="47651-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47651-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47651-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47651-127">Request body</span></span>
<span data-ttu-id="47651-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="47651-128">In the request body, supply a JSON representation for the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

<span data-ttu-id="47651-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47651-129">The following table shows the properties that are required when you create the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).</span></span>

|<span data-ttu-id="47651-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47651-130">Property</span></span>|<span data-ttu-id="47651-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="47651-131">Type</span></span>|<span data-ttu-id="47651-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="47651-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47651-133">id</span><span class="sxs-lookup"><span data-stu-id="47651-133">id</span></span>|<span data-ttu-id="47651-134">String</span><span class="sxs-lookup"><span data-stu-id="47651-134">String</span></span>|<span data-ttu-id="47651-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="47651-135">Key of the entity.</span></span> <span data-ttu-id="47651-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47651-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47651-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47651-137">lastModifiedDateTime</span></span>|<span data-ttu-id="47651-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47651-138">DateTimeOffset</span></span>|<span data-ttu-id="47651-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="47651-139">DateTime the object was last modified.</span></span> <span data-ttu-id="47651-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47651-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47651-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="47651-141">roleScopeTagIds</span></span>|<span data-ttu-id="47651-142">String collection</span><span class="sxs-lookup"><span data-stu-id="47651-142">String collection</span></span>|<span data-ttu-id="47651-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="47651-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="47651-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47651-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47651-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="47651-145">supportsScopeTags</span></span>|<span data-ttu-id="47651-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="47651-146">Boolean</span></span>|<span data-ttu-id="47651-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="47651-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="47651-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="47651-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="47651-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="47651-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="47651-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="47651-150">This property is read-only.</span></span> <span data-ttu-id="47651-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47651-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47651-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="47651-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="47651-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="47651-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="47651-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="47651-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="47651-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47651-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47651-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="47651-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="47651-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="47651-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="47651-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="47651-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="47651-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47651-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47651-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="47651-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="47651-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="47651-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="47651-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="47651-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="47651-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47651-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47651-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47651-164">createdDateTime</span></span>|<span data-ttu-id="47651-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47651-165">DateTimeOffset</span></span>|<span data-ttu-id="47651-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="47651-166">DateTime the object was created.</span></span> <span data-ttu-id="47651-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47651-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47651-168">description</span><span class="sxs-lookup"><span data-stu-id="47651-168">description</span></span>|<span data-ttu-id="47651-169">String</span><span class="sxs-lookup"><span data-stu-id="47651-169">String</span></span>|<span data-ttu-id="47651-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47651-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="47651-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47651-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47651-172">displayName</span><span class="sxs-lookup"><span data-stu-id="47651-172">displayName</span></span>|<span data-ttu-id="47651-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47651-173">String</span></span>|<span data-ttu-id="47651-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47651-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="47651-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47651-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47651-176">versão</span><span class="sxs-lookup"><span data-stu-id="47651-176">version</span></span>|<span data-ttu-id="47651-177">Int32</span><span class="sxs-lookup"><span data-stu-id="47651-177">Int32</span></span>|<span data-ttu-id="47651-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47651-178">Version of the device configuration.</span></span> <span data-ttu-id="47651-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47651-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47651-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="47651-180">authenticationMethod</span></span>|[<span data-ttu-id="47651-181">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="47651-181">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="47651-182">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="47651-182">Authentication method.</span></span> <span data-ttu-id="47651-183">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47651-183">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="47651-184">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="47651-184">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="47651-185">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="47651-185">connectionName</span></span>|<span data-ttu-id="47651-186">String</span><span class="sxs-lookup"><span data-stu-id="47651-186">String</span></span>|<span data-ttu-id="47651-187">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="47651-187">Connection name displayed to the user.</span></span> <span data-ttu-id="47651-188">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47651-188">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="47651-189">role</span><span class="sxs-lookup"><span data-stu-id="47651-189">role</span></span>|<span data-ttu-id="47651-190">String</span><span class="sxs-lookup"><span data-stu-id="47651-190">String</span></span>|<span data-ttu-id="47651-191">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="47651-191">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="47651-192">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47651-192">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="47651-193">esfera</span><span class="sxs-lookup"><span data-stu-id="47651-193">realm</span></span>|<span data-ttu-id="47651-194">String</span><span class="sxs-lookup"><span data-stu-id="47651-194">String</span></span>|<span data-ttu-id="47651-195">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="47651-195">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="47651-196">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47651-196">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="47651-197">servidores</span><span class="sxs-lookup"><span data-stu-id="47651-197">servers</span></span>|<span data-ttu-id="47651-198">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="47651-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="47651-199">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="47651-199">List of VPN Servers on the network.</span></span> <span data-ttu-id="47651-200">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="47651-200">Make sure end users can access these network locations.</span></span> <span data-ttu-id="47651-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="47651-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="47651-202">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47651-202">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="47651-203">Connection</span><span class="sxs-lookup"><span data-stu-id="47651-203">connectionType</span></span>|[<span data-ttu-id="47651-204">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="47651-204">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="47651-205">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="47651-205">Connection type.</span></span> <span data-ttu-id="47651-206">Os possíveis valores são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="47651-206">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|



## <a name="response"></a><span data-ttu-id="47651-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="47651-207">Response</span></span>
<span data-ttu-id="47651-208">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47651-208">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47651-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47651-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="47651-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47651-210">Request</span></span>
<span data-ttu-id="47651-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47651-211">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1417

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerVpnConfiguration",
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
  "authenticationMethod": "usernameAndPassword",
  "connectionName": "Connection Name value",
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
  "connectionType": "pulseSecure"
}
```

### <a name="response"></a><span data-ttu-id="47651-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="47651-212">Response</span></span>
<span data-ttu-id="47651-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47651-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1589

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerVpnConfiguration",
  "id": "972962e3-62e3-9729-e362-2997e3622997",
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
  "authenticationMethod": "usernameAndPassword",
  "connectionName": "Connection Name value",
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
  "connectionType": "pulseSecure"
}
```





