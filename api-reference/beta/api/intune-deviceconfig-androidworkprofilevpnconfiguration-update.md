---
title: Atualizar androidWorkProfileVpnConfiguration
description: Atualiza as propriedades de um objeto androidWorkProfileVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8f1b70cb5c6599584c812fdfe35a38f633277d00
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49226297"
---
# <a name="update-androidworkprofilevpnconfiguration"></a><span data-ttu-id="1995f-103">Atualizar androidWorkProfileVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="1995f-103">Update androidWorkProfileVpnConfiguration</span></span>

<span data-ttu-id="1995f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1995f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1995f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1995f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1995f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1995f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1995f-107">Atualiza as propriedades de um objeto [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1995f-107">Update the properties of a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1995f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1995f-108">Prerequisites</span></span>
<span data-ttu-id="1995f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1995f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1995f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1995f-111">Permission type</span></span>|<span data-ttu-id="1995f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1995f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1995f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1995f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1995f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1995f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1995f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1995f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1995f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1995f-116">Not supported.</span></span>|
|<span data-ttu-id="1995f-117">Application</span><span class="sxs-lookup"><span data-stu-id="1995f-117">Application</span></span>|<span data-ttu-id="1995f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1995f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1995f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1995f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1995f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1995f-120">Request headers</span></span>
|<span data-ttu-id="1995f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1995f-121">Header</span></span>|<span data-ttu-id="1995f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1995f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1995f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1995f-123">Authorization</span></span>|<span data-ttu-id="1995f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1995f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1995f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1995f-125">Accept</span></span>|<span data-ttu-id="1995f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1995f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1995f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1995f-127">Request body</span></span>
<span data-ttu-id="1995f-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1995f-128">In the request body, supply a JSON representation for the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

<span data-ttu-id="1995f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1995f-129">The following table shows the properties that are required when you create the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>

|<span data-ttu-id="1995f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1995f-130">Property</span></span>|<span data-ttu-id="1995f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1995f-131">Type</span></span>|<span data-ttu-id="1995f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1995f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1995f-133">id</span><span class="sxs-lookup"><span data-stu-id="1995f-133">id</span></span>|<span data-ttu-id="1995f-134">String</span><span class="sxs-lookup"><span data-stu-id="1995f-134">String</span></span>|<span data-ttu-id="1995f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1995f-135">Key of the entity.</span></span> <span data-ttu-id="1995f-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1995f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1995f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1995f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1995f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1995f-138">DateTimeOffset</span></span>|<span data-ttu-id="1995f-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1995f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1995f-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1995f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1995f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1995f-141">roleScopeTagIds</span></span>|<span data-ttu-id="1995f-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1995f-142">String collection</span></span>|<span data-ttu-id="1995f-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="1995f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1995f-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1995f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1995f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1995f-145">supportsScopeTags</span></span>|<span data-ttu-id="1995f-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="1995f-146">Boolean</span></span>|<span data-ttu-id="1995f-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="1995f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1995f-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="1995f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1995f-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="1995f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1995f-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1995f-150">This property is read-only.</span></span> <span data-ttu-id="1995f-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1995f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1995f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1995f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1995f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1995f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1995f-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="1995f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1995f-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1995f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1995f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1995f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1995f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1995f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1995f-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="1995f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1995f-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1995f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1995f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1995f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1995f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1995f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1995f-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="1995f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1995f-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1995f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1995f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1995f-164">createdDateTime</span></span>|<span data-ttu-id="1995f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1995f-165">DateTimeOffset</span></span>|<span data-ttu-id="1995f-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1995f-166">DateTime the object was created.</span></span> <span data-ttu-id="1995f-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1995f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1995f-168">description</span><span class="sxs-lookup"><span data-stu-id="1995f-168">description</span></span>|<span data-ttu-id="1995f-169">String</span><span class="sxs-lookup"><span data-stu-id="1995f-169">String</span></span>|<span data-ttu-id="1995f-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1995f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1995f-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1995f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1995f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="1995f-172">displayName</span></span>|<span data-ttu-id="1995f-173">String</span><span class="sxs-lookup"><span data-stu-id="1995f-173">String</span></span>|<span data-ttu-id="1995f-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1995f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1995f-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1995f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1995f-176">versão</span><span class="sxs-lookup"><span data-stu-id="1995f-176">version</span></span>|<span data-ttu-id="1995f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1995f-177">Int32</span></span>|<span data-ttu-id="1995f-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1995f-178">Version of the device configuration.</span></span> <span data-ttu-id="1995f-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1995f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1995f-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="1995f-180">connectionName</span></span>|<span data-ttu-id="1995f-181">String</span><span class="sxs-lookup"><span data-stu-id="1995f-181">String</span></span>|<span data-ttu-id="1995f-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="1995f-182">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="1995f-183">Connection</span><span class="sxs-lookup"><span data-stu-id="1995f-183">connectionType</span></span>|[<span data-ttu-id="1995f-184">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="1995f-184">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="1995f-185">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="1995f-185">Connection type.</span></span> <span data-ttu-id="1995f-186">Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`, `microsoftTunnel`, `netMotionMobility`.</span><span class="sxs-lookup"><span data-stu-id="1995f-186">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="1995f-187">role</span><span class="sxs-lookup"><span data-stu-id="1995f-187">role</span></span>|<span data-ttu-id="1995f-188">String</span><span class="sxs-lookup"><span data-stu-id="1995f-188">String</span></span>|<span data-ttu-id="1995f-189">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="1995f-189">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="1995f-190">esfera</span><span class="sxs-lookup"><span data-stu-id="1995f-190">realm</span></span>|<span data-ttu-id="1995f-191">String</span><span class="sxs-lookup"><span data-stu-id="1995f-191">String</span></span>|<span data-ttu-id="1995f-192">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="1995f-192">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="1995f-193">servidores</span><span class="sxs-lookup"><span data-stu-id="1995f-193">servers</span></span>|<span data-ttu-id="1995f-194">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="1995f-194">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="1995f-195">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="1995f-195">List of VPN Servers on the network.</span></span> <span data-ttu-id="1995f-196">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="1995f-196">Make sure end users can access these network locations.</span></span> <span data-ttu-id="1995f-197">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="1995f-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1995f-198">digitais</span><span class="sxs-lookup"><span data-stu-id="1995f-198">fingerprint</span></span>|<span data-ttu-id="1995f-199">String</span><span class="sxs-lookup"><span data-stu-id="1995f-199">String</span></span>|<span data-ttu-id="1995f-200">A impressão digital é uma cadeia de caracteres que será usada para verificar se o servidor VPN pode ser confiável, o que só é aplicável quando o tipo de conexão é VPN cápsula de ponto de verificação.</span><span class="sxs-lookup"><span data-stu-id="1995f-200">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="1995f-201">customData</span><span class="sxs-lookup"><span data-stu-id="1995f-201">customData</span></span>|<span data-ttu-id="1995f-202">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="1995f-202">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="1995f-203">Dados personalizados quando o tipo de conexão é definido como Citrix.</span><span class="sxs-lookup"><span data-stu-id="1995f-203">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="1995f-204">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="1995f-204">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="1995f-205">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="1995f-205">customKeyValueData</span></span>|<span data-ttu-id="1995f-206">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="1995f-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="1995f-207">Dados personalizados quando o tipo de conexão é definido como Citrix.</span><span class="sxs-lookup"><span data-stu-id="1995f-207">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="1995f-208">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="1995f-208">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="1995f-209">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1995f-209">authenticationMethod</span></span>|[<span data-ttu-id="1995f-210">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1995f-210">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="1995f-211">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="1995f-211">Authentication method.</span></span> <span data-ttu-id="1995f-212">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="1995f-212">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="1995f-213">proxyServer</span><span class="sxs-lookup"><span data-stu-id="1995f-213">proxyServer</span></span>|[<span data-ttu-id="1995f-214">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="1995f-214">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="1995f-215">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="1995f-215">Proxy server.</span></span>|
|<span data-ttu-id="1995f-216">targetedPackageIds</span><span class="sxs-lookup"><span data-stu-id="1995f-216">targetedPackageIds</span></span>|<span data-ttu-id="1995f-217">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1995f-217">String collection</span></span>|<span data-ttu-id="1995f-218">IDs de pacote de aplicativos direcionados.</span><span class="sxs-lookup"><span data-stu-id="1995f-218">Targeted App package IDs.</span></span>|
|<span data-ttu-id="1995f-219">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="1995f-219">targetedMobileApps</span></span>|<span data-ttu-id="1995f-220">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="1995f-220">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1995f-221">Aplicativos móveis direcionados.</span><span class="sxs-lookup"><span data-stu-id="1995f-221">Targeted mobile apps.</span></span> <span data-ttu-id="1995f-222">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="1995f-222">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1995f-223">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="1995f-223">alwaysOn</span></span>|<span data-ttu-id="1995f-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="1995f-224">Boolean</span></span>|<span data-ttu-id="1995f-225">Se a conexão VPN sempre ativa deve ou não ser habilitada.</span><span class="sxs-lookup"><span data-stu-id="1995f-225">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="1995f-226">alwaysOnLockdown</span><span class="sxs-lookup"><span data-stu-id="1995f-226">alwaysOnLockdown</span></span>|<span data-ttu-id="1995f-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="1995f-227">Boolean</span></span>|<span data-ttu-id="1995f-228">Se a conexão VPN sempre ativa estiver habilitada, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.</span><span class="sxs-lookup"><span data-stu-id="1995f-228">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="1995f-229">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="1995f-229">microsoftTunnelSiteId</span></span>|<span data-ttu-id="1995f-230">String</span><span class="sxs-lookup"><span data-stu-id="1995f-230">String</span></span>|<span data-ttu-id="1995f-231">ID de site de túnel da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1995f-231">Microsoft Tunnel site ID.</span></span>|



## <a name="response"></a><span data-ttu-id="1995f-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="1995f-232">Response</span></span>
<span data-ttu-id="1995f-233">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1995f-233">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1995f-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1995f-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="1995f-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1995f-235">Request</span></span>
<span data-ttu-id="1995f-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1995f-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2422

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
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "alwaysOn": true,
  "alwaysOnLockdown": true,
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```

### <a name="response"></a><span data-ttu-id="1995f-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="1995f-237">Response</span></span>
<span data-ttu-id="1995f-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1995f-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2594

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
  "targetedMobileApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "alwaysOn": true,
  "alwaysOnLockdown": true,
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```




