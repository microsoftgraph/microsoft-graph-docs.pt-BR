---
title: Criar androidDeviceOwnerVpnConfiguration
description: Criar um novo objeto androidDeviceOwnerVpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6730061b9136129b76ec3a8f08bac2d33a7fc3cb
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954871"
---
# <a name="create-androiddeviceownervpnconfiguration"></a><span data-ttu-id="103ba-103">Criar androidDeviceOwnerVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="103ba-103">Create androidDeviceOwnerVpnConfiguration</span></span>

> <span data-ttu-id="103ba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="103ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="103ba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="103ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="103ba-106">Criar um novo objeto [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="103ba-106">Create a new [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="103ba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="103ba-107">Prerequisites</span></span>
<span data-ttu-id="103ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="103ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="103ba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="103ba-110">Permission type</span></span>|<span data-ttu-id="103ba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="103ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="103ba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="103ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="103ba-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="103ba-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="103ba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="103ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="103ba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="103ba-115">Not supported.</span></span>|
|<span data-ttu-id="103ba-116">Application</span><span class="sxs-lookup"><span data-stu-id="103ba-116">Application</span></span>|<span data-ttu-id="103ba-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="103ba-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="103ba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="103ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="103ba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="103ba-119">Request headers</span></span>
|<span data-ttu-id="103ba-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="103ba-120">Header</span></span>|<span data-ttu-id="103ba-121">Valor</span><span class="sxs-lookup"><span data-stu-id="103ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="103ba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="103ba-122">Authorization</span></span>|<span data-ttu-id="103ba-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="103ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="103ba-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="103ba-124">Accept</span></span>|<span data-ttu-id="103ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="103ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="103ba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="103ba-126">Request body</span></span>
<span data-ttu-id="103ba-127">No corpo da solicitação, forneça uma representação JSON do objeto androidDeviceOwnerVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="103ba-127">In the request body, supply a JSON representation for the androidDeviceOwnerVpnConfiguration object.</span></span>

<span data-ttu-id="103ba-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="103ba-128">The following table shows the properties that are required when you create the androidDeviceOwnerVpnConfiguration.</span></span>

|<span data-ttu-id="103ba-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="103ba-129">Property</span></span>|<span data-ttu-id="103ba-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="103ba-130">Type</span></span>|<span data-ttu-id="103ba-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="103ba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="103ba-132">id</span><span class="sxs-lookup"><span data-stu-id="103ba-132">id</span></span>|<span data-ttu-id="103ba-133">String</span><span class="sxs-lookup"><span data-stu-id="103ba-133">String</span></span>|<span data-ttu-id="103ba-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="103ba-134">Key of the entity.</span></span> <span data-ttu-id="103ba-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="103ba-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="103ba-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="103ba-136">lastModifiedDateTime</span></span>|<span data-ttu-id="103ba-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="103ba-137">DateTimeOffset</span></span>|<span data-ttu-id="103ba-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="103ba-138">DateTime the object was last modified.</span></span> <span data-ttu-id="103ba-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="103ba-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="103ba-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="103ba-140">roleScopeTagIds</span></span>|<span data-ttu-id="103ba-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="103ba-141">String collection</span></span>|<span data-ttu-id="103ba-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="103ba-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="103ba-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="103ba-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="103ba-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="103ba-144">supportsScopeTags</span></span>|<span data-ttu-id="103ba-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="103ba-145">Boolean</span></span>|<span data-ttu-id="103ba-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="103ba-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="103ba-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="103ba-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="103ba-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="103ba-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="103ba-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="103ba-149">This property is read-only.</span></span> <span data-ttu-id="103ba-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="103ba-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="103ba-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="103ba-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="103ba-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="103ba-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="103ba-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="103ba-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="103ba-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="103ba-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="103ba-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="103ba-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="103ba-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="103ba-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="103ba-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="103ba-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="103ba-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="103ba-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="103ba-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="103ba-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="103ba-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="103ba-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="103ba-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="103ba-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="103ba-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="103ba-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="103ba-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="103ba-163">createdDateTime</span></span>|<span data-ttu-id="103ba-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="103ba-164">DateTimeOffset</span></span>|<span data-ttu-id="103ba-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="103ba-165">DateTime the object was created.</span></span> <span data-ttu-id="103ba-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="103ba-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="103ba-167">description</span><span class="sxs-lookup"><span data-stu-id="103ba-167">description</span></span>|<span data-ttu-id="103ba-168">String</span><span class="sxs-lookup"><span data-stu-id="103ba-168">String</span></span>|<span data-ttu-id="103ba-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="103ba-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="103ba-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="103ba-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="103ba-171">displayName</span><span class="sxs-lookup"><span data-stu-id="103ba-171">displayName</span></span>|<span data-ttu-id="103ba-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="103ba-172">String</span></span>|<span data-ttu-id="103ba-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="103ba-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="103ba-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="103ba-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="103ba-175">versão</span><span class="sxs-lookup"><span data-stu-id="103ba-175">version</span></span>|<span data-ttu-id="103ba-176">Int32</span><span class="sxs-lookup"><span data-stu-id="103ba-176">Int32</span></span>|<span data-ttu-id="103ba-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="103ba-177">Version of the device configuration.</span></span> <span data-ttu-id="103ba-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="103ba-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="103ba-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="103ba-179">authenticationMethod</span></span>|[<span data-ttu-id="103ba-180">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="103ba-180">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="103ba-181">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="103ba-181">Authentication method.</span></span> <span data-ttu-id="103ba-182">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="103ba-182">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="103ba-183">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="103ba-183">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="103ba-184">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="103ba-184">connectionName</span></span>|<span data-ttu-id="103ba-185">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="103ba-185">String</span></span>|<span data-ttu-id="103ba-186">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="103ba-186">Connection name displayed to the user.</span></span> <span data-ttu-id="103ba-187">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="103ba-187">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="103ba-188">role</span><span class="sxs-lookup"><span data-stu-id="103ba-188">role</span></span>|<span data-ttu-id="103ba-189">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="103ba-189">String</span></span>|<span data-ttu-id="103ba-190">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="103ba-190">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="103ba-191">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="103ba-191">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="103ba-192">esfera</span><span class="sxs-lookup"><span data-stu-id="103ba-192">realm</span></span>|<span data-ttu-id="103ba-193">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="103ba-193">String</span></span>|<span data-ttu-id="103ba-194">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="103ba-194">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="103ba-195">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="103ba-195">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="103ba-196">servidores</span><span class="sxs-lookup"><span data-stu-id="103ba-196">servers</span></span>|<span data-ttu-id="103ba-197">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="103ba-197">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="103ba-198">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="103ba-198">List of VPN Servers on the network.</span></span> <span data-ttu-id="103ba-199">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="103ba-199">Make sure end users can access these network locations.</span></span> <span data-ttu-id="103ba-200">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="103ba-200">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="103ba-201">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="103ba-201">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="103ba-202">Connection</span><span class="sxs-lookup"><span data-stu-id="103ba-202">connectionType</span></span>|[<span data-ttu-id="103ba-203">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="103ba-203">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="103ba-204">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="103ba-204">Connection type.</span></span> <span data-ttu-id="103ba-205">Os possíveis valores são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="103ba-205">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|



## <a name="response"></a><span data-ttu-id="103ba-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="103ba-206">Response</span></span>
<span data-ttu-id="103ba-207">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="103ba-207">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="103ba-208">Exemplo</span><span class="sxs-lookup"><span data-stu-id="103ba-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="103ba-209">Solicitação</span><span class="sxs-lookup"><span data-stu-id="103ba-209">Request</span></span>
<span data-ttu-id="103ba-210">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="103ba-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="103ba-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="103ba-211">Response</span></span>
<span data-ttu-id="103ba-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="103ba-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





