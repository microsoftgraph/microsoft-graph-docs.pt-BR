---
title: Atualizar iosikEv2VpnConfiguration
description: Atualiza as propriedades de um objeto iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b077d66fb8951f08c62da61d98ea3b7022dc629
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733836"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="2ca2e-103">Atualizar iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ca2e-103">Update iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="2ca2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ca2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ca2e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ca2e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ca2e-107">Atualiza as propriedades de um objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2ca2e-107">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ca2e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2ca2e-108">Prerequisites</span></span>
<span data-ttu-id="2ca2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ca2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ca2e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ca2e-111">Permission type</span></span>|<span data-ttu-id="2ca2e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ca2e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ca2e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ca2e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2ca2e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ca2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-116">Not supported.</span></span>|
|<span data-ttu-id="2ca2e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ca2e-117">Application</span></span>|<span data-ttu-id="2ca2e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ca2e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ca2e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ca2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2ca2e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ca2e-120">Request headers</span></span>
|<span data-ttu-id="2ca2e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ca2e-121">Header</span></span>|<span data-ttu-id="2ca2e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2ca2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ca2e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ca2e-123">Authorization</span></span>|<span data-ttu-id="2ca2e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ca2e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ca2e-125">Accept</span></span>|<span data-ttu-id="2ca2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ca2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ca2e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ca2e-127">Request body</span></span>
<span data-ttu-id="2ca2e-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2ca2e-128">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="2ca2e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2ca2e-129">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="2ca2e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ca2e-130">Property</span></span>|<span data-ttu-id="2ca2e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ca2e-131">Type</span></span>|<span data-ttu-id="2ca2e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ca2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ca2e-133">id</span><span class="sxs-lookup"><span data-stu-id="2ca2e-133">id</span></span>|<span data-ttu-id="2ca2e-134">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-134">String</span></span>|<span data-ttu-id="2ca2e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-135">Key of the entity.</span></span> <span data-ttu-id="2ca2e-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ca2e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2ca2e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ca2e-138">DateTimeOffset</span></span>|<span data-ttu-id="2ca2e-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2ca2e-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2ca2e-141">roleScopeTagIds</span></span>|<span data-ttu-id="2ca2e-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ca2e-142">String collection</span></span>|<span data-ttu-id="2ca2e-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2ca2e-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2ca2e-145">supportsScopeTags</span></span>|<span data-ttu-id="2ca2e-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ca2e-146">Boolean</span></span>|<span data-ttu-id="2ca2e-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2ca2e-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2ca2e-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2ca2e-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-150">This property is read-only.</span></span> <span data-ttu-id="2ca2e-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2ca2e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2ca2e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2ca2e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2ca2e-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2ca2e-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2ca2e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2ca2e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2ca2e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2ca2e-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2ca2e-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2ca2e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2ca2e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2ca2e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2ca2e-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2ca2e-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ca2e-164">createdDateTime</span></span>|<span data-ttu-id="2ca2e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ca2e-165">DateTimeOffset</span></span>|<span data-ttu-id="2ca2e-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-166">DateTime the object was created.</span></span> <span data-ttu-id="2ca2e-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-168">description</span><span class="sxs-lookup"><span data-stu-id="2ca2e-168">description</span></span>|<span data-ttu-id="2ca2e-169">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-169">String</span></span>|<span data-ttu-id="2ca2e-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2ca2e-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="2ca2e-172">displayName</span></span>|<span data-ttu-id="2ca2e-173">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-173">String</span></span>|<span data-ttu-id="2ca2e-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2ca2e-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-176">versão</span><span class="sxs-lookup"><span data-stu-id="2ca2e-176">version</span></span>|<span data-ttu-id="2ca2e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2ca2e-177">Int32</span></span>|<span data-ttu-id="2ca2e-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-178">Version of the device configuration.</span></span> <span data-ttu-id="2ca2e-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="2ca2e-180">connectionName</span></span>|<span data-ttu-id="2ca2e-181">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-181">String</span></span>|<span data-ttu-id="2ca2e-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-182">Connection name displayed to the user.</span></span> <span data-ttu-id="2ca2e-183">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-184">Connection</span><span class="sxs-lookup"><span data-stu-id="2ca2e-184">connectionType</span></span>|[<span data-ttu-id="2ca2e-185">Enumeraçãoapplevpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="2ca2e-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="2ca2e-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-186">Connection type.</span></span> <span data-ttu-id="2ca2e-187">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2ca2e-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="2ca2e-188">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,,,,, `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` , `alwaysOn` , `microsoftTunnel` , `netMotionMobility` .</span><span class="sxs-lookup"><span data-stu-id="2ca2e-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="2ca2e-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="2ca2e-189">loginGroupOrDomain</span></span>|<span data-ttu-id="2ca2e-190">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-190">String</span></span>|<span data-ttu-id="2ca2e-191">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="2ca2e-192">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-193">role</span><span class="sxs-lookup"><span data-stu-id="2ca2e-193">role</span></span>|<span data-ttu-id="2ca2e-194">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-194">String</span></span>|<span data-ttu-id="2ca2e-195">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="2ca2e-196">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-197">esfera</span><span class="sxs-lookup"><span data-stu-id="2ca2e-197">realm</span></span>|<span data-ttu-id="2ca2e-198">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-198">String</span></span>|<span data-ttu-id="2ca2e-199">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="2ca2e-200">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-201">do</span><span class="sxs-lookup"><span data-stu-id="2ca2e-201">server</span></span>|[<span data-ttu-id="2ca2e-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="2ca2e-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="2ca2e-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-203">VPN Server on the network.</span></span> <span data-ttu-id="2ca2e-204">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="2ca2e-205">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-206">identificador</span><span class="sxs-lookup"><span data-stu-id="2ca2e-206">identifier</span></span>|<span data-ttu-id="2ca2e-207">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-207">String</span></span>|<span data-ttu-id="2ca2e-208">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2ca2e-209">Por exemplo: o Cisco AnyConnect usa um identificador do formulário com. Cisco. AnyConnect. applevpn. plugin herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-210">customData</span><span class="sxs-lookup"><span data-stu-id="2ca2e-210">customData</span></span>|<span data-ttu-id="2ca2e-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="2ca2e-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2ca2e-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="2ca2e-214">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="2ca2e-215">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="2ca2e-216">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-217">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="2ca2e-217">customKeyValueData</span></span>|<span data-ttu-id="2ca2e-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="2ca2e-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2ca2e-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="2ca2e-221">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="2ca2e-222">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="2ca2e-223">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="2ca2e-224">enableSplitTunneling</span></span>|<span data-ttu-id="2ca2e-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ca2e-225">Boolean</span></span>|<span data-ttu-id="2ca2e-226">Enviar todo o tráfego de rede através da VPN.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="2ca2e-227">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2ca2e-228">authenticationMethod</span></span>|[<span data-ttu-id="2ca2e-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2ca2e-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="2ca2e-230">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="2ca2e-231">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2ca2e-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="2ca2e-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="2ca2e-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="2ca2e-233">enablePerApp</span></span>|<span data-ttu-id="2ca2e-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ca2e-234">Boolean</span></span>|<span data-ttu-id="2ca2e-235">Definir isso como true cria Per-App carga de VPN que pode ser associada posteriormente a aplicativos que podem acionar esta VPN conexão no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="2ca2e-236">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="2ca2e-237">safariDomains</span></span>|<span data-ttu-id="2ca2e-238">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ca2e-238">String collection</span></span>|<span data-ttu-id="2ca2e-239">Domínios Safari quando esta configuração VPN por aplicativo estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="2ca2e-240">Além dos aplicativos associados a essa VPN, os domínios Safari especificados aqui também serão capazes de acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="2ca2e-241">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="2ca2e-242">onDemandRules</span></span>|<span data-ttu-id="2ca2e-243">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="2ca2e-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-244">On-Demand Rules.</span></span> <span data-ttu-id="2ca2e-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="2ca2e-246">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-247">providerType</span><span class="sxs-lookup"><span data-stu-id="2ca2e-247">providerType</span></span>|[<span data-ttu-id="2ca2e-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="2ca2e-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="2ca2e-249">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="2ca2e-250">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2ca2e-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="2ca2e-251">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="2ca2e-252">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="2ca2e-252">excludedDomains</span></span>|<span data-ttu-id="2ca2e-253">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ca2e-253">String collection</span></span>|<span data-ttu-id="2ca2e-254">Domínios que são acessados por meio da Internet pública em vez de via VPN, mesmo quando a VPN por aplicativo é ativada herdada de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-254">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-255">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="2ca2e-255">disableOnDemandUserOverride</span></span>|<span data-ttu-id="2ca2e-256">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ca2e-256">Boolean</span></span>|<span data-ttu-id="2ca2e-257">Alternar para impedir que o usuário desabilite a VPN automática no aplicativo de configurações herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-257">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-258">proxyServer</span><span class="sxs-lookup"><span data-stu-id="2ca2e-258">proxyServer</span></span>|[<span data-ttu-id="2ca2e-259">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="2ca2e-259">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="2ca2e-260">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-260">Proxy Server.</span></span> <span data-ttu-id="2ca2e-261">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-261">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-262">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="2ca2e-262">optInToDeviceIdSharing</span></span>|<span data-ttu-id="2ca2e-263">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ca2e-263">Boolean</span></span>|<span data-ttu-id="2ca2e-264">Opt-In compartilhar a ID do dispositivo para clientes VPN de terceiros para uso durante a validação do controle de acesso de rede.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-264">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="2ca2e-265">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-265">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-266">UserDomain</span><span class="sxs-lookup"><span data-stu-id="2ca2e-266">userDomain</span></span>|<span data-ttu-id="2ca2e-267">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-267">String</span></span>|<span data-ttu-id="2ca2e-268">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-268">Zscaler only.</span></span> <span data-ttu-id="2ca2e-269">Insira um domínio estático para preencher previamente o campo de logon com no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-269">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="2ca2e-270">Se for deixado em branco, o domínio do Azure Active Directory do usuário será usado.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-270">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="2ca2e-271">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-272">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="2ca2e-272">strictEnforcement</span></span>|<span data-ttu-id="2ca2e-273">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ca2e-273">Boolean</span></span>|<span data-ttu-id="2ca2e-274">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-274">Zscaler only.</span></span> <span data-ttu-id="2ca2e-275">Bloqueia o tráfego de rede até que o usuário entre no Zscaler app.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-275">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="2ca2e-276">"True" significa que o tráfego é bloqueado.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-276">"True" means traffic is blocked.</span></span> <span data-ttu-id="2ca2e-277">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-277">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-278">cloudName</span><span class="sxs-lookup"><span data-stu-id="2ca2e-278">cloudName</span></span>|<span data-ttu-id="2ca2e-279">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-279">String</span></span>|<span data-ttu-id="2ca2e-280">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-280">Zscaler only.</span></span> <span data-ttu-id="2ca2e-281">Nuvem do Zscaler à qual o usuário está atribuído.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-281">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="2ca2e-282">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-282">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-283">Excludelistpara</span><span class="sxs-lookup"><span data-stu-id="2ca2e-283">excludeList</span></span>|<span data-ttu-id="2ca2e-284">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ca2e-284">String collection</span></span>|<span data-ttu-id="2ca2e-285">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-285">Zscaler only.</span></span> <span data-ttu-id="2ca2e-286">Lista de endereços de rede que não são enviados pela nuvem do Zscaler.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-286">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="2ca2e-287">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-287">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-288">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="2ca2e-288">targetedMobileApps</span></span>|<span data-ttu-id="2ca2e-289">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-289">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="2ca2e-290">Aplicativos móveis direcionados.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-290">Targeted mobile apps.</span></span> <span data-ttu-id="2ca2e-291">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-291">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="2ca2e-292">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-292">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-293">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="2ca2e-293">microsoftTunnelSiteId</span></span>|<span data-ttu-id="2ca2e-294">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-294">String</span></span>|<span data-ttu-id="2ca2e-295">ID de site de túnel da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-295">Microsoft Tunnel site ID.</span></span> <span data-ttu-id="2ca2e-296">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2ca2e-296">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="2ca2e-297">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="2ca2e-297">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="2ca2e-298">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="2ca2e-298">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="2ca2e-299">Parâmetros da Associação de segurança filho</span><span class="sxs-lookup"><span data-stu-id="2ca2e-299">Child Security Association Parameters</span></span>|
|<span data-ttu-id="2ca2e-300">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="2ca2e-300">clientAuthenticationType</span></span>|[<span data-ttu-id="2ca2e-301">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="2ca2e-301">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="2ca2e-302">Tipo de autenticação de cliente que o cliente VPN usará.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-302">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="2ca2e-303">Os valores possíveis são: `userAuthentication` e `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-303">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="2ca2e-304">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="2ca2e-304">deadPeerDetectionRate</span></span>|[<span data-ttu-id="2ca2e-305">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="2ca2e-305">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="2ca2e-306">Determinar a frequência de verificação de uma conexão de mesmo nível.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-306">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="2ca2e-307">.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-307">.</span></span> <span data-ttu-id="2ca2e-308">Os valores possíveis são: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-308">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="2ca2e-309">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="2ca2e-309">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="2ca2e-310">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ca2e-310">Boolean</span></span>|<span data-ttu-id="2ca2e-311">Desabilitar MOBIKE</span><span class="sxs-lookup"><span data-stu-id="2ca2e-311">Disable MOBIKE</span></span>|
|<span data-ttu-id="2ca2e-312">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="2ca2e-312">disableRedirect</span></span>|<span data-ttu-id="2ca2e-313">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ca2e-313">Boolean</span></span>|<span data-ttu-id="2ca2e-314">Desabilitar redirecionamento</span><span class="sxs-lookup"><span data-stu-id="2ca2e-314">Disable Redirect</span></span>|
|<span data-ttu-id="2ca2e-315">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="2ca2e-315">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="2ca2e-316">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ca2e-316">Boolean</span></span>|<span data-ttu-id="2ca2e-317">Habilita uma verificação de revogação de melhor esforço; o tempo limite de resposta do servidor não causará falha</span><span class="sxs-lookup"><span data-stu-id="2ca2e-317">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="2ca2e-318">enableEAP</span><span class="sxs-lookup"><span data-stu-id="2ca2e-318">enableEAP</span></span>|<span data-ttu-id="2ca2e-319">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ca2e-319">Boolean</span></span>|<span data-ttu-id="2ca2e-320">Habilita a autenticação somente EAP</span><span class="sxs-lookup"><span data-stu-id="2ca2e-320">Enables EAP only authentication</span></span>|
|<span data-ttu-id="2ca2e-321">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="2ca2e-321">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="2ca2e-322">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ca2e-322">Boolean</span></span>|<span data-ttu-id="2ca2e-323">Habilitar sigilo total na transferência (PFS).</span><span class="sxs-lookup"><span data-stu-id="2ca2e-323">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="2ca2e-324">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="2ca2e-324">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="2ca2e-325">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ca2e-325">Boolean</span></span>|<span data-ttu-id="2ca2e-326">Habilitar o uso de atributos de sub-rede interna.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-326">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="2ca2e-327">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="2ca2e-327">localIdentifier</span></span>|[<span data-ttu-id="2ca2e-328">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="2ca2e-328">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="2ca2e-329">Método de identificação do cliente que está tentando se conectar via VPN.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-329">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="2ca2e-330">.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-330">.</span></span> <span data-ttu-id="2ca2e-331">Os valores possíveis são: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-331">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="2ca2e-332">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="2ca2e-332">remoteIdentifier</span></span>|<span data-ttu-id="2ca2e-333">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-333">String</span></span>|<span data-ttu-id="2ca2e-334">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-334">Address of the IKEv2 server.</span></span> <span data-ttu-id="2ca2e-335">Deve ser um FQDN, userfqdn, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="2ca2e-335">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="2ca2e-336">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="2ca2e-336">securityAssociationParameters</span></span>|[<span data-ttu-id="2ca2e-337">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="2ca2e-337">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="2ca2e-338">Parâmetros de associação de segurança</span><span class="sxs-lookup"><span data-stu-id="2ca2e-338">Security Association Parameters</span></span>|
|<span data-ttu-id="2ca2e-339">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="2ca2e-339">serverCertificateCommonName</span></span>|<span data-ttu-id="2ca2e-340">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-340">String</span></span>|<span data-ttu-id="2ca2e-341">Nome comum do certificado de servidor IKEv2 usado na autenticação de servidor</span><span class="sxs-lookup"><span data-stu-id="2ca2e-341">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="2ca2e-342">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="2ca2e-342">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="2ca2e-343">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-343">String</span></span>|<span data-ttu-id="2ca2e-344">Nome comum do emissor do emissor do certificado do servidor IKEv2 usado na autenticação</span><span class="sxs-lookup"><span data-stu-id="2ca2e-344">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="2ca2e-345">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="2ca2e-345">serverCertificateType</span></span>|[<span data-ttu-id="2ca2e-346">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="2ca2e-346">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="2ca2e-347">O tipo de certificado que o servidor VPN apresentará ao cliente VPN para autenticação.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-347">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="2ca2e-348">Os valores possíveis são: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-348">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="2ca2e-349">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="2ca2e-349">sharedSecret</span></span>|<span data-ttu-id="2ca2e-350">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-350">String</span></span>|<span data-ttu-id="2ca2e-351">Usado quando a autenticação secreta compartilhada está selecionada</span><span class="sxs-lookup"><span data-stu-id="2ca2e-351">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="2ca2e-352">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="2ca2e-352">tlsMaximumVersion</span></span>|<span data-ttu-id="2ca2e-353">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-353">String</span></span>|<span data-ttu-id="2ca2e-354">A versão máxima do TLS a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="2ca2e-354">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="2ca2e-355">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="2ca2e-355">tlsMinimumVersion</span></span>|<span data-ttu-id="2ca2e-356">String</span><span class="sxs-lookup"><span data-stu-id="2ca2e-356">String</span></span>|<span data-ttu-id="2ca2e-357">A versão de TLS mínima a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="2ca2e-357">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="2ca2e-358">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="2ca2e-358">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="2ca2e-359">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ca2e-359">Boolean</span></span>|<span data-ttu-id="2ca2e-360">Permite o uso de parâmetros de associação de segurança por meio da configuração de todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-360">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="2ca2e-361">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="2ca2e-361">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="2ca2e-362">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ca2e-362">Boolean</span></span>|<span data-ttu-id="2ca2e-363">Permite o uso de parâmetros de associação de segurança filhos ao definir todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-363">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="2ca2e-364">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ca2e-364">alwaysOnConfiguration</span></span>|[<span data-ttu-id="2ca2e-365">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ca2e-365">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="2ca2e-366">Configuração do AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="2ca2e-366">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="2ca2e-367">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ca2e-367">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="2ca2e-368">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ca2e-368">Boolean</span></span>|<span data-ttu-id="2ca2e-369">Determina se a VPN AlwaysOn está habilitada</span><span class="sxs-lookup"><span data-stu-id="2ca2e-369">Determines if Always on VPN is enabled</span></span>|
|<span data-ttu-id="2ca2e-370">mtuSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="2ca2e-370">mtuSizeInBytes</span></span>|<span data-ttu-id="2ca2e-371">Int32</span><span class="sxs-lookup"><span data-stu-id="2ca2e-371">Int32</span></span>|<span data-ttu-id="2ca2e-372">Unidade de transmissão máxima.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-372">Maximum transmission unit.</span></span> <span data-ttu-id="2ca2e-373">Valores válidos de 1 a 65536</span><span class="sxs-lookup"><span data-stu-id="2ca2e-373">Valid values 1 to 65536</span></span>|



## <a name="response"></a><span data-ttu-id="2ca2e-374">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ca2e-374">Response</span></span>
<span data-ttu-id="2ca2e-375">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-375">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ca2e-376">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ca2e-376">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ca2e-377">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ca2e-377">Request</span></span>
<span data-ttu-id="2ca2e-378">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-378">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2ca2e-379">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ca2e-379">Response</span></span>
<span data-ttu-id="2ca2e-p142">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ca2e-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





