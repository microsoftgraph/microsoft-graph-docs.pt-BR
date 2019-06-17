---
title: Criar androidWorkProfileVpnConfiguration
description: Criar um novo objeto androidWorkProfileVpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2e42962029ba931df9bf0908831f4f737da84e9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968998"
---
# <a name="create-androidworkprofilevpnconfiguration"></a><span data-ttu-id="fa0c1-103">Criar androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="fa0c1-103">Create androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="fa0c1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa0c1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa0c1-106">Criar um novo objeto [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fa0c1-106">Create a new [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa0c1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fa0c1-107">Prerequisites</span></span>
<span data-ttu-id="fa0c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa0c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa0c1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa0c1-110">Permission type</span></span>|<span data-ttu-id="fa0c1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa0c1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa0c1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa0c1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fa0c1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa0c1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-115">Not supported.</span></span>|
|<span data-ttu-id="fa0c1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa0c1-116">Application</span></span>|<span data-ttu-id="fa0c1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa0c1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa0c1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fa0c1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa0c1-119">Request headers</span></span>
|<span data-ttu-id="fa0c1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa0c1-120">Header</span></span>|<span data-ttu-id="fa0c1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fa0c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa0c1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa0c1-122">Authorization</span></span>|<span data-ttu-id="fa0c1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa0c1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fa0c1-124">Accept</span></span>|<span data-ttu-id="fa0c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa0c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa0c1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa0c1-126">Request body</span></span>
<span data-ttu-id="fa0c1-127">No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfileVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-127">In the request body, supply a JSON representation for the androidWorkProfileVpnConfiguration object.</span></span>

<span data-ttu-id="fa0c1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWorkProfileVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-128">The following table shows the properties that are required when you create the androidWorkProfileVpnConfiguration.</span></span>

