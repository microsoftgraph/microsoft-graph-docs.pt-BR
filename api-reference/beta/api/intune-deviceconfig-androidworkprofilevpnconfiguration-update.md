---
title: Atualizar androidWorkProfileVpnConfiguration
description: Atualiza as propriedades de um objeto androidWorkProfileVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 283524cfbf51540cb7ac8a1012c1bd4cb988f8ff
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123222"
---
# <a name="update-androidworkprofilevpnconfiguration"></a><span data-ttu-id="db82c-103">Atualizar androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="db82c-103">Update androidWorkProfileVpnConfiguration</span></span>

<span data-ttu-id="db82c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db82c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db82c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="db82c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db82c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db82c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db82c-107">Atualiza as propriedades de um objeto [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="db82c-107">Update the properties of a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db82c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="db82c-108">Prerequisites</span></span>
<span data-ttu-id="db82c-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="db82c-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="db82c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db82c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db82c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db82c-111">Permission type</span></span>|<span data-ttu-id="db82c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="db82c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db82c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db82c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db82c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db82c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db82c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db82c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db82c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db82c-116">Not supported.</span></span>|
|<span data-ttu-id="db82c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db82c-117">Application</span></span>|<span data-ttu-id="db82c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db82c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db82c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db82c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="db82c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db82c-120">Request headers</span></span>
|<span data-ttu-id="db82c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db82c-121">Header</span></span>|<span data-ttu-id="db82c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="db82c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db82c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="db82c-123">Authorization</span></span>|<span data-ttu-id="db82c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db82c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db82c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="db82c-125">Accept</span></span>|<span data-ttu-id="db82c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db82c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db82c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db82c-127">Request body</span></span>
<span data-ttu-id="db82c-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="db82c-128">In the request body, supply a JSON representation for the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

<span data-ttu-id="db82c-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db82c-129">The following table shows the properties that are required when you create the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>

