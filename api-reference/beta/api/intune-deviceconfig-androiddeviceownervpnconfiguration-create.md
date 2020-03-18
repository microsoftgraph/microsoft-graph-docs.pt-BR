---
title: Criar androidDeviceOwnerVpnConfiguration
description: Criar um novo objeto androidDeviceOwnerVpnConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 724b9f20f75ed1a84e7dc024a103517171692b9d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759679"
---
# <a name="create-androiddeviceownervpnconfiguration"></a><span data-ttu-id="48e51-103">Criar androidDeviceOwnerVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="48e51-103">Create androidDeviceOwnerVpnConfiguration</span></span>

> <span data-ttu-id="48e51-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="48e51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48e51-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="48e51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48e51-106">Criar um novo objeto [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="48e51-106">Create a new [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48e51-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="48e51-107">Prerequisites</span></span>
<span data-ttu-id="48e51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48e51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48e51-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48e51-110">Permission type</span></span>|<span data-ttu-id="48e51-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="48e51-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48e51-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48e51-112">Delegated (work or school account)</span></span>|<span data-ttu-id="48e51-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48e51-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="48e51-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48e51-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48e51-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48e51-115">Not supported.</span></span>|
|<span data-ttu-id="48e51-116">Application</span><span class="sxs-lookup"><span data-stu-id="48e51-116">Application</span></span>|<span data-ttu-id="48e51-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48e51-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="48e51-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48e51-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="48e51-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48e51-119">Request headers</span></span>
|<span data-ttu-id="48e51-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="48e51-120">Header</span></span>|<span data-ttu-id="48e51-121">Valor</span><span class="sxs-lookup"><span data-stu-id="48e51-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48e51-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="48e51-122">Authorization</span></span>|<span data-ttu-id="48e51-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48e51-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48e51-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="48e51-124">Accept</span></span>|<span data-ttu-id="48e51-125">application/json</span><span class="sxs-lookup"><span data-stu-id="48e51-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48e51-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48e51-126">Request body</span></span>
<span data-ttu-id="48e51-127">No corpo da solicitação, forneça uma representação JSON do objeto androidDeviceOwnerVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="48e51-127">In the request body, supply a JSON representation for the androidDeviceOwnerVpnConfiguration object.</span></span>

<span data-ttu-id="48e51-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="48e51-128">The following table shows the properties that are required when you create the androidDeviceOwnerVpnConfiguration.</span></span>

|<span data-ttu-id="48e51-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48e51-129">Property</span></span>|<span data-ttu-id="48e51-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="48e51-130">Type</span></span>|<span data-ttu-id="48e51-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="48e51-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48e51-132">id</span><span class="sxs-lookup"><span data-stu-id="48e51-132">id</span></span>|<span data-ttu-id="48e51-133">String</span><span class="sxs-lookup"><span data-stu-id="48e51-133">String</span></span>|<span data-ttu-id="48e51-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="48e51-134">Key of the entity.</span></span> <span data-ttu-id="48e51-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48e51-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48e51-136">lastModifiedDateTime</span></span>|<span data-ttu-id="48e51-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48e51-137">DateTimeOffset</span></span>|<span data-ttu-id="48e51-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="48e51-138">DateTime the object was last modified.</span></span> <span data-ttu-id="48e51-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48e51-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="48e51-140">roleScopeTagIds</span></span>|<span data-ttu-id="48e51-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="48e51-141">String collection</span></span>|<span data-ttu-id="48e51-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="48e51-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="48e51-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48e51-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="48e51-144">supportsScopeTags</span></span>|<span data-ttu-id="48e51-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="48e51-145">Boolean</span></span>|<span data-ttu-id="48e51-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="48e51-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="48e51-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="48e51-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="48e51-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="48e51-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="48e51-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="48e51-149">This property is read-only.</span></span> <span data-ttu-id="48e51-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48e51-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="48e51-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="48e51-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="48e51-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="48e51-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="48e51-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="48e51-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48e51-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="48e51-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="48e51-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="48e51-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="48e51-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="48e51-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="48e51-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48e51-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="48e51-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="48e51-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="48e51-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="48e51-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="48e51-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="48e51-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48e51-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48e51-163">createdDateTime</span></span>|<span data-ttu-id="48e51-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48e51-164">DateTimeOffset</span></span>|<span data-ttu-id="48e51-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="48e51-165">DateTime the object was created.</span></span> <span data-ttu-id="48e51-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48e51-167">description</span><span class="sxs-lookup"><span data-stu-id="48e51-167">description</span></span>|<span data-ttu-id="48e51-168">String</span><span class="sxs-lookup"><span data-stu-id="48e51-168">String</span></span>|<span data-ttu-id="48e51-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="48e51-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="48e51-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48e51-171">displayName</span><span class="sxs-lookup"><span data-stu-id="48e51-171">displayName</span></span>|<span data-ttu-id="48e51-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="48e51-172">String</span></span>|<span data-ttu-id="48e51-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="48e51-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="48e51-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48e51-175">versão</span><span class="sxs-lookup"><span data-stu-id="48e51-175">version</span></span>|<span data-ttu-id="48e51-176">Int32</span><span class="sxs-lookup"><span data-stu-id="48e51-176">Int32</span></span>|<span data-ttu-id="48e51-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="48e51-177">Version of the device configuration.</span></span> <span data-ttu-id="48e51-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="48e51-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="48e51-179">authenticationMethod</span></span>|[<span data-ttu-id="48e51-180">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="48e51-180">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="48e51-181">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="48e51-181">Authentication method.</span></span> <span data-ttu-id="48e51-182">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="48e51-182">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="48e51-183">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="48e51-183">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="48e51-184">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="48e51-184">connectionName</span></span>|<span data-ttu-id="48e51-185">String</span><span class="sxs-lookup"><span data-stu-id="48e51-185">String</span></span>|<span data-ttu-id="48e51-186">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="48e51-186">Connection name displayed to the user.</span></span> <span data-ttu-id="48e51-187">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-187">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="48e51-188">role</span><span class="sxs-lookup"><span data-stu-id="48e51-188">role</span></span>|<span data-ttu-id="48e51-189">String</span><span class="sxs-lookup"><span data-stu-id="48e51-189">String</span></span>|<span data-ttu-id="48e51-190">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="48e51-190">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="48e51-191">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-191">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="48e51-192">esfera</span><span class="sxs-lookup"><span data-stu-id="48e51-192">realm</span></span>|<span data-ttu-id="48e51-193">String</span><span class="sxs-lookup"><span data-stu-id="48e51-193">String</span></span>|<span data-ttu-id="48e51-194">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="48e51-194">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="48e51-195">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-195">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="48e51-196">servidores</span><span class="sxs-lookup"><span data-stu-id="48e51-196">servers</span></span>|<span data-ttu-id="48e51-197">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-197">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="48e51-198">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="48e51-198">List of VPN Servers on the network.</span></span> <span data-ttu-id="48e51-199">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="48e51-199">Make sure end users can access these network locations.</span></span> <span data-ttu-id="48e51-200">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="48e51-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="48e51-201">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="48e51-201">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="48e51-202">Connection</span><span class="sxs-lookup"><span data-stu-id="48e51-202">connectionType</span></span>|[<span data-ttu-id="48e51-203">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="48e51-203">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="48e51-204">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="48e51-204">Connection type.</span></span> <span data-ttu-id="48e51-205">Os possíveis valores são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="48e51-205">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|



## <a name="response"></a><span data-ttu-id="48e51-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="48e51-206">Response</span></span>
<span data-ttu-id="48e51-207">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48e51-207">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48e51-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="48e51-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="48e51-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48e51-209">Request</span></span>
<span data-ttu-id="48e51-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="48e51-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="48e51-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="48e51-211">Response</span></span>
<span data-ttu-id="48e51-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="48e51-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




