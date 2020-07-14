---
title: Atualizar iosVpnConfiguration
description: Atualiza as propriedades de um objeto iosVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3f2f54bc367a4533a084b1c000f3c5572d4415f7
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123033"
---
# <a name="update-iosvpnconfiguration"></a><span data-ttu-id="f92fe-103">Atualizar iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f92fe-103">Update iosVpnConfiguration</span></span>

<span data-ttu-id="f92fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f92fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f92fe-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f92fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f92fe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f92fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f92fe-107">Atualiza as propriedades de um objeto [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f92fe-107">Update the properties of a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f92fe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f92fe-108">Prerequisites</span></span>
<span data-ttu-id="f92fe-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f92fe-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f92fe-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f92fe-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f92fe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f92fe-111">Permission type</span></span>|<span data-ttu-id="f92fe-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f92fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f92fe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f92fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f92fe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f92fe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f92fe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f92fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f92fe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f92fe-116">Not supported.</span></span>|
|<span data-ttu-id="f92fe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f92fe-117">Application</span></span>|<span data-ttu-id="f92fe-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f92fe-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f92fe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f92fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f92fe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f92fe-120">Request headers</span></span>
|<span data-ttu-id="f92fe-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f92fe-121">Header</span></span>|<span data-ttu-id="f92fe-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f92fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f92fe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f92fe-123">Authorization</span></span>|<span data-ttu-id="f92fe-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f92fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f92fe-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f92fe-125">Accept</span></span>|<span data-ttu-id="f92fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f92fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f92fe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f92fe-127">Request body</span></span>
<span data-ttu-id="f92fe-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f92fe-128">In the request body, supply a JSON representation for the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="f92fe-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f92fe-129">The following table shows the properties that are required when you create the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span>

|<span data-ttu-id="f92fe-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f92fe-130">Property</span></span>|<span data-ttu-id="f92fe-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f92fe-131">Type</span></span>|<span data-ttu-id="f92fe-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f92fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f92fe-133">id</span><span class="sxs-lookup"><span data-stu-id="f92fe-133">id</span></span>|<span data-ttu-id="f92fe-134">String</span><span class="sxs-lookup"><span data-stu-id="f92fe-134">String</span></span>|<span data-ttu-id="f92fe-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f92fe-135">Key of the entity.</span></span> <span data-ttu-id="f92fe-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f92fe-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f92fe-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f92fe-138">DateTimeOffset</span></span>|<span data-ttu-id="f92fe-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f92fe-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f92fe-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f92fe-141">roleScopeTagIds</span></span>|<span data-ttu-id="f92fe-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f92fe-142">String collection</span></span>|<span data-ttu-id="f92fe-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f92fe-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f92fe-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f92fe-145">supportsScopeTags</span></span>|<span data-ttu-id="f92fe-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="f92fe-146">Boolean</span></span>|<span data-ttu-id="f92fe-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f92fe-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f92fe-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f92fe-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f92fe-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f92fe-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f92fe-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f92fe-150">This property is read-only.</span></span> <span data-ttu-id="f92fe-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f92fe-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f92fe-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f92fe-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f92fe-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="f92fe-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f92fe-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f92fe-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f92fe-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f92fe-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f92fe-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="f92fe-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f92fe-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f92fe-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f92fe-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f92fe-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f92fe-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="f92fe-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f92fe-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f92fe-164">createdDateTime</span></span>|<span data-ttu-id="f92fe-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f92fe-165">DateTimeOffset</span></span>|<span data-ttu-id="f92fe-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f92fe-166">DateTime the object was created.</span></span> <span data-ttu-id="f92fe-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-168">descrição</span><span class="sxs-lookup"><span data-stu-id="f92fe-168">description</span></span>|<span data-ttu-id="f92fe-169">String</span><span class="sxs-lookup"><span data-stu-id="f92fe-169">String</span></span>|<span data-ttu-id="f92fe-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f92fe-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f92fe-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f92fe-172">displayName</span></span>|<span data-ttu-id="f92fe-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f92fe-173">String</span></span>|<span data-ttu-id="f92fe-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f92fe-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f92fe-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-176">versão</span><span class="sxs-lookup"><span data-stu-id="f92fe-176">version</span></span>|<span data-ttu-id="f92fe-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f92fe-177">Int32</span></span>|<span data-ttu-id="f92fe-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f92fe-178">Version of the device configuration.</span></span> <span data-ttu-id="f92fe-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="f92fe-180">connectionName</span></span>|<span data-ttu-id="f92fe-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f92fe-181">String</span></span>|<span data-ttu-id="f92fe-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="f92fe-182">Connection name displayed to the user.</span></span> <span data-ttu-id="f92fe-183">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-184">Connection</span><span class="sxs-lookup"><span data-stu-id="f92fe-184">connectionType</span></span>|[<span data-ttu-id="f92fe-185">Enumeraçãoapplevpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="f92fe-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="f92fe-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="f92fe-186">Connection type.</span></span> <span data-ttu-id="f92fe-187">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f92fe-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="f92fe-188">Os valores possíveis são:, `ciscoAnyConnect` `pulseSecure` , `f5EdgeClient` , `dellSonicWallMobileConnect` , `checkPointCapsuleVpn` , `customVpn` ,,,,,,,,,,,,,,, `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` , `paloAltoGlobalProtectV2` , `ikEv2` , `alwaysOn` , `microsoftTunnel` .</span><span class="sxs-lookup"><span data-stu-id="f92fe-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`.</span></span>|
|<span data-ttu-id="f92fe-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="f92fe-189">loginGroupOrDomain</span></span>|<span data-ttu-id="f92fe-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f92fe-190">String</span></span>|<span data-ttu-id="f92fe-191">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="f92fe-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="f92fe-192">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-193">role</span><span class="sxs-lookup"><span data-stu-id="f92fe-193">role</span></span>|<span data-ttu-id="f92fe-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f92fe-194">String</span></span>|<span data-ttu-id="f92fe-195">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="f92fe-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f92fe-196">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-197">esfera</span><span class="sxs-lookup"><span data-stu-id="f92fe-197">realm</span></span>|<span data-ttu-id="f92fe-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f92fe-198">String</span></span>|<span data-ttu-id="f92fe-199">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="f92fe-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f92fe-200">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-201">do</span><span class="sxs-lookup"><span data-stu-id="f92fe-201">server</span></span>|[<span data-ttu-id="f92fe-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="f92fe-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="f92fe-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="f92fe-203">VPN Server on the network.</span></span> <span data-ttu-id="f92fe-204">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="f92fe-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="f92fe-205">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-206">identificador</span><span class="sxs-lookup"><span data-stu-id="f92fe-206">identifier</span></span>|<span data-ttu-id="f92fe-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f92fe-207">String</span></span>|<span data-ttu-id="f92fe-208">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="f92fe-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f92fe-209">Por exemplo: o Cisco AnyConnect usa um identificador do formulário com. Cisco. AnyConnect. applevpn. plugin herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-210">customData</span><span class="sxs-lookup"><span data-stu-id="f92fe-210">customData</span></span>|<span data-ttu-id="f92fe-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="f92fe-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="f92fe-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f92fe-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="f92fe-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="f92fe-214">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="f92fe-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="f92fe-215">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="f92fe-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="f92fe-216">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-217">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="f92fe-217">customKeyValueData</span></span>|<span data-ttu-id="f92fe-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f92fe-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="f92fe-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f92fe-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="f92fe-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="f92fe-221">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="f92fe-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="f92fe-222">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="f92fe-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="f92fe-223">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="f92fe-224">enableSplitTunneling</span></span>|<span data-ttu-id="f92fe-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="f92fe-225">Boolean</span></span>|<span data-ttu-id="f92fe-226">Enviar todo o tráfego de rede através da VPN.</span><span class="sxs-lookup"><span data-stu-id="f92fe-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="f92fe-227">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f92fe-228">authenticationMethod</span></span>|[<span data-ttu-id="f92fe-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f92fe-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="f92fe-230">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="f92fe-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="f92fe-231">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f92fe-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="f92fe-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="f92fe-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="f92fe-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="f92fe-233">enablePerApp</span></span>|<span data-ttu-id="f92fe-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="f92fe-234">Boolean</span></span>|<span data-ttu-id="f92fe-235">A configuração dessa opção como true cria uma carga de VPN por aplicativo, que pode ser mais tarde associada aos aplicativos que podem acionar esta conexão VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="f92fe-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="f92fe-236">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="f92fe-237">safariDomains</span></span>|<span data-ttu-id="f92fe-238">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f92fe-238">String collection</span></span>|<span data-ttu-id="f92fe-239">Domínios Safari quando esta configuração VPN por aplicativo estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="f92fe-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="f92fe-240">Além dos aplicativos associados a essa VPN, os domínios Safari especificados aqui também serão capazes de acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="f92fe-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="f92fe-241">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="f92fe-242">onDemandRules</span></span>|<span data-ttu-id="f92fe-243">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="f92fe-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="f92fe-244">On-Demand Rules.</span></span> <span data-ttu-id="f92fe-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f92fe-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f92fe-246">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-247">proxyServer</span><span class="sxs-lookup"><span data-stu-id="f92fe-247">proxyServer</span></span>|[<span data-ttu-id="f92fe-248">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f92fe-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="f92fe-249">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="f92fe-249">Proxy Server.</span></span> <span data-ttu-id="f92fe-250">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-251">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="f92fe-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="f92fe-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="f92fe-252">Boolean</span></span>|<span data-ttu-id="f92fe-253">Optar por compartilhar a ID do dispositivo para clientes VPN de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="f92fe-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="f92fe-254">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f92fe-255">providerType</span><span class="sxs-lookup"><span data-stu-id="f92fe-255">providerType</span></span>|[<span data-ttu-id="f92fe-256">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="f92fe-256">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="f92fe-257">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f92fe-257">Provider type for per-app VPN.</span></span> <span data-ttu-id="f92fe-258">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="f92fe-258">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="f92fe-259">UserDomain</span><span class="sxs-lookup"><span data-stu-id="f92fe-259">userDomain</span></span>|<span data-ttu-id="f92fe-260">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f92fe-260">String</span></span>|<span data-ttu-id="f92fe-261">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="f92fe-261">Zscaler only.</span></span> <span data-ttu-id="f92fe-262">Insira um domínio estático para preencher previamente o campo de logon com no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="f92fe-262">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="f92fe-263">Se for deixado em branco, o domínio do Azure Active Directory do usuário será usado.</span><span class="sxs-lookup"><span data-stu-id="f92fe-263">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="f92fe-264">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="f92fe-264">strictEnforcement</span></span>|<span data-ttu-id="f92fe-265">Booliano</span><span class="sxs-lookup"><span data-stu-id="f92fe-265">Boolean</span></span>|<span data-ttu-id="f92fe-266">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="f92fe-266">Zscaler only.</span></span> <span data-ttu-id="f92fe-267">Bloqueia o tráfego de rede até que o usuário entre no Zscaler app.</span><span class="sxs-lookup"><span data-stu-id="f92fe-267">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="f92fe-268">"True" significa que o tráfego é bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f92fe-268">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="f92fe-269">cloudName</span><span class="sxs-lookup"><span data-stu-id="f92fe-269">cloudName</span></span>|<span data-ttu-id="f92fe-270">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f92fe-270">String</span></span>|<span data-ttu-id="f92fe-271">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="f92fe-271">Zscaler only.</span></span> <span data-ttu-id="f92fe-272">Nuvem do Zscaler à qual o usuário está atribuído.</span><span class="sxs-lookup"><span data-stu-id="f92fe-272">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="f92fe-273">Excludelistpara</span><span class="sxs-lookup"><span data-stu-id="f92fe-273">excludeList</span></span>|<span data-ttu-id="f92fe-274">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f92fe-274">String collection</span></span>|<span data-ttu-id="f92fe-275">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="f92fe-275">Zscaler only.</span></span> <span data-ttu-id="f92fe-276">Lista de endereços de rede que não são enviados pela nuvem do Zscaler.</span><span class="sxs-lookup"><span data-stu-id="f92fe-276">List of network addresses which are not sent through the Zscaler cloud.</span></span>|
|<span data-ttu-id="f92fe-277">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="f92fe-277">targetedMobileApps</span></span>|<span data-ttu-id="f92fe-278">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="f92fe-278">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f92fe-279">Aplicativos móveis direcionados.</span><span class="sxs-lookup"><span data-stu-id="f92fe-279">Targeted mobile apps.</span></span> <span data-ttu-id="f92fe-280">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f92fe-280">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f92fe-281">Resposta</span><span class="sxs-lookup"><span data-stu-id="f92fe-281">Response</span></span>
<span data-ttu-id="f92fe-282">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f92fe-282">If successful, this method returns a `200 OK` response code and an updated [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f92fe-283">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f92fe-283">Example</span></span>

### <a name="request"></a><span data-ttu-id="f92fe-284">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f92fe-284">Request</span></span>
<span data-ttu-id="f92fe-285">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f92fe-285">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3072

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="f92fe-286">Resposta</span><span class="sxs-lookup"><span data-stu-id="f92fe-286">Response</span></span>
<span data-ttu-id="f92fe-287">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="f92fe-287">Here is an example of the response.</span></span> <span data-ttu-id="f92fe-288">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="f92fe-288">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f92fe-289">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="f92fe-289">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3244

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
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
  ]
}
```



