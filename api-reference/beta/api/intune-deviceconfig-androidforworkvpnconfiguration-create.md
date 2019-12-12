---
title: Criar androidForWorkVpnConfiguration
description: Criar um novo objeto androidForWorkVpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2524121f2ec4cf1c14eb0f0d28b48eccf7e1766b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955004"
---
# <a name="create-androidforworkvpnconfiguration"></a><span data-ttu-id="de383-103">Criar androidForWorkVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="de383-103">Create androidForWorkVpnConfiguration</span></span>

> <span data-ttu-id="de383-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="de383-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de383-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de383-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de383-106">Criar um novo objeto [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="de383-106">Create a new [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de383-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="de383-107">Prerequisites</span></span>
<span data-ttu-id="de383-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de383-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de383-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de383-110">Permission type</span></span>|<span data-ttu-id="de383-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="de383-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de383-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de383-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de383-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de383-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="de383-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de383-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de383-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de383-115">Not supported.</span></span>|
|<span data-ttu-id="de383-116">Application</span><span class="sxs-lookup"><span data-stu-id="de383-116">Application</span></span>|<span data-ttu-id="de383-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de383-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de383-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de383-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="de383-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de383-119">Request headers</span></span>
|<span data-ttu-id="de383-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de383-120">Header</span></span>|<span data-ttu-id="de383-121">Valor</span><span class="sxs-lookup"><span data-stu-id="de383-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de383-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="de383-122">Authorization</span></span>|<span data-ttu-id="de383-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de383-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de383-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="de383-124">Accept</span></span>|<span data-ttu-id="de383-125">application/json</span><span class="sxs-lookup"><span data-stu-id="de383-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de383-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de383-126">Request body</span></span>
<span data-ttu-id="de383-127">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="de383-127">In the request body, supply a JSON representation for the androidForWorkVpnConfiguration object.</span></span>

<span data-ttu-id="de383-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="de383-128">The following table shows the properties that are required when you create the androidForWorkVpnConfiguration.</span></span>