|<span data-ttu-id="fa0c1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa0c1-129">Property</span></span>|<span data-ttu-id="fa0c1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa0c1-130">Type</span></span>|<span data-ttu-id="fa0c1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa0c1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa0c1-132">id</span><span class="sxs-lookup"><span data-stu-id="fa0c1-132">id</span></span>|<span data-ttu-id="fa0c1-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa0c1-133">String</span></span>|<span data-ttu-id="fa0c1-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-134">Key of the entity.</span></span> <span data-ttu-id="fa0c1-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa0c1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa0c1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fa0c1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa0c1-137">DateTimeOffset</span></span>|<span data-ttu-id="fa0c1-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="fa0c1-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa0c1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fa0c1-140">roleScopeTagIds</span></span>|<span data-ttu-id="fa0c1-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fa0c1-141">String collection</span></span>|<span data-ttu-id="fa0c1-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fa0c1-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa0c1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fa0c1-144">supportsScopeTags</span></span>|<span data-ttu-id="fa0c1-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="fa0c1-145">Boolean</span></span>|<span data-ttu-id="fa0c1-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fa0c1-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fa0c1-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fa0c1-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-149">This property is read-only.</span></span> <span data-ttu-id="fa0c1-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa0c1-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fa0c1-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fa0c1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fa0c1-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fa0c1-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fa0c1-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa0c1-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fa0c1-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fa0c1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fa0c1-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fa0c1-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fa0c1-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa0c1-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fa0c1-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fa0c1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fa0c1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fa0c1-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fa0c1-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa0c1-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa0c1-163">createdDateTime</span></span>|<span data-ttu-id="fa0c1-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa0c1-164">DateTimeOffset</span></span>|<span data-ttu-id="fa0c1-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-165">DateTime the object was created.</span></span> <span data-ttu-id="fa0c1-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa0c1-167">descrição</span><span class="sxs-lookup"><span data-stu-id="fa0c1-167">description</span></span>|<span data-ttu-id="fa0c1-168">String</span><span class="sxs-lookup"><span data-stu-id="fa0c1-168">String</span></span>|<span data-ttu-id="fa0c1-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fa0c1-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa0c1-171">displayName</span><span class="sxs-lookup"><span data-stu-id="fa0c1-171">displayName</span></span>|<span data-ttu-id="fa0c1-172">String</span><span class="sxs-lookup"><span data-stu-id="fa0c1-172">String</span></span>|<span data-ttu-id="fa0c1-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fa0c1-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa0c1-175">versão</span><span class="sxs-lookup"><span data-stu-id="fa0c1-175">version</span></span>|<span data-ttu-id="fa0c1-176">Int32</span><span class="sxs-lookup"><span data-stu-id="fa0c1-176">Int32</span></span>|<span data-ttu-id="fa0c1-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-177">Version of the device configuration.</span></span> <span data-ttu-id="fa0c1-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa0c1-179">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="fa0c1-179">connectionName</span></span>|<span data-ttu-id="fa0c1-180">String</span><span class="sxs-lookup"><span data-stu-id="fa0c1-180">String</span></span>|<span data-ttu-id="fa0c1-181">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-181">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="fa0c1-182">Connection</span><span class="sxs-lookup"><span data-stu-id="fa0c1-182">connectionType</span></span>|[<span data-ttu-id="fa0c1-183">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="fa0c1-183">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="fa0c1-184">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-184">Connection type.</span></span> <span data-ttu-id="fa0c1-185">Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-185">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="fa0c1-186">role</span><span class="sxs-lookup"><span data-stu-id="fa0c1-186">role</span></span>|<span data-ttu-id="fa0c1-187">String</span><span class="sxs-lookup"><span data-stu-id="fa0c1-187">String</span></span>|<span data-ttu-id="fa0c1-188">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-188">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="fa0c1-189">esfera</span><span class="sxs-lookup"><span data-stu-id="fa0c1-189">realm</span></span>|<span data-ttu-id="fa0c1-190">String</span><span class="sxs-lookup"><span data-stu-id="fa0c1-190">String</span></span>|<span data-ttu-id="fa0c1-191">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-191">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="fa0c1-192">servidores</span><span class="sxs-lookup"><span data-stu-id="fa0c1-192">servers</span></span>|<span data-ttu-id="fa0c1-193">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-193">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="fa0c1-194">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-194">List of VPN Servers on the network.</span></span> <span data-ttu-id="fa0c1-195">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-195">Make sure end users can access these network locations.</span></span> <span data-ttu-id="fa0c1-196">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="fa0c1-197">digitais</span><span class="sxs-lookup"><span data-stu-id="fa0c1-197">fingerprint</span></span>|<span data-ttu-id="fa0c1-198">String</span><span class="sxs-lookup"><span data-stu-id="fa0c1-198">String</span></span>|<span data-ttu-id="fa0c1-199">A impressão digital é uma cadeia de caracteres que será usada para verificar se o servidor VPN pode ser confiável, o que só é aplicável quando o tipo de conexão é VPN cápsula de ponto de verificação.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-199">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="fa0c1-200">customData</span><span class="sxs-lookup"><span data-stu-id="fa0c1-200">customData</span></span>|<span data-ttu-id="fa0c1-201">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-201">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="fa0c1-202">Dados personalizados quando o tipo de conexão é definido como Citrix.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-202">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="fa0c1-203">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-203">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="fa0c1-204">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="fa0c1-204">customKeyValueData</span></span>|<span data-ttu-id="fa0c1-205">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="fa0c1-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="fa0c1-206">Dados personalizados quando o tipo de conexão é definido como Citrix.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-206">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="fa0c1-207">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-207">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="fa0c1-208">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fa0c1-208">authenticationMethod</span></span>|[<span data-ttu-id="fa0c1-209">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fa0c1-209">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="fa0c1-210">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-210">Authentication method.</span></span> <span data-ttu-id="fa0c1-211">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-211">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="fa0c1-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa0c1-212">Response</span></span>
<span data-ttu-id="fa0c1-213">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-213">If successful, this method returns a `201 Created` response code and a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa0c1-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa0c1-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa0c1-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa0c1-215">Request</span></span>
<span data-ttu-id="fa0c1-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1762

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="fa0c1-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa0c1-217">Response</span></span>
<span data-ttu-id="fa0c1-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fa0c1-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1934

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
  "id": "32910378-0378-3291-7803-913278039132",
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





