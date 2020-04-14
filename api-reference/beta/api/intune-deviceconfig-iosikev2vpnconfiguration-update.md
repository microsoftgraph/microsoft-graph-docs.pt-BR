---
title: Atualizar iosikEv2VpnConfiguration
description: Atualiza as propriedades de um objeto iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 70099b8e64ba6076b1e63610df5ee58a5b7aa3f2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43438909"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="f8920-103">Atualizar iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8920-103">Update iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="f8920-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8920-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8920-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8920-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8920-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8920-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8920-107">Atualiza as propriedades de um objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f8920-107">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8920-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8920-108">Prerequisites</span></span>
<span data-ttu-id="f8920-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8920-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8920-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8920-111">Permission type</span></span>|<span data-ttu-id="f8920-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8920-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8920-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8920-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8920-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8920-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8920-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8920-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8920-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8920-116">Not supported.</span></span>|
|<span data-ttu-id="f8920-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8920-117">Application</span></span>|<span data-ttu-id="f8920-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8920-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8920-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8920-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f8920-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8920-120">Request headers</span></span>
|<span data-ttu-id="f8920-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8920-121">Header</span></span>|<span data-ttu-id="f8920-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f8920-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8920-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8920-123">Authorization</span></span>|<span data-ttu-id="f8920-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8920-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8920-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f8920-125">Accept</span></span>|<span data-ttu-id="f8920-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8920-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8920-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8920-127">Request body</span></span>
<span data-ttu-id="f8920-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f8920-128">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="f8920-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8920-129">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="f8920-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8920-130">Property</span></span>|<span data-ttu-id="f8920-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8920-131">Type</span></span>|<span data-ttu-id="f8920-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8920-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8920-133">id</span><span class="sxs-lookup"><span data-stu-id="f8920-133">id</span></span>|<span data-ttu-id="f8920-134">String</span><span class="sxs-lookup"><span data-stu-id="f8920-134">String</span></span>|<span data-ttu-id="f8920-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f8920-135">Key of the entity.</span></span> <span data-ttu-id="f8920-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8920-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f8920-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8920-138">DateTimeOffset</span></span>|<span data-ttu-id="f8920-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f8920-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f8920-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f8920-141">roleScopeTagIds</span></span>|<span data-ttu-id="f8920-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f8920-142">String collection</span></span>|<span data-ttu-id="f8920-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f8920-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f8920-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f8920-145">supportsScopeTags</span></span>|<span data-ttu-id="f8920-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8920-146">Boolean</span></span>|<span data-ttu-id="f8920-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f8920-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f8920-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f8920-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f8920-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f8920-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f8920-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f8920-150">This property is read-only.</span></span> <span data-ttu-id="f8920-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f8920-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f8920-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f8920-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f8920-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="f8920-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f8920-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f8920-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f8920-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f8920-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f8920-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="f8920-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f8920-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f8920-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f8920-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f8920-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f8920-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="f8920-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f8920-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8920-164">createdDateTime</span></span>|<span data-ttu-id="f8920-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8920-165">DateTimeOffset</span></span>|<span data-ttu-id="f8920-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f8920-166">DateTime the object was created.</span></span> <span data-ttu-id="f8920-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-168">description</span><span class="sxs-lookup"><span data-stu-id="f8920-168">description</span></span>|<span data-ttu-id="f8920-169">String</span><span class="sxs-lookup"><span data-stu-id="f8920-169">String</span></span>|<span data-ttu-id="f8920-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8920-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f8920-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f8920-172">displayName</span></span>|<span data-ttu-id="f8920-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8920-173">String</span></span>|<span data-ttu-id="f8920-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8920-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f8920-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-176">versão</span><span class="sxs-lookup"><span data-stu-id="f8920-176">version</span></span>|<span data-ttu-id="f8920-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f8920-177">Int32</span></span>|<span data-ttu-id="f8920-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8920-178">Version of the device configuration.</span></span> <span data-ttu-id="f8920-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="f8920-180">connectionName</span></span>|<span data-ttu-id="f8920-181">String</span><span class="sxs-lookup"><span data-stu-id="f8920-181">String</span></span>|<span data-ttu-id="f8920-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="f8920-182">Connection name displayed to the user.</span></span> <span data-ttu-id="f8920-183">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-184">Connection</span><span class="sxs-lookup"><span data-stu-id="f8920-184">connectionType</span></span>|[<span data-ttu-id="f8920-185">Enumeraçãoapplevpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="f8920-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="f8920-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="f8920-186">Connection type.</span></span> <span data-ttu-id="f8920-187">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8920-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="f8920-188">Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span><span class="sxs-lookup"><span data-stu-id="f8920-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span></span>|
|<span data-ttu-id="f8920-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="f8920-189">loginGroupOrDomain</span></span>|<span data-ttu-id="f8920-190">String</span><span class="sxs-lookup"><span data-stu-id="f8920-190">String</span></span>|<span data-ttu-id="f8920-191">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="f8920-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="f8920-192">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-193">role</span><span class="sxs-lookup"><span data-stu-id="f8920-193">role</span></span>|<span data-ttu-id="f8920-194">String</span><span class="sxs-lookup"><span data-stu-id="f8920-194">String</span></span>|<span data-ttu-id="f8920-195">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="f8920-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f8920-196">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-197">esfera</span><span class="sxs-lookup"><span data-stu-id="f8920-197">realm</span></span>|<span data-ttu-id="f8920-198">String</span><span class="sxs-lookup"><span data-stu-id="f8920-198">String</span></span>|<span data-ttu-id="f8920-199">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="f8920-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="f8920-200">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-201">do</span><span class="sxs-lookup"><span data-stu-id="f8920-201">server</span></span>|[<span data-ttu-id="f8920-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="f8920-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="f8920-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="f8920-203">VPN Server on the network.</span></span> <span data-ttu-id="f8920-204">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="f8920-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="f8920-205">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-206">identificador</span><span class="sxs-lookup"><span data-stu-id="f8920-206">identifier</span></span>|<span data-ttu-id="f8920-207">String</span><span class="sxs-lookup"><span data-stu-id="f8920-207">String</span></span>|<span data-ttu-id="f8920-208">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="f8920-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f8920-209">Por exemplo: o Cisco AnyConnect usa um identificador do formulário com. Cisco. AnyConnect. applevpn. plugin herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-210">customData</span><span class="sxs-lookup"><span data-stu-id="f8920-210">customData</span></span>|<span data-ttu-id="f8920-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="f8920-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="f8920-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f8920-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="f8920-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="f8920-214">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="f8920-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="f8920-215">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="f8920-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="f8920-216">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-217">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="f8920-217">customKeyValueData</span></span>|<span data-ttu-id="f8920-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f8920-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="f8920-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="f8920-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="f8920-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="f8920-221">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="f8920-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="f8920-222">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="f8920-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="f8920-223">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="f8920-224">enableSplitTunneling</span></span>|<span data-ttu-id="f8920-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8920-225">Boolean</span></span>|<span data-ttu-id="f8920-226">Enviar todo o tráfego de rede através da VPN.</span><span class="sxs-lookup"><span data-stu-id="f8920-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="f8920-227">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f8920-228">authenticationMethod</span></span>|[<span data-ttu-id="f8920-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f8920-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="f8920-230">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="f8920-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="f8920-231">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8920-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="f8920-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="f8920-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="f8920-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="f8920-233">enablePerApp</span></span>|<span data-ttu-id="f8920-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8920-234">Boolean</span></span>|<span data-ttu-id="f8920-235">A configuração dessa opção como true cria uma carga de VPN por aplicativo, que pode ser mais tarde associada aos aplicativos que podem acionar esta conexão VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="f8920-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="f8920-236">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="f8920-237">safariDomains</span></span>|<span data-ttu-id="f8920-238">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f8920-238">String collection</span></span>|<span data-ttu-id="f8920-239">Domínios Safari quando esta configuração VPN por aplicativo estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="f8920-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="f8920-240">Além dos aplicativos associados a essa VPN, os domínios Safari especificados aqui também serão capazes de acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="f8920-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="f8920-241">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="f8920-242">onDemandRules</span></span>|<span data-ttu-id="f8920-243">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="f8920-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="f8920-244">On-Demand Rules.</span></span> <span data-ttu-id="f8920-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f8920-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f8920-246">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-247">proxyServer</span><span class="sxs-lookup"><span data-stu-id="f8920-247">proxyServer</span></span>|[<span data-ttu-id="f8920-248">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="f8920-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="f8920-249">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="f8920-249">Proxy Server.</span></span> <span data-ttu-id="f8920-250">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-251">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="f8920-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="f8920-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8920-252">Boolean</span></span>|<span data-ttu-id="f8920-253">Optar por compartilhar a ID do dispositivo para clientes VPN de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="f8920-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="f8920-254">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-255">providerType</span><span class="sxs-lookup"><span data-stu-id="f8920-255">providerType</span></span>|[<span data-ttu-id="f8920-256">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="f8920-256">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="f8920-257">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f8920-257">Provider type for per-app VPN.</span></span> <span data-ttu-id="f8920-258">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f8920-258">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="f8920-259">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="f8920-259">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="f8920-260">UserDomain</span><span class="sxs-lookup"><span data-stu-id="f8920-260">userDomain</span></span>|<span data-ttu-id="f8920-261">String</span><span class="sxs-lookup"><span data-stu-id="f8920-261">String</span></span>|<span data-ttu-id="f8920-262">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="f8920-262">Zscaler only.</span></span> <span data-ttu-id="f8920-263">Insira um domínio estático para preencher previamente o campo de logon com no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="f8920-263">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="f8920-264">Se for deixado em branco, o domínio do Azure Active Directory do usuário será usado.</span><span class="sxs-lookup"><span data-stu-id="f8920-264">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="f8920-265">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-265">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-266">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="f8920-266">strictEnforcement</span></span>|<span data-ttu-id="f8920-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8920-267">Boolean</span></span>|<span data-ttu-id="f8920-268">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="f8920-268">Zscaler only.</span></span> <span data-ttu-id="f8920-269">Bloqueia o tráfego de rede até que o usuário entre no Zscaler app.</span><span class="sxs-lookup"><span data-stu-id="f8920-269">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="f8920-270">"True" significa que o tráfego é bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f8920-270">"True" means traffic is blocked.</span></span> <span data-ttu-id="f8920-271">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-272">cloudName</span><span class="sxs-lookup"><span data-stu-id="f8920-272">cloudName</span></span>|<span data-ttu-id="f8920-273">String</span><span class="sxs-lookup"><span data-stu-id="f8920-273">String</span></span>|<span data-ttu-id="f8920-274">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="f8920-274">Zscaler only.</span></span> <span data-ttu-id="f8920-275">Nuvem do Zscaler à qual o usuário está atribuído.</span><span class="sxs-lookup"><span data-stu-id="f8920-275">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="f8920-276">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-276">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-277">Excludelistpara</span><span class="sxs-lookup"><span data-stu-id="f8920-277">excludeList</span></span>|<span data-ttu-id="f8920-278">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f8920-278">String collection</span></span>|<span data-ttu-id="f8920-279">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="f8920-279">Zscaler only.</span></span> <span data-ttu-id="f8920-280">Lista de endereços de rede que não são enviados pela nuvem do Zscaler.</span><span class="sxs-lookup"><span data-stu-id="f8920-280">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="f8920-281">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f8920-281">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="f8920-282">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f8920-282">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="f8920-283">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f8920-283">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="f8920-284">Parâmetros da Associação de segurança filho</span><span class="sxs-lookup"><span data-stu-id="f8920-284">Child Security Association Parameters</span></span>|
|<span data-ttu-id="f8920-285">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="f8920-285">clientAuthenticationType</span></span>|[<span data-ttu-id="f8920-286">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="f8920-286">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="f8920-287">Tipo de autenticação de cliente que o cliente VPN usará.</span><span class="sxs-lookup"><span data-stu-id="f8920-287">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="f8920-288">Os valores possíveis são: `userAuthentication` e `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="f8920-288">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="f8920-289">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="f8920-289">deadPeerDetectionRate</span></span>|[<span data-ttu-id="f8920-290">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="f8920-290">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="f8920-291">Determinar a frequência de verificação de uma conexão de mesmo nível.</span><span class="sxs-lookup"><span data-stu-id="f8920-291">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="f8920-292">.</span><span class="sxs-lookup"><span data-stu-id="f8920-292">.</span></span> <span data-ttu-id="f8920-293">Os valores possíveis são: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="f8920-293">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="f8920-294">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="f8920-294">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="f8920-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8920-295">Boolean</span></span>|<span data-ttu-id="f8920-296">Desabilitar MOBIKE</span><span class="sxs-lookup"><span data-stu-id="f8920-296">Disable MOBIKE</span></span>|
|<span data-ttu-id="f8920-297">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="f8920-297">disableRedirect</span></span>|<span data-ttu-id="f8920-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8920-298">Boolean</span></span>|<span data-ttu-id="f8920-299">Desabilitar redirecionamento</span><span class="sxs-lookup"><span data-stu-id="f8920-299">Disable Redirect</span></span>|
|<span data-ttu-id="f8920-300">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="f8920-300">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="f8920-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8920-301">Boolean</span></span>|<span data-ttu-id="f8920-302">Habilita uma verificação de revogação de melhor esforço; o tempo limite de resposta do servidor não causará falha</span><span class="sxs-lookup"><span data-stu-id="f8920-302">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="f8920-303">enableEAP</span><span class="sxs-lookup"><span data-stu-id="f8920-303">enableEAP</span></span>|<span data-ttu-id="f8920-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8920-304">Boolean</span></span>|<span data-ttu-id="f8920-305">Habilita a autenticação somente EAP</span><span class="sxs-lookup"><span data-stu-id="f8920-305">Enables EAP only authentication</span></span>|
|<span data-ttu-id="f8920-306">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="f8920-306">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="f8920-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8920-307">Boolean</span></span>|<span data-ttu-id="f8920-308">Habilitar sigilo total na transferência (PFS).</span><span class="sxs-lookup"><span data-stu-id="f8920-308">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="f8920-309">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="f8920-309">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="f8920-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8920-310">Boolean</span></span>|<span data-ttu-id="f8920-311">Habilitar o uso de atributos de sub-rede interna.</span><span class="sxs-lookup"><span data-stu-id="f8920-311">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="f8920-312">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="f8920-312">localIdentifier</span></span>|[<span data-ttu-id="f8920-313">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="f8920-313">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="f8920-314">Método de identificação do cliente que está tentando se conectar via VPN.</span><span class="sxs-lookup"><span data-stu-id="f8920-314">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="f8920-315">.</span><span class="sxs-lookup"><span data-stu-id="f8920-315">.</span></span> <span data-ttu-id="f8920-316">Os valores possíveis são: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="f8920-316">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="f8920-317">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="f8920-317">remoteIdentifier</span></span>|<span data-ttu-id="f8920-318">String</span><span class="sxs-lookup"><span data-stu-id="f8920-318">String</span></span>|<span data-ttu-id="f8920-319">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="f8920-319">Address of the IKEv2 server.</span></span> <span data-ttu-id="f8920-320">Deve ser um FQDN, userfqdn, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="f8920-320">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="f8920-321">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f8920-321">securityAssociationParameters</span></span>|[<span data-ttu-id="f8920-322">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f8920-322">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="f8920-323">Parâmetros de associação de segurança</span><span class="sxs-lookup"><span data-stu-id="f8920-323">Security Association Parameters</span></span>|
|<span data-ttu-id="f8920-324">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="f8920-324">serverCertificateCommonName</span></span>|<span data-ttu-id="f8920-325">String</span><span class="sxs-lookup"><span data-stu-id="f8920-325">String</span></span>|<span data-ttu-id="f8920-326">Nome comum do certificado de servidor IKEv2 usado na autenticação de servidor</span><span class="sxs-lookup"><span data-stu-id="f8920-326">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="f8920-327">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="f8920-327">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="f8920-328">String</span><span class="sxs-lookup"><span data-stu-id="f8920-328">String</span></span>|<span data-ttu-id="f8920-329">Nome comum do emissor do emissor do certificado do servidor IKEv2 usado na autenticação</span><span class="sxs-lookup"><span data-stu-id="f8920-329">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="f8920-330">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="f8920-330">serverCertificateType</span></span>|[<span data-ttu-id="f8920-331">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="f8920-331">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="f8920-332">O tipo de certificado que o servidor VPN apresentará ao cliente VPN para autenticação.</span><span class="sxs-lookup"><span data-stu-id="f8920-332">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="f8920-333">Os valores possíveis são: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="f8920-333">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="f8920-334">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="f8920-334">sharedSecret</span></span>|<span data-ttu-id="f8920-335">String</span><span class="sxs-lookup"><span data-stu-id="f8920-335">String</span></span>|<span data-ttu-id="f8920-336">Usado quando a autenticação secreta compartilhada está selecionada</span><span class="sxs-lookup"><span data-stu-id="f8920-336">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="f8920-337">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="f8920-337">tlsMaximumVersion</span></span>|<span data-ttu-id="f8920-338">String</span><span class="sxs-lookup"><span data-stu-id="f8920-338">String</span></span>|<span data-ttu-id="f8920-339">A versão máxima do TLS a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="f8920-339">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="f8920-340">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="f8920-340">tlsMinimumVersion</span></span>|<span data-ttu-id="f8920-341">String</span><span class="sxs-lookup"><span data-stu-id="f8920-341">String</span></span>|<span data-ttu-id="f8920-342">A versão de TLS mínima a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="f8920-342">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="f8920-343">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f8920-343">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="f8920-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8920-344">Boolean</span></span>|<span data-ttu-id="f8920-345">Permite o uso de parâmetros de associação de segurança por meio da configuração de todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="f8920-345">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="f8920-346">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="f8920-346">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="f8920-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8920-347">Boolean</span></span>|<span data-ttu-id="f8920-348">Permite o uso de parâmetros de associação de segurança filhos ao definir todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="f8920-348">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="f8920-349">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8920-349">alwaysOnConfiguration</span></span>|[<span data-ttu-id="f8920-350">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8920-350">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="f8920-351">Configuração do AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="f8920-351">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="f8920-352">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8920-352">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="f8920-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8920-353">Boolean</span></span>|<span data-ttu-id="f8920-354">Determina se a VPN AlwaysOn está habilitada</span><span class="sxs-lookup"><span data-stu-id="f8920-354">Determines if Always on VPN is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="f8920-355">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8920-355">Response</span></span>
<span data-ttu-id="f8920-356">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8920-356">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8920-357">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8920-357">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8920-358">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8920-358">Request</span></span>
<span data-ttu-id="f8920-359">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8920-359">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4984

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

### <a name="response"></a><span data-ttu-id="f8920-360">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8920-360">Response</span></span>
<span data-ttu-id="f8920-p139">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8920-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5156

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



