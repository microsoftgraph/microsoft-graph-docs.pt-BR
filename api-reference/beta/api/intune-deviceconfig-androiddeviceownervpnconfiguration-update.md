---
title: Atualizar androidDeviceOwnerVpnConfiguration
description: Atualiza as propriedades de um objeto androidDeviceOwnerVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6af039e59db358f75e560a76d45c5fb2bb48df0b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49240100"
---
# <a name="update-androiddeviceownervpnconfiguration"></a><span data-ttu-id="bb913-103">Atualizar androidDeviceOwnerVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb913-103">Update androidDeviceOwnerVpnConfiguration</span></span>

<span data-ttu-id="bb913-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb913-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb913-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bb913-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb913-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb913-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb913-107">Atualiza as propriedades de um objeto [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bb913-107">Update the properties of a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb913-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bb913-108">Prerequisites</span></span>
<span data-ttu-id="bb913-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb913-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb913-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb913-111">Permission type</span></span>|<span data-ttu-id="bb913-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bb913-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb913-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb913-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bb913-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb913-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb913-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb913-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb913-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb913-116">Not supported.</span></span>|
|<span data-ttu-id="bb913-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb913-117">Application</span></span>|<span data-ttu-id="bb913-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb913-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb913-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb913-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bb913-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb913-120">Request headers</span></span>
|<span data-ttu-id="bb913-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb913-121">Header</span></span>|<span data-ttu-id="bb913-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bb913-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb913-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb913-123">Authorization</span></span>|<span data-ttu-id="bb913-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb913-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb913-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bb913-125">Accept</span></span>|<span data-ttu-id="bb913-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bb913-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb913-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb913-127">Request body</span></span>
<span data-ttu-id="bb913-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bb913-128">In the request body, supply a JSON representation for the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

<span data-ttu-id="bb913-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb913-129">The following table shows the properties that are required when you create the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).</span></span>

