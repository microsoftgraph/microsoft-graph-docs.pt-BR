---
title: Atualizar androidVpnConfiguration
description: Atualiza as propriedades de um objeto androidVpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 065c77d360f45d21b53a75b1adfacf7896b4c4e5
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954696"
---
# <a name="update-androidvpnconfiguration"></a><span data-ttu-id="edcde-103">Atualizar androidVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="edcde-103">Update androidVpnConfiguration</span></span>

> <span data-ttu-id="edcde-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="edcde-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edcde-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="edcde-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edcde-106">Atualiza as propriedades de um objeto [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="edcde-106">Update the properties of a [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="edcde-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="edcde-107">Prerequisites</span></span>
<span data-ttu-id="edcde-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edcde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edcde-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="edcde-110">Permission type</span></span>|<span data-ttu-id="edcde-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="edcde-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edcde-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="edcde-112">Delegated (work or school account)</span></span>|<span data-ttu-id="edcde-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edcde-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="edcde-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="edcde-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edcde-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="edcde-115">Not supported.</span></span>|
|<span data-ttu-id="edcde-116">Application</span><span class="sxs-lookup"><span data-stu-id="edcde-116">Application</span></span>|<span data-ttu-id="edcde-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edcde-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="edcde-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="edcde-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="edcde-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="edcde-119">Request headers</span></span>
|<span data-ttu-id="edcde-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="edcde-120">Header</span></span>|<span data-ttu-id="edcde-121">Valor</span><span class="sxs-lookup"><span data-stu-id="edcde-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edcde-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="edcde-122">Authorization</span></span>|<span data-ttu-id="edcde-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="edcde-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edcde-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="edcde-124">Accept</span></span>|<span data-ttu-id="edcde-125">application/json</span><span class="sxs-lookup"><span data-stu-id="edcde-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edcde-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="edcde-126">Request body</span></span>
<span data-ttu-id="edcde-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="edcde-127">In the request body, supply a JSON representation for the [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>

<span data-ttu-id="edcde-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edcde-128">The following table shows the properties that are required when you create the [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md).</span></span>

|<span data-ttu-id="edcde-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="edcde-129">Property</span></span>|<span data-ttu-id="edcde-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="edcde-130">Type</span></span>|<span data-ttu-id="edcde-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="edcde-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edcde-132">id</span><span class="sxs-lookup"><span data-stu-id="edcde-132">id</span></span>|<span data-ttu-id="edcde-133">String</span><span class="sxs-lookup"><span data-stu-id="edcde-133">String</span></span>|<span data-ttu-id="edcde-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="edcde-134">Key of the entity.</span></span> <span data-ttu-id="edcde-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edcde-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edcde-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="edcde-136">lastModifiedDateTime</span></span>|<span data-ttu-id="edcde-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edcde-137">DateTimeOffset</span></span>|<span data-ttu-id="edcde-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="edcde-138">DateTime the object was last modified.</span></span> <span data-ttu-id="edcde-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edcde-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edcde-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="edcde-140">roleScopeTagIds</span></span>|<span data-ttu-id="edcde-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="edcde-141">String collection</span></span>|<span data-ttu-id="edcde-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="edcde-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="edcde-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edcde-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edcde-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="edcde-144">supportsScopeTags</span></span>|<span data-ttu-id="edcde-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="edcde-145">Boolean</span></span>|<span data-ttu-id="edcde-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="edcde-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="edcde-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="edcde-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="edcde-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="edcde-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="edcde-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="edcde-149">This property is read-only.</span></span> <span data-ttu-id="edcde-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edcde-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edcde-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="edcde-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="edcde-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="edcde-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="edcde-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="edcde-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="edcde-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edcde-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edcde-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="edcde-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="edcde-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="edcde-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="edcde-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="edcde-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="edcde-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edcde-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edcde-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="edcde-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="edcde-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="edcde-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="edcde-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="edcde-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="edcde-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edcde-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edcde-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="edcde-163">createdDateTime</span></span>|<span data-ttu-id="edcde-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edcde-164">DateTimeOffset</span></span>|<span data-ttu-id="edcde-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="edcde-165">DateTime the object was created.</span></span> <span data-ttu-id="edcde-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edcde-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edcde-167">description</span><span class="sxs-lookup"><span data-stu-id="edcde-167">description</span></span>|<span data-ttu-id="edcde-168">String</span><span class="sxs-lookup"><span data-stu-id="edcde-168">String</span></span>|<span data-ttu-id="edcde-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="edcde-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="edcde-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edcde-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edcde-171">displayName</span><span class="sxs-lookup"><span data-stu-id="edcde-171">displayName</span></span>|<span data-ttu-id="edcde-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="edcde-172">String</span></span>|<span data-ttu-id="edcde-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="edcde-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="edcde-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edcde-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edcde-175">versão</span><span class="sxs-lookup"><span data-stu-id="edcde-175">version</span></span>|<span data-ttu-id="edcde-176">Int32</span><span class="sxs-lookup"><span data-stu-id="edcde-176">Int32</span></span>|<span data-ttu-id="edcde-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="edcde-177">Version of the device configuration.</span></span> <span data-ttu-id="edcde-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="edcde-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="edcde-179">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="edcde-179">connectionName</span></span>|<span data-ttu-id="edcde-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="edcde-180">String</span></span>|<span data-ttu-id="edcde-181">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="edcde-181">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="edcde-182">Connection</span><span class="sxs-lookup"><span data-stu-id="edcde-182">connectionType</span></span>|[<span data-ttu-id="edcde-183">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="edcde-183">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="edcde-184">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="edcde-184">Connection type.</span></span> <span data-ttu-id="edcde-185">Os possíveis valores são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="edcde-185">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="edcde-186">role</span><span class="sxs-lookup"><span data-stu-id="edcde-186">role</span></span>|<span data-ttu-id="edcde-187">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="edcde-187">String</span></span>|<span data-ttu-id="edcde-188">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="edcde-188">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="edcde-189">esfera</span><span class="sxs-lookup"><span data-stu-id="edcde-189">realm</span></span>|<span data-ttu-id="edcde-190">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="edcde-190">String</span></span>|<span data-ttu-id="edcde-191">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="edcde-191">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="edcde-192">servidores</span><span class="sxs-lookup"><span data-stu-id="edcde-192">servers</span></span>|<span data-ttu-id="edcde-193">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="edcde-193">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="edcde-194">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="edcde-194">List of VPN Servers on the network.</span></span> <span data-ttu-id="edcde-195">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="edcde-195">Make sure end users can access these network locations.</span></span> <span data-ttu-id="edcde-196">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="edcde-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="edcde-197">digitais</span><span class="sxs-lookup"><span data-stu-id="edcde-197">fingerprint</span></span>|<span data-ttu-id="edcde-198">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="edcde-198">String</span></span>|<span data-ttu-id="edcde-199">A impressão digital é uma cadeia de caracteres que será usada para verificar se o servidor VPN pode ser confiável, o que só é aplicável quando o tipo de conexão é VPN cápsula de ponto de verificação.</span><span class="sxs-lookup"><span data-stu-id="edcde-199">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="edcde-200">customData</span><span class="sxs-lookup"><span data-stu-id="edcde-200">customData</span></span>|<span data-ttu-id="edcde-201">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="edcde-201">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="edcde-202">Dados personalizados quando o tipo de conexão é definido como Citrix.</span><span class="sxs-lookup"><span data-stu-id="edcde-202">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="edcde-203">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="edcde-203">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="edcde-204">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="edcde-204">customKeyValueData</span></span>|<span data-ttu-id="edcde-205">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="edcde-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="edcde-206">Dados personalizados quando o tipo de conexão é definido como Citrix.</span><span class="sxs-lookup"><span data-stu-id="edcde-206">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="edcde-207">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="edcde-207">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="edcde-208">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="edcde-208">authenticationMethod</span></span>|[<span data-ttu-id="edcde-209">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="edcde-209">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="edcde-210">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="edcde-210">Authentication method.</span></span> <span data-ttu-id="edcde-211">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="edcde-211">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="edcde-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="edcde-212">Response</span></span>
<span data-ttu-id="edcde-213">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="edcde-213">If successful, this method returns a `200 OK` response code and an updated [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edcde-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="edcde-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="edcde-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="edcde-215">Request</span></span>
<span data-ttu-id="edcde-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="edcde-216">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="edcde-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="edcde-217">Response</span></span>
<span data-ttu-id="edcde-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="edcde-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