|<span data-ttu-id="db82c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db82c-130">Property</span></span>|<span data-ttu-id="db82c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="db82c-131">Type</span></span>|<span data-ttu-id="db82c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="db82c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db82c-133">id</span><span class="sxs-lookup"><span data-stu-id="db82c-133">id</span></span>|<span data-ttu-id="db82c-134">String</span><span class="sxs-lookup"><span data-stu-id="db82c-134">String</span></span>|<span data-ttu-id="db82c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="db82c-135">Key of the entity.</span></span> <span data-ttu-id="db82c-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db82c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db82c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db82c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="db82c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db82c-138">DateTimeOffset</span></span>|<span data-ttu-id="db82c-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="db82c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="db82c-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db82c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db82c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="db82c-141">roleScopeTagIds</span></span>|<span data-ttu-id="db82c-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="db82c-142">String collection</span></span>|<span data-ttu-id="db82c-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="db82c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="db82c-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db82c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db82c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="db82c-145">supportsScopeTags</span></span>|<span data-ttu-id="db82c-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="db82c-146">Boolean</span></span>|<span data-ttu-id="db82c-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="db82c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="db82c-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="db82c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="db82c-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="db82c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="db82c-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="db82c-150">This property is read-only.</span></span> <span data-ttu-id="db82c-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db82c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db82c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="db82c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="db82c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="db82c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="db82c-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="db82c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="db82c-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db82c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db82c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="db82c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="db82c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="db82c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="db82c-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="db82c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="db82c-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db82c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db82c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="db82c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="db82c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="db82c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="db82c-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="db82c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="db82c-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db82c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db82c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db82c-164">createdDateTime</span></span>|<span data-ttu-id="db82c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db82c-165">DateTimeOffset</span></span>|<span data-ttu-id="db82c-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="db82c-166">DateTime the object was created.</span></span> <span data-ttu-id="db82c-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db82c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db82c-168">descrição</span><span class="sxs-lookup"><span data-stu-id="db82c-168">description</span></span>|<span data-ttu-id="db82c-169">String</span><span class="sxs-lookup"><span data-stu-id="db82c-169">String</span></span>|<span data-ttu-id="db82c-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db82c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="db82c-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db82c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db82c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="db82c-172">displayName</span></span>|<span data-ttu-id="db82c-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db82c-173">String</span></span>|<span data-ttu-id="db82c-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db82c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="db82c-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db82c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db82c-176">versão</span><span class="sxs-lookup"><span data-stu-id="db82c-176">version</span></span>|<span data-ttu-id="db82c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="db82c-177">Int32</span></span>|<span data-ttu-id="db82c-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db82c-178">Version of the device configuration.</span></span> <span data-ttu-id="db82c-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db82c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db82c-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="db82c-180">connectionName</span></span>|<span data-ttu-id="db82c-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db82c-181">String</span></span>|<span data-ttu-id="db82c-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="db82c-182">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="db82c-183">Connection</span><span class="sxs-lookup"><span data-stu-id="db82c-183">connectionType</span></span>|[<span data-ttu-id="db82c-184">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="db82c-184">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="db82c-185">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="db82c-185">Connection type.</span></span> <span data-ttu-id="db82c-186">Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`, `microsoftTunnel`.</span><span class="sxs-lookup"><span data-stu-id="db82c-186">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`, `microsoftTunnel`.</span></span>|
|<span data-ttu-id="db82c-187">role</span><span class="sxs-lookup"><span data-stu-id="db82c-187">role</span></span>|<span data-ttu-id="db82c-188">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db82c-188">String</span></span>|<span data-ttu-id="db82c-189">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="db82c-189">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="db82c-190">esfera</span><span class="sxs-lookup"><span data-stu-id="db82c-190">realm</span></span>|<span data-ttu-id="db82c-191">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db82c-191">String</span></span>|<span data-ttu-id="db82c-192">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="db82c-192">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="db82c-193">servidores</span><span class="sxs-lookup"><span data-stu-id="db82c-193">servers</span></span>|<span data-ttu-id="db82c-194">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="db82c-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="db82c-195">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="db82c-195">List of VPN Servers on the network.</span></span> <span data-ttu-id="db82c-196">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="db82c-196">Make sure end users can access these network locations.</span></span> <span data-ttu-id="db82c-197">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="db82c-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="db82c-198">digitais</span><span class="sxs-lookup"><span data-stu-id="db82c-198">fingerprint</span></span>|<span data-ttu-id="db82c-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db82c-199">String</span></span>|<span data-ttu-id="db82c-200">A impressão digital é uma cadeia de caracteres que será usada para verificar se o servidor VPN pode ser confiável, o que só é aplicável quando o tipo de conexão é VPN cápsula de ponto de verificação.</span><span class="sxs-lookup"><span data-stu-id="db82c-200">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="db82c-201">customData</span><span class="sxs-lookup"><span data-stu-id="db82c-201">customData</span></span>|<span data-ttu-id="db82c-202">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="db82c-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="db82c-203">Dados personalizados quando o tipo de conexão é definido como Citrix.</span><span class="sxs-lookup"><span data-stu-id="db82c-203">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="db82c-204">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="db82c-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="db82c-205">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="db82c-205">customKeyValueData</span></span>|<span data-ttu-id="db82c-206">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="db82c-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="db82c-207">Dados personalizados quando o tipo de conexão é definido como Citrix.</span><span class="sxs-lookup"><span data-stu-id="db82c-207">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="db82c-208">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="db82c-208">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="db82c-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="db82c-209">authenticationMethod</span></span>|[<span data-ttu-id="db82c-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="db82c-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="db82c-211">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="db82c-211">Authentication method.</span></span> <span data-ttu-id="db82c-212">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="db82c-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="db82c-213">proxyServer</span><span class="sxs-lookup"><span data-stu-id="db82c-213">proxyServer</span></span>|[<span data-ttu-id="db82c-214">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="db82c-214">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="db82c-215">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="db82c-215">Proxy server.</span></span>|
|<span data-ttu-id="db82c-216">targetedPackageIds</span><span class="sxs-lookup"><span data-stu-id="db82c-216">targetedPackageIds</span></span>|<span data-ttu-id="db82c-217">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="db82c-217">String collection</span></span>|<span data-ttu-id="db82c-218">IDs de pacote de aplicativos direcionados.</span><span class="sxs-lookup"><span data-stu-id="db82c-218">Targeted App package IDs.</span></span>|
|<span data-ttu-id="db82c-219">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="db82c-219">alwaysOn</span></span>|<span data-ttu-id="db82c-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="db82c-220">Boolean</span></span>|<span data-ttu-id="db82c-221">Se a conexão VPN sempre ativa deve ou não ser habilitada.</span><span class="sxs-lookup"><span data-stu-id="db82c-221">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="db82c-222">alwaysOnLockdown</span><span class="sxs-lookup"><span data-stu-id="db82c-222">alwaysOnLockdown</span></span>|<span data-ttu-id="db82c-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="db82c-223">Boolean</span></span>|<span data-ttu-id="db82c-224">Se a conexão VPN sempre ativa estiver habilitada, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.</span><span class="sxs-lookup"><span data-stu-id="db82c-224">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|



## <a name="response"></a><span data-ttu-id="db82c-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="db82c-225">Response</span></span>
<span data-ttu-id="db82c-226">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db82c-226">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db82c-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db82c-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="db82c-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db82c-228">Request</span></span>
<span data-ttu-id="db82c-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db82c-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2103

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
  "authenticationMethod": "usernameAndPassword",
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "targetedPackageIds": [
    "Targeted Package Ids value"
  ],
  "alwaysOn": true,
  "alwaysOnLockdown": true
}
```

### <a name="response"></a><span data-ttu-id="db82c-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="db82c-230">Response</span></span>
<span data-ttu-id="db82c-231">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="db82c-231">Here is an example of the response.</span></span> <span data-ttu-id="db82c-232">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="db82c-232">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="db82c-233">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="db82c-233">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2275

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
  "authenticationMethod": "usernameAndPassword",
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "targetedPackageIds": [
    "Targeted Package Ids value"
  ],
  "alwaysOn": true,
  "alwaysOnLockdown": true
}
```