|<span data-ttu-id="de383-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de383-129">Property</span></span>|<span data-ttu-id="de383-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="de383-130">Type</span></span>|<span data-ttu-id="de383-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="de383-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de383-132">id</span><span class="sxs-lookup"><span data-stu-id="de383-132">id</span></span>|<span data-ttu-id="de383-133">String</span><span class="sxs-lookup"><span data-stu-id="de383-133">String</span></span>|<span data-ttu-id="de383-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="de383-134">Key of the entity.</span></span> <span data-ttu-id="de383-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de383-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de383-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de383-136">lastModifiedDateTime</span></span>|<span data-ttu-id="de383-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de383-137">DateTimeOffset</span></span>|<span data-ttu-id="de383-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="de383-138">DateTime the object was last modified.</span></span> <span data-ttu-id="de383-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de383-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de383-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="de383-140">roleScopeTagIds</span></span>|<span data-ttu-id="de383-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="de383-141">String collection</span></span>|<span data-ttu-id="de383-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="de383-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="de383-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de383-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de383-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="de383-144">supportsScopeTags</span></span>|<span data-ttu-id="de383-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="de383-145">Boolean</span></span>|<span data-ttu-id="de383-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="de383-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="de383-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="de383-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="de383-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="de383-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="de383-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="de383-149">This property is read-only.</span></span> <span data-ttu-id="de383-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de383-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de383-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="de383-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="de383-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="de383-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="de383-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="de383-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="de383-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de383-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de383-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="de383-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="de383-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="de383-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="de383-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="de383-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="de383-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de383-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de383-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="de383-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="de383-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="de383-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="de383-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="de383-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="de383-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de383-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de383-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de383-163">createdDateTime</span></span>|<span data-ttu-id="de383-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de383-164">DateTimeOffset</span></span>|<span data-ttu-id="de383-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="de383-165">DateTime the object was created.</span></span> <span data-ttu-id="de383-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de383-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de383-167">description</span><span class="sxs-lookup"><span data-stu-id="de383-167">description</span></span>|<span data-ttu-id="de383-168">String</span><span class="sxs-lookup"><span data-stu-id="de383-168">String</span></span>|<span data-ttu-id="de383-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de383-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="de383-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de383-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de383-171">displayName</span><span class="sxs-lookup"><span data-stu-id="de383-171">displayName</span></span>|<span data-ttu-id="de383-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de383-172">String</span></span>|<span data-ttu-id="de383-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de383-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="de383-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de383-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de383-175">versão</span><span class="sxs-lookup"><span data-stu-id="de383-175">version</span></span>|<span data-ttu-id="de383-176">Int32</span><span class="sxs-lookup"><span data-stu-id="de383-176">Int32</span></span>|<span data-ttu-id="de383-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="de383-177">Version of the device configuration.</span></span> <span data-ttu-id="de383-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="de383-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="de383-179">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="de383-179">connectionName</span></span>|<span data-ttu-id="de383-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="de383-180">String</span></span>|<span data-ttu-id="de383-181">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="de383-181">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="de383-182">Connection</span><span class="sxs-lookup"><span data-stu-id="de383-182">connectionType</span></span>|[<span data-ttu-id="de383-183">androidForWorkVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="de383-183">androidForWorkVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|<span data-ttu-id="de383-184">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="de383-184">Connection type.</span></span> <span data-ttu-id="de383-185">Os possíveis valores são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="de383-185">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="de383-186">role</span><span class="sxs-lookup"><span data-stu-id="de383-186">role</span></span>|<span data-ttu-id="de383-187">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="de383-187">String</span></span>|<span data-ttu-id="de383-188">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="de383-188">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="de383-189">esfera</span><span class="sxs-lookup"><span data-stu-id="de383-189">realm</span></span>|<span data-ttu-id="de383-190">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="de383-190">String</span></span>|<span data-ttu-id="de383-191">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="de383-191">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="de383-192">servidores</span><span class="sxs-lookup"><span data-stu-id="de383-192">servers</span></span>|<span data-ttu-id="de383-193">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="de383-193">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="de383-194">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="de383-194">List of VPN Servers on the network.</span></span> <span data-ttu-id="de383-195">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="de383-195">Make sure end users can access these network locations.</span></span> <span data-ttu-id="de383-196">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="de383-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="de383-197">digitais</span><span class="sxs-lookup"><span data-stu-id="de383-197">fingerprint</span></span>|<span data-ttu-id="de383-198">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="de383-198">String</span></span>|<span data-ttu-id="de383-199">A impressão digital é uma cadeia de caracteres que será usada para verificar se o servidor VPN pode ser confiável, o que só é aplicável quando o tipo de conexão é VPN cápsula de ponto de verificação.</span><span class="sxs-lookup"><span data-stu-id="de383-199">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="de383-200">customData</span><span class="sxs-lookup"><span data-stu-id="de383-200">customData</span></span>|<span data-ttu-id="de383-201">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="de383-201">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="de383-202">Dados personalizados quando o tipo de conexão é definido como Citrix.</span><span class="sxs-lookup"><span data-stu-id="de383-202">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="de383-203">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="de383-203">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="de383-204">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="de383-204">customKeyValueData</span></span>|<span data-ttu-id="de383-205">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="de383-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="de383-206">Dados personalizados quando o tipo de conexão é definido como Citrix.</span><span class="sxs-lookup"><span data-stu-id="de383-206">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="de383-207">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="de383-207">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="de383-208">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="de383-208">authenticationMethod</span></span>|[<span data-ttu-id="de383-209">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="de383-209">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="de383-210">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="de383-210">Authentication method.</span></span> <span data-ttu-id="de383-211">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="de383-211">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="de383-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="de383-212">Response</span></span>
<span data-ttu-id="de383-213">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de383-213">If successful, this method returns a `201 Created` response code and a [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de383-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de383-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="de383-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de383-215">Request</span></span>
<span data-ttu-id="de383-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de383-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1758

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="de383-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="de383-217">Response</span></span>
<span data-ttu-id="de383-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de383-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1930

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
  "id": "2cf4c52c-c52c-2cf4-2cc5-f42c2cc5f42c",
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