|<span data-ttu-id="bb913-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb913-130">Property</span></span>|<span data-ttu-id="bb913-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb913-131">Type</span></span>|<span data-ttu-id="bb913-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb913-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb913-133">id</span><span class="sxs-lookup"><span data-stu-id="bb913-133">id</span></span>|<span data-ttu-id="bb913-134">String</span><span class="sxs-lookup"><span data-stu-id="bb913-134">String</span></span>|<span data-ttu-id="bb913-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bb913-135">Key of the entity.</span></span> <span data-ttu-id="bb913-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb913-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb913-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bb913-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb913-138">DateTimeOffset</span></span>|<span data-ttu-id="bb913-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="bb913-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bb913-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb913-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bb913-141">roleScopeTagIds</span></span>|<span data-ttu-id="bb913-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb913-142">String collection</span></span>|<span data-ttu-id="bb913-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="bb913-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bb913-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb913-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bb913-145">supportsScopeTags</span></span>|<span data-ttu-id="bb913-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb913-146">Boolean</span></span>|<span data-ttu-id="bb913-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="bb913-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bb913-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="bb913-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bb913-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="bb913-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bb913-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb913-150">This property is read-only.</span></span> <span data-ttu-id="bb913-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb913-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bb913-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bb913-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bb913-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bb913-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="bb913-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bb913-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb913-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bb913-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bb913-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bb913-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bb913-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="bb913-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bb913-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb913-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bb913-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bb913-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bb913-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bb913-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="bb913-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bb913-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb913-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb913-164">createdDateTime</span></span>|<span data-ttu-id="bb913-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb913-165">DateTimeOffset</span></span>|<span data-ttu-id="bb913-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="bb913-166">DateTime the object was created.</span></span> <span data-ttu-id="bb913-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb913-168">description</span><span class="sxs-lookup"><span data-stu-id="bb913-168">description</span></span>|<span data-ttu-id="bb913-169">String</span><span class="sxs-lookup"><span data-stu-id="bb913-169">String</span></span>|<span data-ttu-id="bb913-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb913-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bb913-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb913-172">displayName</span><span class="sxs-lookup"><span data-stu-id="bb913-172">displayName</span></span>|<span data-ttu-id="bb913-173">String</span><span class="sxs-lookup"><span data-stu-id="bb913-173">String</span></span>|<span data-ttu-id="bb913-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb913-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bb913-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb913-176">versão</span><span class="sxs-lookup"><span data-stu-id="bb913-176">version</span></span>|<span data-ttu-id="bb913-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bb913-177">Int32</span></span>|<span data-ttu-id="bb913-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bb913-178">Version of the device configuration.</span></span> <span data-ttu-id="bb913-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb913-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="bb913-180">authenticationMethod</span></span>|[<span data-ttu-id="bb913-181">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="bb913-181">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="bb913-182">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="bb913-182">Authentication method.</span></span> <span data-ttu-id="bb913-183">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb913-183">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="bb913-184">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="bb913-184">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="bb913-185">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="bb913-185">connectionName</span></span>|<span data-ttu-id="bb913-186">String</span><span class="sxs-lookup"><span data-stu-id="bb913-186">String</span></span>|<span data-ttu-id="bb913-187">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="bb913-187">Connection name displayed to the user.</span></span> <span data-ttu-id="bb913-188">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-188">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="bb913-189">role</span><span class="sxs-lookup"><span data-stu-id="bb913-189">role</span></span>|<span data-ttu-id="bb913-190">String</span><span class="sxs-lookup"><span data-stu-id="bb913-190">String</span></span>|<span data-ttu-id="bb913-191">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="bb913-191">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="bb913-192">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-192">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="bb913-193">esfera</span><span class="sxs-lookup"><span data-stu-id="bb913-193">realm</span></span>|<span data-ttu-id="bb913-194">String</span><span class="sxs-lookup"><span data-stu-id="bb913-194">String</span></span>|<span data-ttu-id="bb913-195">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="bb913-195">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="bb913-196">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-196">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="bb913-197">servidores</span><span class="sxs-lookup"><span data-stu-id="bb913-197">servers</span></span>|<span data-ttu-id="bb913-198">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="bb913-199">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="bb913-199">List of VPN Servers on the network.</span></span> <span data-ttu-id="bb913-200">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="bb913-200">Make sure end users can access these network locations.</span></span> <span data-ttu-id="bb913-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="bb913-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="bb913-202">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-202">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="bb913-203">Connection</span><span class="sxs-lookup"><span data-stu-id="bb913-203">connectionType</span></span>|[<span data-ttu-id="bb913-204">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="bb913-204">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="bb913-205">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="bb913-205">Connection type.</span></span> <span data-ttu-id="bb913-206">Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`.</span><span class="sxs-lookup"><span data-stu-id="bb913-206">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="bb913-207">proxyServer</span><span class="sxs-lookup"><span data-stu-id="bb913-207">proxyServer</span></span>|[<span data-ttu-id="bb913-208">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="bb913-208">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="bb913-209">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="bb913-209">Proxy server.</span></span>|
|<span data-ttu-id="bb913-210">targetedPackageIds</span><span class="sxs-lookup"><span data-stu-id="bb913-210">targetedPackageIds</span></span>|<span data-ttu-id="bb913-211">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb913-211">String collection</span></span>|<span data-ttu-id="bb913-212">IDs de pacote de aplicativos direcionados.</span><span class="sxs-lookup"><span data-stu-id="bb913-212">Targeted App package IDs.</span></span>|
|<span data-ttu-id="bb913-213">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="bb913-213">targetedMobileApps</span></span>|<span data-ttu-id="bb913-214">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-214">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bb913-215">Aplicativos móveis direcionados.</span><span class="sxs-lookup"><span data-stu-id="bb913-215">Targeted mobile apps.</span></span> <span data-ttu-id="bb913-216">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="bb913-216">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="bb913-217">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="bb913-217">alwaysOn</span></span>|<span data-ttu-id="bb913-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb913-218">Boolean</span></span>|<span data-ttu-id="bb913-219">Se a conexão VPN sempre ativa deve ou não ser habilitada.</span><span class="sxs-lookup"><span data-stu-id="bb913-219">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="bb913-220">alwaysOnLockdown</span><span class="sxs-lookup"><span data-stu-id="bb913-220">alwaysOnLockdown</span></span>|<span data-ttu-id="bb913-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="bb913-221">Boolean</span></span>|<span data-ttu-id="bb913-222">Se a conexão VPN sempre ativa estiver habilitada, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.</span><span class="sxs-lookup"><span data-stu-id="bb913-222">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="bb913-223">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="bb913-223">microsoftTunnelSiteId</span></span>|<span data-ttu-id="bb913-224">String</span><span class="sxs-lookup"><span data-stu-id="bb913-224">String</span></span>|<span data-ttu-id="bb913-225">ID de site de túnel da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="bb913-225">Microsoft Tunnel site ID.</span></span>|
|<span data-ttu-id="bb913-226">customData</span><span class="sxs-lookup"><span data-stu-id="bb913-226">customData</span></span>|<span data-ttu-id="bb913-227">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-227">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="bb913-228">Dados personalizados para definir pares de chave/valor específicos para um provedor VPN.</span><span class="sxs-lookup"><span data-stu-id="bb913-228">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="bb913-229">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="bb913-229">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="bb913-230">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="bb913-230">customKeyValueData</span></span>|<span data-ttu-id="bb913-231">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="bb913-231">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="bb913-232">Dados personalizados para definir pares de chave/valor específicos para um provedor VPN.</span><span class="sxs-lookup"><span data-stu-id="bb913-232">Custom data to define key/value pairs specific to a VPN provider.</span></span> <span data-ttu-id="bb913-233">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="bb913-233">This collection can contain a maximum of 25 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="bb913-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb913-234">Response</span></span>
<span data-ttu-id="bb913-235">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb913-235">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb913-236">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb913-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb913-237">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb913-237">Request</span></span>
<span data-ttu-id="bb913-238">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb913-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2383

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
  "connectionType": "pulseSecure",
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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="bb913-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb913-239">Response</span></span>
<span data-ttu-id="bb913-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb913-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2555

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
  "connectionType": "pulseSecure",
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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value",
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
  ]
}
```




