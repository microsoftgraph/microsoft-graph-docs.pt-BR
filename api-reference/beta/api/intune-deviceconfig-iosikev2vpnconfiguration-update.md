---
title: Atualizar iosikEv2VpnConfiguration
description: Atualiza as propriedades de um objeto iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 265a124431e2c1e01cce1d87360717926b319150
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123082"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="b5aba-103">Atualizar iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b5aba-103">Update iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="b5aba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5aba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5aba-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b5aba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5aba-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b5aba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5aba-107">Atualiza as propriedades de um objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b5aba-107">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5aba-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b5aba-108">Prerequisites</span></span>
<span data-ttu-id="b5aba-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b5aba-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b5aba-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5aba-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5aba-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5aba-111">Permission type</span></span>|<span data-ttu-id="b5aba-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b5aba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5aba-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5aba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5aba-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5aba-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5aba-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5aba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5aba-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5aba-116">Not supported.</span></span>|
|<span data-ttu-id="b5aba-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5aba-117">Application</span></span>|<span data-ttu-id="b5aba-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5aba-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5aba-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5aba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b5aba-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5aba-120">Request headers</span></span>
|<span data-ttu-id="b5aba-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b5aba-121">Header</span></span>|<span data-ttu-id="b5aba-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b5aba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5aba-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5aba-123">Authorization</span></span>|<span data-ttu-id="b5aba-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5aba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5aba-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b5aba-125">Accept</span></span>|<span data-ttu-id="b5aba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5aba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5aba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5aba-127">Request body</span></span>
<span data-ttu-id="b5aba-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b5aba-128">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="b5aba-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5aba-129">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="b5aba-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5aba-130">Property</span></span>|<span data-ttu-id="b5aba-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5aba-131">Type</span></span>|<span data-ttu-id="b5aba-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5aba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5aba-133">id</span><span class="sxs-lookup"><span data-stu-id="b5aba-133">id</span></span>|<span data-ttu-id="b5aba-134">String</span><span class="sxs-lookup"><span data-stu-id="b5aba-134">String</span></span>|<span data-ttu-id="b5aba-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b5aba-135">Key of the entity.</span></span> <span data-ttu-id="b5aba-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5aba-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b5aba-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5aba-138">DateTimeOffset</span></span>|<span data-ttu-id="b5aba-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b5aba-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b5aba-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b5aba-141">roleScopeTagIds</span></span>|<span data-ttu-id="b5aba-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-142">String collection</span></span>|<span data-ttu-id="b5aba-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b5aba-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b5aba-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b5aba-145">supportsScopeTags</span></span>|<span data-ttu-id="b5aba-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5aba-146">Boolean</span></span>|<span data-ttu-id="b5aba-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b5aba-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b5aba-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b5aba-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b5aba-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b5aba-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b5aba-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b5aba-150">This property is read-only.</span></span> <span data-ttu-id="b5aba-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b5aba-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b5aba-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b5aba-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b5aba-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="b5aba-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b5aba-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b5aba-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b5aba-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b5aba-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b5aba-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="b5aba-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b5aba-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b5aba-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b5aba-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b5aba-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b5aba-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="b5aba-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b5aba-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5aba-164">createdDateTime</span></span>|<span data-ttu-id="b5aba-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5aba-165">DateTimeOffset</span></span>|<span data-ttu-id="b5aba-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b5aba-166">DateTime the object was created.</span></span> <span data-ttu-id="b5aba-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-168">descrição</span><span class="sxs-lookup"><span data-stu-id="b5aba-168">description</span></span>|<span data-ttu-id="b5aba-169">String</span><span class="sxs-lookup"><span data-stu-id="b5aba-169">String</span></span>|<span data-ttu-id="b5aba-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b5aba-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b5aba-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b5aba-172">displayName</span></span>|<span data-ttu-id="b5aba-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-173">String</span></span>|<span data-ttu-id="b5aba-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b5aba-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b5aba-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-176">versão</span><span class="sxs-lookup"><span data-stu-id="b5aba-176">version</span></span>|<span data-ttu-id="b5aba-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b5aba-177">Int32</span></span>|<span data-ttu-id="b5aba-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b5aba-178">Version of the device configuration.</span></span> <span data-ttu-id="b5aba-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="b5aba-180">connectionName</span></span>|<span data-ttu-id="b5aba-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-181">String</span></span>|<span data-ttu-id="b5aba-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="b5aba-182">Connection name displayed to the user.</span></span> <span data-ttu-id="b5aba-183">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-184">Connection</span><span class="sxs-lookup"><span data-stu-id="b5aba-184">connectionType</span></span>|[<span data-ttu-id="b5aba-185">Enumeraçãoapplevpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="b5aba-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="b5aba-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="b5aba-186">Connection type.</span></span> <span data-ttu-id="b5aba-187">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5aba-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="b5aba-188">Os valores possíveis são:, `ciscoAnyConnect` `pulseSecure` , `f5EdgeClient` , `dellSonicWallMobileConnect` , `checkPointCapsuleVpn` , `customVpn` ,,,,,,,,,,,,,,, `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` , `paloAltoGlobalProtectV2` , `ikEv2` , `alwaysOn` , `microsoftTunnel` .</span><span class="sxs-lookup"><span data-stu-id="b5aba-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`.</span></span>|
|<span data-ttu-id="b5aba-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="b5aba-189">loginGroupOrDomain</span></span>|<span data-ttu-id="b5aba-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-190">String</span></span>|<span data-ttu-id="b5aba-191">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="b5aba-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="b5aba-192">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-193">role</span><span class="sxs-lookup"><span data-stu-id="b5aba-193">role</span></span>|<span data-ttu-id="b5aba-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-194">String</span></span>|<span data-ttu-id="b5aba-195">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="b5aba-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="b5aba-196">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-197">esfera</span><span class="sxs-lookup"><span data-stu-id="b5aba-197">realm</span></span>|<span data-ttu-id="b5aba-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-198">String</span></span>|<span data-ttu-id="b5aba-199">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="b5aba-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="b5aba-200">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-201">do</span><span class="sxs-lookup"><span data-stu-id="b5aba-201">server</span></span>|[<span data-ttu-id="b5aba-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="b5aba-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="b5aba-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="b5aba-203">VPN Server on the network.</span></span> <span data-ttu-id="b5aba-204">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="b5aba-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="b5aba-205">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-206">identificador</span><span class="sxs-lookup"><span data-stu-id="b5aba-206">identifier</span></span>|<span data-ttu-id="b5aba-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-207">String</span></span>|<span data-ttu-id="b5aba-208">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="b5aba-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b5aba-209">Por exemplo: o Cisco AnyConnect usa um identificador do formulário com. Cisco. AnyConnect. applevpn. plugin herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-210">customData</span><span class="sxs-lookup"><span data-stu-id="b5aba-210">customData</span></span>|<span data-ttu-id="b5aba-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="b5aba-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="b5aba-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b5aba-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="b5aba-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="b5aba-214">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="b5aba-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="b5aba-215">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="b5aba-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="b5aba-216">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-217">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="b5aba-217">customKeyValueData</span></span>|<span data-ttu-id="b5aba-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b5aba-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="b5aba-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b5aba-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="b5aba-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="b5aba-221">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="b5aba-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="b5aba-222">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="b5aba-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="b5aba-223">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="b5aba-224">enableSplitTunneling</span></span>|<span data-ttu-id="b5aba-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5aba-225">Boolean</span></span>|<span data-ttu-id="b5aba-226">Enviar todo o tráfego de rede através da VPN.</span><span class="sxs-lookup"><span data-stu-id="b5aba-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="b5aba-227">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b5aba-228">authenticationMethod</span></span>|[<span data-ttu-id="b5aba-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b5aba-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="b5aba-230">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="b5aba-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="b5aba-231">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5aba-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="b5aba-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="b5aba-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="b5aba-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="b5aba-233">enablePerApp</span></span>|<span data-ttu-id="b5aba-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5aba-234">Boolean</span></span>|<span data-ttu-id="b5aba-235">A configuração dessa opção como true cria uma carga de VPN por aplicativo, que pode ser mais tarde associada aos aplicativos que podem acionar esta conexão VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="b5aba-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="b5aba-236">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="b5aba-237">safariDomains</span></span>|<span data-ttu-id="b5aba-238">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-238">String collection</span></span>|<span data-ttu-id="b5aba-239">Domínios Safari quando esta configuração VPN por aplicativo estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="b5aba-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="b5aba-240">Além dos aplicativos associados a essa VPN, os domínios Safari especificados aqui também serão capazes de acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="b5aba-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="b5aba-241">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="b5aba-242">onDemandRules</span></span>|<span data-ttu-id="b5aba-243">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="b5aba-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="b5aba-244">On-Demand Rules.</span></span> <span data-ttu-id="b5aba-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b5aba-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b5aba-246">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-247">proxyServer</span><span class="sxs-lookup"><span data-stu-id="b5aba-247">proxyServer</span></span>|[<span data-ttu-id="b5aba-248">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="b5aba-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="b5aba-249">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="b5aba-249">Proxy Server.</span></span> <span data-ttu-id="b5aba-250">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-251">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="b5aba-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="b5aba-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5aba-252">Boolean</span></span>|<span data-ttu-id="b5aba-253">Optar por compartilhar a ID do dispositivo para clientes VPN de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="b5aba-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="b5aba-254">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-255">providerType</span><span class="sxs-lookup"><span data-stu-id="b5aba-255">providerType</span></span>|[<span data-ttu-id="b5aba-256">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="b5aba-256">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="b5aba-257">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b5aba-257">Provider type for per-app VPN.</span></span> <span data-ttu-id="b5aba-258">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b5aba-258">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="b5aba-259">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="b5aba-259">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="b5aba-260">UserDomain</span><span class="sxs-lookup"><span data-stu-id="b5aba-260">userDomain</span></span>|<span data-ttu-id="b5aba-261">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-261">String</span></span>|<span data-ttu-id="b5aba-262">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="b5aba-262">Zscaler only.</span></span> <span data-ttu-id="b5aba-263">Insira um domínio estático para preencher previamente o campo de logon com no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="b5aba-263">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="b5aba-264">Se for deixado em branco, o domínio do Azure Active Directory do usuário será usado.</span><span class="sxs-lookup"><span data-stu-id="b5aba-264">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="b5aba-265">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-265">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-266">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="b5aba-266">strictEnforcement</span></span>|<span data-ttu-id="b5aba-267">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5aba-267">Boolean</span></span>|<span data-ttu-id="b5aba-268">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="b5aba-268">Zscaler only.</span></span> <span data-ttu-id="b5aba-269">Bloqueia o tráfego de rede até que o usuário entre no Zscaler app.</span><span class="sxs-lookup"><span data-stu-id="b5aba-269">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="b5aba-270">"True" significa que o tráfego é bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b5aba-270">"True" means traffic is blocked.</span></span> <span data-ttu-id="b5aba-271">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-272">cloudName</span><span class="sxs-lookup"><span data-stu-id="b5aba-272">cloudName</span></span>|<span data-ttu-id="b5aba-273">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-273">String</span></span>|<span data-ttu-id="b5aba-274">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="b5aba-274">Zscaler only.</span></span> <span data-ttu-id="b5aba-275">Nuvem do Zscaler à qual o usuário está atribuído.</span><span class="sxs-lookup"><span data-stu-id="b5aba-275">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="b5aba-276">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-276">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-277">Excludelistpara</span><span class="sxs-lookup"><span data-stu-id="b5aba-277">excludeList</span></span>|<span data-ttu-id="b5aba-278">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-278">String collection</span></span>|<span data-ttu-id="b5aba-279">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="b5aba-279">Zscaler only.</span></span> <span data-ttu-id="b5aba-280">Lista de endereços de rede que não são enviados pela nuvem do Zscaler.</span><span class="sxs-lookup"><span data-stu-id="b5aba-280">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="b5aba-281">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-281">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-282">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="b5aba-282">targetedMobileApps</span></span>|<span data-ttu-id="b5aba-283">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-283">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b5aba-284">Aplicativos móveis direcionados.</span><span class="sxs-lookup"><span data-stu-id="b5aba-284">Targeted mobile apps.</span></span> <span data-ttu-id="b5aba-285">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b5aba-285">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b5aba-286">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b5aba-286">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b5aba-287">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="b5aba-287">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="b5aba-288">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="b5aba-288">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="b5aba-289">Parâmetros da Associação de segurança filho</span><span class="sxs-lookup"><span data-stu-id="b5aba-289">Child Security Association Parameters</span></span>|
|<span data-ttu-id="b5aba-290">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="b5aba-290">clientAuthenticationType</span></span>|[<span data-ttu-id="b5aba-291">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="b5aba-291">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="b5aba-292">Tipo de autenticação de cliente que o cliente VPN usará.</span><span class="sxs-lookup"><span data-stu-id="b5aba-292">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="b5aba-293">Os valores possíveis são: `userAuthentication` e `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="b5aba-293">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="b5aba-294">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="b5aba-294">deadPeerDetectionRate</span></span>|[<span data-ttu-id="b5aba-295">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="b5aba-295">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="b5aba-296">Determinar a frequência de verificação de uma conexão de mesmo nível.</span><span class="sxs-lookup"><span data-stu-id="b5aba-296">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="b5aba-297">.</span><span class="sxs-lookup"><span data-stu-id="b5aba-297">.</span></span> <span data-ttu-id="b5aba-298">Os valores possíveis são: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="b5aba-298">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="b5aba-299">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="b5aba-299">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="b5aba-300">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5aba-300">Boolean</span></span>|<span data-ttu-id="b5aba-301">Desabilitar MOBIKE</span><span class="sxs-lookup"><span data-stu-id="b5aba-301">Disable MOBIKE</span></span>|
|<span data-ttu-id="b5aba-302">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="b5aba-302">disableRedirect</span></span>|<span data-ttu-id="b5aba-303">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5aba-303">Boolean</span></span>|<span data-ttu-id="b5aba-304">Desabilitar redirecionamento</span><span class="sxs-lookup"><span data-stu-id="b5aba-304">Disable Redirect</span></span>|
|<span data-ttu-id="b5aba-305">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="b5aba-305">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="b5aba-306">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5aba-306">Boolean</span></span>|<span data-ttu-id="b5aba-307">Habilita uma verificação de revogação de melhor esforço; o tempo limite de resposta do servidor não causará falha</span><span class="sxs-lookup"><span data-stu-id="b5aba-307">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="b5aba-308">enableEAP</span><span class="sxs-lookup"><span data-stu-id="b5aba-308">enableEAP</span></span>|<span data-ttu-id="b5aba-309">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5aba-309">Boolean</span></span>|<span data-ttu-id="b5aba-310">Habilita a autenticação somente EAP</span><span class="sxs-lookup"><span data-stu-id="b5aba-310">Enables EAP only authentication</span></span>|
|<span data-ttu-id="b5aba-311">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="b5aba-311">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="b5aba-312">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5aba-312">Boolean</span></span>|<span data-ttu-id="b5aba-313">Habilitar sigilo total na transferência (PFS).</span><span class="sxs-lookup"><span data-stu-id="b5aba-313">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="b5aba-314">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="b5aba-314">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="b5aba-315">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5aba-315">Boolean</span></span>|<span data-ttu-id="b5aba-316">Habilitar o uso de atributos de sub-rede interna.</span><span class="sxs-lookup"><span data-stu-id="b5aba-316">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="b5aba-317">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="b5aba-317">localIdentifier</span></span>|[<span data-ttu-id="b5aba-318">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="b5aba-318">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="b5aba-319">Método de identificação do cliente que está tentando se conectar via VPN.</span><span class="sxs-lookup"><span data-stu-id="b5aba-319">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="b5aba-320">.</span><span class="sxs-lookup"><span data-stu-id="b5aba-320">.</span></span> <span data-ttu-id="b5aba-321">Os valores possíveis são: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="b5aba-321">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="b5aba-322">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="b5aba-322">remoteIdentifier</span></span>|<span data-ttu-id="b5aba-323">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-323">String</span></span>|<span data-ttu-id="b5aba-324">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="b5aba-324">Address of the IKEv2 server.</span></span> <span data-ttu-id="b5aba-325">Deve ser um FQDN, userfqdn, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="b5aba-325">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="b5aba-326">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="b5aba-326">securityAssociationParameters</span></span>|[<span data-ttu-id="b5aba-327">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="b5aba-327">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="b5aba-328">Parâmetros de associação de segurança</span><span class="sxs-lookup"><span data-stu-id="b5aba-328">Security Association Parameters</span></span>|
|<span data-ttu-id="b5aba-329">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="b5aba-329">serverCertificateCommonName</span></span>|<span data-ttu-id="b5aba-330">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-330">String</span></span>|<span data-ttu-id="b5aba-331">Nome comum do certificado de servidor IKEv2 usado na autenticação de servidor</span><span class="sxs-lookup"><span data-stu-id="b5aba-331">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="b5aba-332">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="b5aba-332">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="b5aba-333">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-333">String</span></span>|<span data-ttu-id="b5aba-334">Nome comum do emissor do emissor do certificado do servidor IKEv2 usado na autenticação</span><span class="sxs-lookup"><span data-stu-id="b5aba-334">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="b5aba-335">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="b5aba-335">serverCertificateType</span></span>|[<span data-ttu-id="b5aba-336">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="b5aba-336">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="b5aba-337">O tipo de certificado que o servidor VPN apresentará ao cliente VPN para autenticação.</span><span class="sxs-lookup"><span data-stu-id="b5aba-337">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="b5aba-338">Os valores possíveis são: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="b5aba-338">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="b5aba-339">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="b5aba-339">sharedSecret</span></span>|<span data-ttu-id="b5aba-340">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-340">String</span></span>|<span data-ttu-id="b5aba-341">Usado quando a autenticação secreta compartilhada está selecionada</span><span class="sxs-lookup"><span data-stu-id="b5aba-341">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="b5aba-342">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b5aba-342">tlsMaximumVersion</span></span>|<span data-ttu-id="b5aba-343">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-343">String</span></span>|<span data-ttu-id="b5aba-344">A versão máxima do TLS a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="b5aba-344">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="b5aba-345">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b5aba-345">tlsMinimumVersion</span></span>|<span data-ttu-id="b5aba-346">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5aba-346">String</span></span>|<span data-ttu-id="b5aba-347">A versão de TLS mínima a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="b5aba-347">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="b5aba-348">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="b5aba-348">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="b5aba-349">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5aba-349">Boolean</span></span>|<span data-ttu-id="b5aba-350">Permite o uso de parâmetros de associação de segurança por meio da configuração de todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="b5aba-350">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="b5aba-351">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="b5aba-351">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="b5aba-352">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5aba-352">Boolean</span></span>|<span data-ttu-id="b5aba-353">Permite o uso de parâmetros de associação de segurança filhos ao definir todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="b5aba-353">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="b5aba-354">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b5aba-354">alwaysOnConfiguration</span></span>|[<span data-ttu-id="b5aba-355">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b5aba-355">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="b5aba-356">Configuração do AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="b5aba-356">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="b5aba-357">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b5aba-357">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="b5aba-358">Booliano</span><span class="sxs-lookup"><span data-stu-id="b5aba-358">Boolean</span></span>|<span data-ttu-id="b5aba-359">Determina se a VPN AlwaysOn está habilitada</span><span class="sxs-lookup"><span data-stu-id="b5aba-359">Determines if Always on VPN is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="b5aba-360">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5aba-360">Response</span></span>
<span data-ttu-id="b5aba-361">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5aba-361">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5aba-362">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5aba-362">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5aba-363">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5aba-363">Request</span></span>
<span data-ttu-id="b5aba-364">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5aba-364">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 5241

{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
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
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
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
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
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
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "clientAuthenticationType": "deviceAuthentication",
  "deadPeerDetectionRate": "none",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "empty",
  "remoteIdentifier": "Remote Identifier value",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "serverCertificateCommonName": "Server Certificate Common Name value",
  "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
  "serverCertificateType": "ecdsa256",
  "sharedSecret": "Shared Secret value",
  "tlsMaximumVersion": "Tls Maximum Version value",
  "tlsMinimumVersion": "Tls Minimum Version value",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true,
  "alwaysOnConfiguration": {
    "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
    "tunnelConfiguration": "cellular",
    "userToggleEnabled": true,
    "voicemailExceptionAction": "allowTrafficOutside",
    "airPrintExceptionAction": "allowTrafficOutside",
    "cellularExceptionAction": "allowTrafficOutside",
    "allowAllCaptiveNetworkPlugins": true,
    "allowedCaptiveNetworkPlugins": {
      "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
      "allowedBundleIdentifiers": [
        "Allowed Bundle Identifiers value"
      ]
    },
    "allowCaptiveWebSheet": true,
    "natKeepAliveIntervalInSeconds": 13,
    "natKeepAliveOffloadEnable": true
  },
  "enableAlwaysOnConfiguration": true
}
```

### <a name="response"></a><span data-ttu-id="b5aba-365">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5aba-365">Response</span></span>
<span data-ttu-id="b5aba-366">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="b5aba-366">Here is an example of the response.</span></span> <span data-ttu-id="b5aba-367">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b5aba-367">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b5aba-368">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b5aba-368">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5413

{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
  "id": "b87b0327-0327-b87b-2703-7bb827037bb8",
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
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
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
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
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
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "clientAuthenticationType": "deviceAuthentication",
  "deadPeerDetectionRate": "none",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "empty",
  "remoteIdentifier": "Remote Identifier value",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "serverCertificateCommonName": "Server Certificate Common Name value",
  "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
  "serverCertificateType": "ecdsa256",
  "sharedSecret": "Shared Secret value",
  "tlsMaximumVersion": "Tls Maximum Version value",
  "tlsMinimumVersion": "Tls Minimum Version value",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true,
  "alwaysOnConfiguration": {
    "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
    "tunnelConfiguration": "cellular",
    "userToggleEnabled": true,
    "voicemailExceptionAction": "allowTrafficOutside",
    "airPrintExceptionAction": "allowTrafficOutside",
    "cellularExceptionAction": "allowTrafficOutside",
    "allowAllCaptiveNetworkPlugins": true,
    "allowedCaptiveNetworkPlugins": {
      "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
      "allowedBundleIdentifiers": [
        "Allowed Bundle Identifiers value"
      ]
    },
    "allowCaptiveWebSheet": true,
    "natKeepAliveIntervalInSeconds": 13,
    "natKeepAliveOffloadEnable": true
  },
  "enableAlwaysOnConfiguration": true
}
```



