---
title: Atualizar iosikEv2VpnConfiguration
description: Atualiza as propriedades de um objeto iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 460487509d0746f3627e46ccdf4e1668bfe401b8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47995202"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="8ec90-103">Atualizar iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ec90-103">Update iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="8ec90-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ec90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ec90-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8ec90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ec90-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ec90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ec90-107">Atualiza as propriedades de um objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8ec90-107">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ec90-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8ec90-108">Prerequisites</span></span>
<span data-ttu-id="8ec90-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ec90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ec90-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ec90-111">Permission type</span></span>|<span data-ttu-id="8ec90-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8ec90-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ec90-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ec90-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ec90-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ec90-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ec90-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ec90-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ec90-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ec90-116">Not supported.</span></span>|
|<span data-ttu-id="8ec90-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ec90-117">Application</span></span>|<span data-ttu-id="8ec90-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ec90-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ec90-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ec90-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8ec90-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ec90-120">Request headers</span></span>
|<span data-ttu-id="8ec90-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8ec90-121">Header</span></span>|<span data-ttu-id="8ec90-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8ec90-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ec90-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ec90-123">Authorization</span></span>|<span data-ttu-id="8ec90-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ec90-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ec90-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8ec90-125">Accept</span></span>|<span data-ttu-id="8ec90-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ec90-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ec90-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ec90-127">Request body</span></span>
<span data-ttu-id="8ec90-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8ec90-128">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="8ec90-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ec90-129">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="8ec90-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ec90-130">Property</span></span>|<span data-ttu-id="8ec90-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ec90-131">Type</span></span>|<span data-ttu-id="8ec90-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ec90-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ec90-133">id</span><span class="sxs-lookup"><span data-stu-id="8ec90-133">id</span></span>|<span data-ttu-id="8ec90-134">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-134">String</span></span>|<span data-ttu-id="8ec90-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8ec90-135">Key of the entity.</span></span> <span data-ttu-id="8ec90-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ec90-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8ec90-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ec90-138">DateTimeOffset</span></span>|<span data-ttu-id="8ec90-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8ec90-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8ec90-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8ec90-141">roleScopeTagIds</span></span>|<span data-ttu-id="8ec90-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ec90-142">String collection</span></span>|<span data-ttu-id="8ec90-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="8ec90-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8ec90-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8ec90-145">supportsScopeTags</span></span>|<span data-ttu-id="8ec90-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec90-146">Boolean</span></span>|<span data-ttu-id="8ec90-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="8ec90-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8ec90-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="8ec90-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8ec90-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="8ec90-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8ec90-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8ec90-150">This property is read-only.</span></span> <span data-ttu-id="8ec90-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8ec90-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8ec90-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8ec90-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8ec90-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="8ec90-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8ec90-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8ec90-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8ec90-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8ec90-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8ec90-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="8ec90-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8ec90-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8ec90-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8ec90-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8ec90-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8ec90-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="8ec90-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8ec90-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ec90-164">createdDateTime</span></span>|<span data-ttu-id="8ec90-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ec90-165">DateTimeOffset</span></span>|<span data-ttu-id="8ec90-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8ec90-166">DateTime the object was created.</span></span> <span data-ttu-id="8ec90-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-168">description</span><span class="sxs-lookup"><span data-stu-id="8ec90-168">description</span></span>|<span data-ttu-id="8ec90-169">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-169">String</span></span>|<span data-ttu-id="8ec90-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8ec90-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8ec90-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-172">displayName</span><span class="sxs-lookup"><span data-stu-id="8ec90-172">displayName</span></span>|<span data-ttu-id="8ec90-173">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-173">String</span></span>|<span data-ttu-id="8ec90-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8ec90-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8ec90-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-176">versão</span><span class="sxs-lookup"><span data-stu-id="8ec90-176">version</span></span>|<span data-ttu-id="8ec90-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8ec90-177">Int32</span></span>|<span data-ttu-id="8ec90-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8ec90-178">Version of the device configuration.</span></span> <span data-ttu-id="8ec90-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="8ec90-180">connectionName</span></span>|<span data-ttu-id="8ec90-181">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-181">String</span></span>|<span data-ttu-id="8ec90-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="8ec90-182">Connection name displayed to the user.</span></span> <span data-ttu-id="8ec90-183">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-184">Connection</span><span class="sxs-lookup"><span data-stu-id="8ec90-184">connectionType</span></span>|[<span data-ttu-id="8ec90-185">Enumeraçãoapplevpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="8ec90-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="8ec90-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="8ec90-186">Connection type.</span></span> <span data-ttu-id="8ec90-187">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ec90-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="8ec90-188">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,,,,, `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` , `alwaysOn` , `microsoftTunnel` , `netMotionMobility` .</span><span class="sxs-lookup"><span data-stu-id="8ec90-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="8ec90-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="8ec90-189">loginGroupOrDomain</span></span>|<span data-ttu-id="8ec90-190">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-190">String</span></span>|<span data-ttu-id="8ec90-191">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="8ec90-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="8ec90-192">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-193">role</span><span class="sxs-lookup"><span data-stu-id="8ec90-193">role</span></span>|<span data-ttu-id="8ec90-194">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-194">String</span></span>|<span data-ttu-id="8ec90-195">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="8ec90-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="8ec90-196">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-197">esfera</span><span class="sxs-lookup"><span data-stu-id="8ec90-197">realm</span></span>|<span data-ttu-id="8ec90-198">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-198">String</span></span>|<span data-ttu-id="8ec90-199">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="8ec90-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="8ec90-200">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-201">do</span><span class="sxs-lookup"><span data-stu-id="8ec90-201">server</span></span>|[<span data-ttu-id="8ec90-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="8ec90-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="8ec90-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="8ec90-203">VPN Server on the network.</span></span> <span data-ttu-id="8ec90-204">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="8ec90-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="8ec90-205">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-206">identificador</span><span class="sxs-lookup"><span data-stu-id="8ec90-206">identifier</span></span>|<span data-ttu-id="8ec90-207">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-207">String</span></span>|<span data-ttu-id="8ec90-208">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="8ec90-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="8ec90-209">Por exemplo: o Cisco AnyConnect usa um identificador do formulário com. Cisco. AnyConnect. applevpn. plugin herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-210">customData</span><span class="sxs-lookup"><span data-stu-id="8ec90-210">customData</span></span>|<span data-ttu-id="8ec90-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="8ec90-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="8ec90-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="8ec90-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="8ec90-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="8ec90-214">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="8ec90-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="8ec90-215">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="8ec90-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="8ec90-216">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-217">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="8ec90-217">customKeyValueData</span></span>|<span data-ttu-id="8ec90-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="8ec90-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="8ec90-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="8ec90-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="8ec90-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="8ec90-221">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="8ec90-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="8ec90-222">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="8ec90-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="8ec90-223">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="8ec90-224">enableSplitTunneling</span></span>|<span data-ttu-id="8ec90-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec90-225">Boolean</span></span>|<span data-ttu-id="8ec90-226">Enviar todo o tráfego de rede através da VPN.</span><span class="sxs-lookup"><span data-stu-id="8ec90-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="8ec90-227">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8ec90-228">authenticationMethod</span></span>|[<span data-ttu-id="8ec90-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8ec90-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="8ec90-230">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="8ec90-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="8ec90-231">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ec90-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="8ec90-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="8ec90-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="8ec90-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="8ec90-233">enablePerApp</span></span>|<span data-ttu-id="8ec90-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec90-234">Boolean</span></span>|<span data-ttu-id="8ec90-235">A configuração dessa opção como true cria uma carga de VPN por aplicativo, que pode ser mais tarde associada aos aplicativos que podem acionar esta conexão VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="8ec90-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="8ec90-236">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="8ec90-237">safariDomains</span></span>|<span data-ttu-id="8ec90-238">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ec90-238">String collection</span></span>|<span data-ttu-id="8ec90-239">Domínios Safari quando esta configuração VPN por aplicativo estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="8ec90-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="8ec90-240">Além dos aplicativos associados a essa VPN, os domínios Safari especificados aqui também serão capazes de acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="8ec90-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="8ec90-241">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="8ec90-242">onDemandRules</span></span>|<span data-ttu-id="8ec90-243">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="8ec90-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="8ec90-244">On-Demand Rules.</span></span> <span data-ttu-id="8ec90-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="8ec90-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="8ec90-246">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-247">providerType</span><span class="sxs-lookup"><span data-stu-id="8ec90-247">providerType</span></span>|[<span data-ttu-id="8ec90-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="8ec90-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="8ec90-249">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8ec90-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="8ec90-250">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ec90-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="8ec90-251">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="8ec90-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="8ec90-252">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="8ec90-252">excludedDomains</span></span>|<span data-ttu-id="8ec90-253">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ec90-253">String collection</span></span>|<span data-ttu-id="8ec90-254">Domínios que são acessados por meio da Internet pública em vez de via VPN, mesmo quando a VPN por aplicativo é ativada herdada de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-254">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-255">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="8ec90-255">disableOnDemandUserOverride</span></span>|<span data-ttu-id="8ec90-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec90-256">Boolean</span></span>|<span data-ttu-id="8ec90-257">Alternar para impedir que o usuário desabilite a VPN automática no aplicativo de configurações herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-257">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-258">proxyServer</span><span class="sxs-lookup"><span data-stu-id="8ec90-258">proxyServer</span></span>|[<span data-ttu-id="8ec90-259">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="8ec90-259">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="8ec90-260">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="8ec90-260">Proxy Server.</span></span> <span data-ttu-id="8ec90-261">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-261">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-262">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="8ec90-262">optInToDeviceIdSharing</span></span>|<span data-ttu-id="8ec90-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec90-263">Boolean</span></span>|<span data-ttu-id="8ec90-264">Optar por compartilhar a ID do dispositivo para clientes VPN de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="8ec90-264">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="8ec90-265">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-265">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-266">UserDomain</span><span class="sxs-lookup"><span data-stu-id="8ec90-266">userDomain</span></span>|<span data-ttu-id="8ec90-267">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-267">String</span></span>|<span data-ttu-id="8ec90-268">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="8ec90-268">Zscaler only.</span></span> <span data-ttu-id="8ec90-269">Insira um domínio estático para preencher previamente o campo de logon com no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="8ec90-269">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="8ec90-270">Se for deixado em branco, o domínio do Azure Active Directory do usuário será usado.</span><span class="sxs-lookup"><span data-stu-id="8ec90-270">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="8ec90-271">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-272">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="8ec90-272">strictEnforcement</span></span>|<span data-ttu-id="8ec90-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec90-273">Boolean</span></span>|<span data-ttu-id="8ec90-274">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="8ec90-274">Zscaler only.</span></span> <span data-ttu-id="8ec90-275">Bloqueia o tráfego de rede até que o usuário entre no Zscaler app.</span><span class="sxs-lookup"><span data-stu-id="8ec90-275">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="8ec90-276">"True" significa que o tráfego é bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8ec90-276">"True" means traffic is blocked.</span></span> <span data-ttu-id="8ec90-277">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-277">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-278">cloudName</span><span class="sxs-lookup"><span data-stu-id="8ec90-278">cloudName</span></span>|<span data-ttu-id="8ec90-279">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-279">String</span></span>|<span data-ttu-id="8ec90-280">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="8ec90-280">Zscaler only.</span></span> <span data-ttu-id="8ec90-281">Nuvem do Zscaler à qual o usuário está atribuído.</span><span class="sxs-lookup"><span data-stu-id="8ec90-281">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="8ec90-282">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-282">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-283">Excludelistpara</span><span class="sxs-lookup"><span data-stu-id="8ec90-283">excludeList</span></span>|<span data-ttu-id="8ec90-284">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ec90-284">String collection</span></span>|<span data-ttu-id="8ec90-285">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="8ec90-285">Zscaler only.</span></span> <span data-ttu-id="8ec90-286">Lista de endereços de rede que não são enviados pela nuvem do Zscaler.</span><span class="sxs-lookup"><span data-stu-id="8ec90-286">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="8ec90-287">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-287">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-288">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="8ec90-288">targetedMobileApps</span></span>|<span data-ttu-id="8ec90-289">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-289">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8ec90-290">Aplicativos móveis direcionados.</span><span class="sxs-lookup"><span data-stu-id="8ec90-290">Targeted mobile apps.</span></span> <span data-ttu-id="8ec90-291">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="8ec90-291">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="8ec90-292">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-292">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-293">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="8ec90-293">microsoftTunnelSiteId</span></span>|<span data-ttu-id="8ec90-294">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-294">String</span></span>|<span data-ttu-id="8ec90-295">ID de site de túnel da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8ec90-295">Microsoft Tunnel site ID.</span></span> <span data-ttu-id="8ec90-296">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8ec90-296">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="8ec90-297">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="8ec90-297">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="8ec90-298">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="8ec90-298">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="8ec90-299">Parâmetros da Associação de segurança filho</span><span class="sxs-lookup"><span data-stu-id="8ec90-299">Child Security Association Parameters</span></span>|
|<span data-ttu-id="8ec90-300">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="8ec90-300">clientAuthenticationType</span></span>|[<span data-ttu-id="8ec90-301">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="8ec90-301">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="8ec90-302">Tipo de autenticação de cliente que o cliente VPN usará.</span><span class="sxs-lookup"><span data-stu-id="8ec90-302">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="8ec90-303">Os valores possíveis são: `userAuthentication` e `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="8ec90-303">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="8ec90-304">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="8ec90-304">deadPeerDetectionRate</span></span>|[<span data-ttu-id="8ec90-305">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="8ec90-305">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="8ec90-306">Determinar a frequência de verificação de uma conexão de mesmo nível.</span><span class="sxs-lookup"><span data-stu-id="8ec90-306">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="8ec90-307">.</span><span class="sxs-lookup"><span data-stu-id="8ec90-307">.</span></span> <span data-ttu-id="8ec90-308">Os valores possíveis são: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="8ec90-308">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="8ec90-309">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="8ec90-309">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="8ec90-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec90-310">Boolean</span></span>|<span data-ttu-id="8ec90-311">Desabilitar MOBIKE</span><span class="sxs-lookup"><span data-stu-id="8ec90-311">Disable MOBIKE</span></span>|
|<span data-ttu-id="8ec90-312">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="8ec90-312">disableRedirect</span></span>|<span data-ttu-id="8ec90-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec90-313">Boolean</span></span>|<span data-ttu-id="8ec90-314">Desabilitar redirecionamento</span><span class="sxs-lookup"><span data-stu-id="8ec90-314">Disable Redirect</span></span>|
|<span data-ttu-id="8ec90-315">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="8ec90-315">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="8ec90-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec90-316">Boolean</span></span>|<span data-ttu-id="8ec90-317">Habilita uma verificação de revogação de melhor esforço; o tempo limite de resposta do servidor não causará falha</span><span class="sxs-lookup"><span data-stu-id="8ec90-317">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="8ec90-318">enableEAP</span><span class="sxs-lookup"><span data-stu-id="8ec90-318">enableEAP</span></span>|<span data-ttu-id="8ec90-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec90-319">Boolean</span></span>|<span data-ttu-id="8ec90-320">Habilita a autenticação somente EAP</span><span class="sxs-lookup"><span data-stu-id="8ec90-320">Enables EAP only authentication</span></span>|
|<span data-ttu-id="8ec90-321">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="8ec90-321">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="8ec90-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec90-322">Boolean</span></span>|<span data-ttu-id="8ec90-323">Habilitar sigilo total na transferência (PFS).</span><span class="sxs-lookup"><span data-stu-id="8ec90-323">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="8ec90-324">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="8ec90-324">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="8ec90-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec90-325">Boolean</span></span>|<span data-ttu-id="8ec90-326">Habilitar o uso de atributos de sub-rede interna.</span><span class="sxs-lookup"><span data-stu-id="8ec90-326">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="8ec90-327">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="8ec90-327">localIdentifier</span></span>|[<span data-ttu-id="8ec90-328">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="8ec90-328">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="8ec90-329">Método de identificação do cliente que está tentando se conectar via VPN.</span><span class="sxs-lookup"><span data-stu-id="8ec90-329">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="8ec90-330">.</span><span class="sxs-lookup"><span data-stu-id="8ec90-330">.</span></span> <span data-ttu-id="8ec90-331">Os valores possíveis são: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="8ec90-331">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="8ec90-332">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="8ec90-332">remoteIdentifier</span></span>|<span data-ttu-id="8ec90-333">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-333">String</span></span>|<span data-ttu-id="8ec90-334">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="8ec90-334">Address of the IKEv2 server.</span></span> <span data-ttu-id="8ec90-335">Deve ser um FQDN, userfqdn, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="8ec90-335">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="8ec90-336">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="8ec90-336">securityAssociationParameters</span></span>|[<span data-ttu-id="8ec90-337">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="8ec90-337">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="8ec90-338">Parâmetros de associação de segurança</span><span class="sxs-lookup"><span data-stu-id="8ec90-338">Security Association Parameters</span></span>|
|<span data-ttu-id="8ec90-339">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="8ec90-339">serverCertificateCommonName</span></span>|<span data-ttu-id="8ec90-340">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-340">String</span></span>|<span data-ttu-id="8ec90-341">Nome comum do certificado de servidor IKEv2 usado na autenticação de servidor</span><span class="sxs-lookup"><span data-stu-id="8ec90-341">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="8ec90-342">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="8ec90-342">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="8ec90-343">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-343">String</span></span>|<span data-ttu-id="8ec90-344">Nome comum do emissor do emissor do certificado do servidor IKEv2 usado na autenticação</span><span class="sxs-lookup"><span data-stu-id="8ec90-344">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="8ec90-345">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="8ec90-345">serverCertificateType</span></span>|[<span data-ttu-id="8ec90-346">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="8ec90-346">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="8ec90-347">O tipo de certificado que o servidor VPN apresentará ao cliente VPN para autenticação.</span><span class="sxs-lookup"><span data-stu-id="8ec90-347">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="8ec90-348">Os valores possíveis são: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="8ec90-348">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="8ec90-349">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="8ec90-349">sharedSecret</span></span>|<span data-ttu-id="8ec90-350">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-350">String</span></span>|<span data-ttu-id="8ec90-351">Usado quando a autenticação secreta compartilhada está selecionada</span><span class="sxs-lookup"><span data-stu-id="8ec90-351">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="8ec90-352">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="8ec90-352">tlsMaximumVersion</span></span>|<span data-ttu-id="8ec90-353">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-353">String</span></span>|<span data-ttu-id="8ec90-354">A versão máxima do TLS a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="8ec90-354">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="8ec90-355">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="8ec90-355">tlsMinimumVersion</span></span>|<span data-ttu-id="8ec90-356">String</span><span class="sxs-lookup"><span data-stu-id="8ec90-356">String</span></span>|<span data-ttu-id="8ec90-357">A versão de TLS mínima a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="8ec90-357">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="8ec90-358">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="8ec90-358">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="8ec90-359">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec90-359">Boolean</span></span>|<span data-ttu-id="8ec90-360">Permite o uso de parâmetros de associação de segurança por meio da configuração de todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="8ec90-360">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="8ec90-361">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="8ec90-361">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="8ec90-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec90-362">Boolean</span></span>|<span data-ttu-id="8ec90-363">Permite o uso de parâmetros de associação de segurança filhos ao definir todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="8ec90-363">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="8ec90-364">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ec90-364">alwaysOnConfiguration</span></span>|[<span data-ttu-id="8ec90-365">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ec90-365">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="8ec90-366">Configuração do AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="8ec90-366">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="8ec90-367">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ec90-367">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="8ec90-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ec90-368">Boolean</span></span>|<span data-ttu-id="8ec90-369">Determina se a VPN AlwaysOn está habilitada</span><span class="sxs-lookup"><span data-stu-id="8ec90-369">Determines if Always on VPN is enabled</span></span>|
|<span data-ttu-id="8ec90-370">mtuSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="8ec90-370">mtuSizeInBytes</span></span>|<span data-ttu-id="8ec90-371">Int32</span><span class="sxs-lookup"><span data-stu-id="8ec90-371">Int32</span></span>|<span data-ttu-id="8ec90-372">Unidade de transmissão máxima.</span><span class="sxs-lookup"><span data-stu-id="8ec90-372">Maximum transmission unit.</span></span> <span data-ttu-id="8ec90-373">Valores válidos de 1 a 65536</span><span class="sxs-lookup"><span data-stu-id="8ec90-373">Valid values 1 to 65536</span></span>|



## <a name="response"></a><span data-ttu-id="8ec90-374">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ec90-374">Response</span></span>
<span data-ttu-id="8ec90-375">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ec90-375">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ec90-376">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ec90-376">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ec90-377">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ec90-377">Request</span></span>
<span data-ttu-id="8ec90-378">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ec90-378">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 5428

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
  "providerType": "appProxy",
  "excludedDomains": [
    "Excluded Domains value"
  ],
  "disableOnDemandUserOverride": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value",
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
  "enableAlwaysOnConfiguration": true,
  "mtuSizeInBytes": 14
}
```

### <a name="response"></a><span data-ttu-id="8ec90-379">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ec90-379">Response</span></span>
<span data-ttu-id="8ec90-p142">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ec90-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5600

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
  "providerType": "appProxy",
  "excludedDomains": [
    "Excluded Domains value"
  ],
  "disableOnDemandUserOverride": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value",
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
  "enableAlwaysOnConfiguration": true,
  "mtuSizeInBytes": 14
}
```






