---
title: Atualizar androidVpnConfiguration
description: Atualiza as propriedades de um objeto androidVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 00e2a385af5f7dba317fd3794c04659f57c17105
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43435442"
---
# <a name="update-androidvpnconfiguration"></a><span data-ttu-id="ef0fc-103">Atualizar androidVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ef0fc-103">Update androidVpnConfiguration</span></span>

<span data-ttu-id="ef0fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef0fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef0fc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef0fc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef0fc-107">Atualiza as propriedades de um objeto [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ef0fc-107">Update the properties of a [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef0fc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef0fc-108">Prerequisites</span></span>
<span data-ttu-id="ef0fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef0fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef0fc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef0fc-111">Permission type</span></span>|<span data-ttu-id="ef0fc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef0fc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef0fc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef0fc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef0fc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef0fc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-116">Not supported.</span></span>|
|<span data-ttu-id="ef0fc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef0fc-117">Application</span></span>|<span data-ttu-id="ef0fc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef0fc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef0fc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef0fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ef0fc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef0fc-120">Request headers</span></span>
|<span data-ttu-id="ef0fc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef0fc-121">Header</span></span>|<span data-ttu-id="ef0fc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ef0fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef0fc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef0fc-123">Authorization</span></span>|<span data-ttu-id="ef0fc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef0fc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ef0fc-125">Accept</span></span>|<span data-ttu-id="ef0fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef0fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef0fc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef0fc-127">Request body</span></span>
<span data-ttu-id="ef0fc-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ef0fc-128">In the request body, supply a JSON representation for the [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>

<span data-ttu-id="ef0fc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ef0fc-129">The following table shows the properties that are required when you create the [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md).</span></span>

|<span data-ttu-id="ef0fc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef0fc-130">Property</span></span>|<span data-ttu-id="ef0fc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef0fc-131">Type</span></span>|<span data-ttu-id="ef0fc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef0fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef0fc-133">id</span><span class="sxs-lookup"><span data-stu-id="ef0fc-133">id</span></span>|<span data-ttu-id="ef0fc-134">String</span><span class="sxs-lookup"><span data-stu-id="ef0fc-134">String</span></span>|<span data-ttu-id="ef0fc-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-135">Key of the entity.</span></span> <span data-ttu-id="ef0fc-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0fc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef0fc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ef0fc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef0fc-138">DateTimeOffset</span></span>|<span data-ttu-id="ef0fc-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ef0fc-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0fc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ef0fc-141">roleScopeTagIds</span></span>|<span data-ttu-id="ef0fc-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="ef0fc-142">String collection</span></span>|<span data-ttu-id="ef0fc-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ef0fc-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0fc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ef0fc-145">supportsScopeTags</span></span>|<span data-ttu-id="ef0fc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef0fc-146">Boolean</span></span>|<span data-ttu-id="ef0fc-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ef0fc-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ef0fc-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ef0fc-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-150">This property is read-only.</span></span> <span data-ttu-id="ef0fc-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0fc-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ef0fc-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ef0fc-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ef0fc-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ef0fc-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ef0fc-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0fc-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ef0fc-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ef0fc-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ef0fc-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ef0fc-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ef0fc-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0fc-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ef0fc-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ef0fc-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ef0fc-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ef0fc-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ef0fc-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0fc-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef0fc-164">createdDateTime</span></span>|<span data-ttu-id="ef0fc-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef0fc-165">DateTimeOffset</span></span>|<span data-ttu-id="ef0fc-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-166">DateTime the object was created.</span></span> <span data-ttu-id="ef0fc-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0fc-168">description</span><span class="sxs-lookup"><span data-stu-id="ef0fc-168">description</span></span>|<span data-ttu-id="ef0fc-169">String</span><span class="sxs-lookup"><span data-stu-id="ef0fc-169">String</span></span>|<span data-ttu-id="ef0fc-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ef0fc-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0fc-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ef0fc-172">displayName</span></span>|<span data-ttu-id="ef0fc-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef0fc-173">String</span></span>|<span data-ttu-id="ef0fc-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ef0fc-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0fc-176">versão</span><span class="sxs-lookup"><span data-stu-id="ef0fc-176">version</span></span>|<span data-ttu-id="ef0fc-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ef0fc-177">Int32</span></span>|<span data-ttu-id="ef0fc-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-178">Version of the device configuration.</span></span> <span data-ttu-id="ef0fc-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0fc-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="ef0fc-180">connectionName</span></span>|<span data-ttu-id="ef0fc-181">String</span><span class="sxs-lookup"><span data-stu-id="ef0fc-181">String</span></span>|<span data-ttu-id="ef0fc-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-182">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="ef0fc-183">Connection</span><span class="sxs-lookup"><span data-stu-id="ef0fc-183">connectionType</span></span>|[<span data-ttu-id="ef0fc-184">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ef0fc-184">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="ef0fc-185">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-185">Connection type.</span></span> <span data-ttu-id="ef0fc-186">Os possíveis valores são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-186">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="ef0fc-187">role</span><span class="sxs-lookup"><span data-stu-id="ef0fc-187">role</span></span>|<span data-ttu-id="ef0fc-188">String</span><span class="sxs-lookup"><span data-stu-id="ef0fc-188">String</span></span>|<span data-ttu-id="ef0fc-189">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-189">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="ef0fc-190">esfera</span><span class="sxs-lookup"><span data-stu-id="ef0fc-190">realm</span></span>|<span data-ttu-id="ef0fc-191">String</span><span class="sxs-lookup"><span data-stu-id="ef0fc-191">String</span></span>|<span data-ttu-id="ef0fc-192">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-192">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="ef0fc-193">servidores</span><span class="sxs-lookup"><span data-stu-id="ef0fc-193">servers</span></span>|<span data-ttu-id="ef0fc-194">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="ef0fc-195">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-195">List of VPN Servers on the network.</span></span> <span data-ttu-id="ef0fc-196">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-196">Make sure end users can access these network locations.</span></span> <span data-ttu-id="ef0fc-197">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ef0fc-198">digitais</span><span class="sxs-lookup"><span data-stu-id="ef0fc-198">fingerprint</span></span>|<span data-ttu-id="ef0fc-199">String</span><span class="sxs-lookup"><span data-stu-id="ef0fc-199">String</span></span>|<span data-ttu-id="ef0fc-200">A impressão digital é uma cadeia de caracteres que será usada para verificar se o servidor VPN pode ser confiável, o que só é aplicável quando o tipo de conexão é VPN cápsula de ponto de verificação.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-200">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="ef0fc-201">customData</span><span class="sxs-lookup"><span data-stu-id="ef0fc-201">customData</span></span>|<span data-ttu-id="ef0fc-202">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="ef0fc-203">Dados personalizados quando o tipo de conexão é definido como Citrix.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-203">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="ef0fc-204">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="ef0fc-205">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="ef0fc-205">customKeyValueData</span></span>|<span data-ttu-id="ef0fc-206">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ef0fc-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ef0fc-207">Dados personalizados quando o tipo de conexão é definido como Citrix.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-207">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="ef0fc-208">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-208">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="ef0fc-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ef0fc-209">authenticationMethod</span></span>|[<span data-ttu-id="ef0fc-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ef0fc-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="ef0fc-211">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-211">Authentication method.</span></span> <span data-ttu-id="ef0fc-212">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="ef0fc-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef0fc-213">Response</span></span>
<span data-ttu-id="ef0fc-214">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-214">If successful, this method returns a `200 OK` response code and an updated [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef0fc-215">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef0fc-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef0fc-216">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef0fc-216">Request</span></span>
<span data-ttu-id="ef0fc-217">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-217">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1751

{
  "@odata.type": "#microsoft.graph.androidVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="ef0fc-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef0fc-218">Response</span></span>
<span data-ttu-id="ef0fc-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef0fc-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1923

{
  "@odata.type": "#microsoft.graph.androidVpnConfiguration",
  "id": "d4c48852-8852-d4c4-5288-c4d45288c4d4",
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



