---
title: Atualizar androidDeviceOwnerVpnConfiguration
description: Atualiza as propriedades de um objeto androidDeviceOwnerVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6121694f9beb977ff76fe7798575335190201a01
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123299"
---
# <a name="update-androiddeviceownervpnconfiguration"></a><span data-ttu-id="3ea12-103">Atualizar androidDeviceOwnerVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="3ea12-103">Update androidDeviceOwnerVpnConfiguration</span></span>

<span data-ttu-id="3ea12-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ea12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ea12-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3ea12-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ea12-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ea12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ea12-107">Atualiza as propriedades de um objeto [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3ea12-107">Update the properties of a [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ea12-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3ea12-108">Prerequisites</span></span>
<span data-ttu-id="3ea12-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3ea12-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3ea12-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ea12-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ea12-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ea12-111">Permission type</span></span>|<span data-ttu-id="3ea12-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3ea12-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ea12-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ea12-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ea12-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ea12-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3ea12-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ea12-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ea12-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ea12-116">Not supported.</span></span>|
|<span data-ttu-id="3ea12-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ea12-117">Application</span></span>|<span data-ttu-id="3ea12-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ea12-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ea12-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ea12-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3ea12-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ea12-120">Request headers</span></span>
|<span data-ttu-id="3ea12-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3ea12-121">Header</span></span>|<span data-ttu-id="3ea12-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3ea12-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ea12-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ea12-123">Authorization</span></span>|<span data-ttu-id="3ea12-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ea12-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ea12-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3ea12-125">Accept</span></span>|<span data-ttu-id="3ea12-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ea12-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ea12-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ea12-127">Request body</span></span>
<span data-ttu-id="3ea12-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3ea12-128">In the request body, supply a JSON representation for the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object.</span></span>

<span data-ttu-id="3ea12-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3ea12-129">The following table shows the properties that are required when you create the [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md).</span></span>

|<span data-ttu-id="3ea12-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ea12-130">Property</span></span>|<span data-ttu-id="3ea12-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ea12-131">Type</span></span>|<span data-ttu-id="3ea12-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ea12-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ea12-133">id</span><span class="sxs-lookup"><span data-stu-id="3ea12-133">id</span></span>|<span data-ttu-id="3ea12-134">String</span><span class="sxs-lookup"><span data-stu-id="3ea12-134">String</span></span>|<span data-ttu-id="3ea12-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3ea12-135">Key of the entity.</span></span> <span data-ttu-id="3ea12-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea12-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea12-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ea12-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3ea12-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ea12-138">DateTimeOffset</span></span>|<span data-ttu-id="3ea12-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3ea12-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3ea12-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea12-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea12-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3ea12-141">roleScopeTagIds</span></span>|<span data-ttu-id="3ea12-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ea12-142">String collection</span></span>|<span data-ttu-id="3ea12-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3ea12-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3ea12-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea12-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea12-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3ea12-145">supportsScopeTags</span></span>|<span data-ttu-id="3ea12-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="3ea12-146">Boolean</span></span>|<span data-ttu-id="3ea12-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="3ea12-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3ea12-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="3ea12-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3ea12-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="3ea12-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3ea12-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ea12-150">This property is read-only.</span></span> <span data-ttu-id="3ea12-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea12-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea12-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3ea12-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3ea12-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3ea12-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3ea12-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="3ea12-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3ea12-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea12-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea12-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3ea12-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3ea12-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3ea12-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3ea12-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="3ea12-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3ea12-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea12-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea12-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3ea12-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3ea12-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3ea12-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3ea12-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="3ea12-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3ea12-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea12-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea12-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ea12-164">createdDateTime</span></span>|<span data-ttu-id="3ea12-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ea12-165">DateTimeOffset</span></span>|<span data-ttu-id="3ea12-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3ea12-166">DateTime the object was created.</span></span> <span data-ttu-id="3ea12-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea12-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea12-168">descrição</span><span class="sxs-lookup"><span data-stu-id="3ea12-168">description</span></span>|<span data-ttu-id="3ea12-169">String</span><span class="sxs-lookup"><span data-stu-id="3ea12-169">String</span></span>|<span data-ttu-id="3ea12-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3ea12-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3ea12-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea12-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea12-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3ea12-172">displayName</span></span>|<span data-ttu-id="3ea12-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ea12-173">String</span></span>|<span data-ttu-id="3ea12-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3ea12-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3ea12-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea12-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea12-176">versão</span><span class="sxs-lookup"><span data-stu-id="3ea12-176">version</span></span>|<span data-ttu-id="3ea12-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3ea12-177">Int32</span></span>|<span data-ttu-id="3ea12-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3ea12-178">Version of the device configuration.</span></span> <span data-ttu-id="3ea12-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea12-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3ea12-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3ea12-180">authenticationMethod</span></span>|[<span data-ttu-id="3ea12-181">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3ea12-181">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="3ea12-182">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3ea12-182">Authentication method.</span></span> <span data-ttu-id="3ea12-183">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3ea12-183">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md).</span></span> <span data-ttu-id="3ea12-184">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="3ea12-184">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="3ea12-185">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="3ea12-185">connectionName</span></span>|<span data-ttu-id="3ea12-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ea12-186">String</span></span>|<span data-ttu-id="3ea12-187">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="3ea12-187">Connection name displayed to the user.</span></span> <span data-ttu-id="3ea12-188">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea12-188">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="3ea12-189">role</span><span class="sxs-lookup"><span data-stu-id="3ea12-189">role</span></span>|<span data-ttu-id="3ea12-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ea12-190">String</span></span>|<span data-ttu-id="3ea12-191">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="3ea12-191">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="3ea12-192">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea12-192">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="3ea12-193">esfera</span><span class="sxs-lookup"><span data-stu-id="3ea12-193">realm</span></span>|<span data-ttu-id="3ea12-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ea12-194">String</span></span>|<span data-ttu-id="3ea12-195">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="3ea12-195">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="3ea12-196">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea12-196">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="3ea12-197">servidores</span><span class="sxs-lookup"><span data-stu-id="3ea12-197">servers</span></span>|<span data-ttu-id="3ea12-198">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="3ea12-198">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="3ea12-199">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="3ea12-199">List of VPN Servers on the network.</span></span> <span data-ttu-id="3ea12-200">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="3ea12-200">Make sure end users can access these network locations.</span></span> <span data-ttu-id="3ea12-201">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="3ea12-201">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="3ea12-202">Herdado de [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3ea12-202">Inherited from [vpnConfiguration](../resources/intune-deviceconfig-vpnconfiguration.md)</span></span>|
|<span data-ttu-id="3ea12-203">Connection</span><span class="sxs-lookup"><span data-stu-id="3ea12-203">connectionType</span></span>|[<span data-ttu-id="3ea12-204">androidVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="3ea12-204">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="3ea12-205">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="3ea12-205">Connection type.</span></span> <span data-ttu-id="3ea12-206">Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`.</span><span class="sxs-lookup"><span data-stu-id="3ea12-206">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `microsoftTunnel`.</span></span>|
|<span data-ttu-id="3ea12-207">proxyServer</span><span class="sxs-lookup"><span data-stu-id="3ea12-207">proxyServer</span></span>|[<span data-ttu-id="3ea12-208">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="3ea12-208">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="3ea12-209">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="3ea12-209">Proxy server.</span></span>|
|<span data-ttu-id="3ea12-210">targetedPackageIds</span><span class="sxs-lookup"><span data-stu-id="3ea12-210">targetedPackageIds</span></span>|<span data-ttu-id="3ea12-211">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ea12-211">String collection</span></span>|<span data-ttu-id="3ea12-212">IDs de pacote de aplicativos direcionados.</span><span class="sxs-lookup"><span data-stu-id="3ea12-212">Targeted App package IDs.</span></span>|
|<span data-ttu-id="3ea12-213">alwaysOn</span><span class="sxs-lookup"><span data-stu-id="3ea12-213">alwaysOn</span></span>|<span data-ttu-id="3ea12-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="3ea12-214">Boolean</span></span>|<span data-ttu-id="3ea12-215">Se a conexão VPN sempre ativa deve ou não ser habilitada.</span><span class="sxs-lookup"><span data-stu-id="3ea12-215">Whether or not to enable always-on VPN connection.</span></span>|
|<span data-ttu-id="3ea12-216">alwaysOnLockdown</span><span class="sxs-lookup"><span data-stu-id="3ea12-216">alwaysOnLockdown</span></span>|<span data-ttu-id="3ea12-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="3ea12-217">Boolean</span></span>|<span data-ttu-id="3ea12-218">Se a conexão VPN sempre ativa estiver habilitada, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.</span><span class="sxs-lookup"><span data-stu-id="3ea12-218">If always-on VPN connection is enabled, whether or not to lock network traffic when that VPN is disconnected.</span></span>|



## <a name="response"></a><span data-ttu-id="3ea12-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ea12-219">Response</span></span>
<span data-ttu-id="3ea12-220">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ea12-220">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerVpnConfiguration](../resources/intune-deviceconfig-androiddeviceownervpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ea12-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ea12-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ea12-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ea12-222">Request</span></span>
<span data-ttu-id="3ea12-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ea12-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1758

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
  "alwaysOn": true,
  "alwaysOnLockdown": true
}
```

### <a name="response"></a><span data-ttu-id="3ea12-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ea12-224">Response</span></span>
<span data-ttu-id="3ea12-225">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="3ea12-225">Here is an example of the response.</span></span> <span data-ttu-id="3ea12-226">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="3ea12-226">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3ea12-227">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3ea12-227">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1930

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
  "alwaysOn": true,
  "alwaysOnLockdown": true
}
```



