---
title: Criar iosikEv2VpnConfiguration
description: Criar um novo objeto iosikEv2VpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f2b406ab5cf9b4720b2e9eb108463c6f84ecb315
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41635913"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="545ee-103">Criar iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="545ee-103">Create iosikEv2VpnConfiguration</span></span>

> <span data-ttu-id="545ee-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="545ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="545ee-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="545ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="545ee-106">Criar um novo objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="545ee-106">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="545ee-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="545ee-107">Prerequisites</span></span>
<span data-ttu-id="545ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="545ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="545ee-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="545ee-110">Permission type</span></span>|<span data-ttu-id="545ee-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="545ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="545ee-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="545ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="545ee-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="545ee-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="545ee-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="545ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="545ee-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="545ee-115">Not supported.</span></span>|
|<span data-ttu-id="545ee-116">Application</span><span class="sxs-lookup"><span data-stu-id="545ee-116">Application</span></span>|<span data-ttu-id="545ee-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="545ee-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="545ee-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="545ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="545ee-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="545ee-119">Request headers</span></span>
|<span data-ttu-id="545ee-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="545ee-120">Header</span></span>|<span data-ttu-id="545ee-121">Valor</span><span class="sxs-lookup"><span data-stu-id="545ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="545ee-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="545ee-122">Authorization</span></span>|<span data-ttu-id="545ee-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="545ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="545ee-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="545ee-124">Accept</span></span>|<span data-ttu-id="545ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="545ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="545ee-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="545ee-126">Request body</span></span>
<span data-ttu-id="545ee-127">No corpo da solicitação, forneça uma representação JSON do objeto iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="545ee-127">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="545ee-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="545ee-128">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="545ee-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="545ee-129">Property</span></span>|<span data-ttu-id="545ee-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="545ee-130">Type</span></span>|<span data-ttu-id="545ee-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="545ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="545ee-132">id</span><span class="sxs-lookup"><span data-stu-id="545ee-132">id</span></span>|<span data-ttu-id="545ee-133">String</span><span class="sxs-lookup"><span data-stu-id="545ee-133">String</span></span>|<span data-ttu-id="545ee-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="545ee-134">Key of the entity.</span></span> <span data-ttu-id="545ee-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="545ee-136">lastModifiedDateTime</span></span>|<span data-ttu-id="545ee-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="545ee-137">DateTimeOffset</span></span>|<span data-ttu-id="545ee-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="545ee-138">DateTime the object was last modified.</span></span> <span data-ttu-id="545ee-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="545ee-140">roleScopeTagIds</span></span>|<span data-ttu-id="545ee-141">String collection</span><span class="sxs-lookup"><span data-stu-id="545ee-141">String collection</span></span>|<span data-ttu-id="545ee-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="545ee-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="545ee-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="545ee-144">supportsScopeTags</span></span>|<span data-ttu-id="545ee-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="545ee-145">Boolean</span></span>|<span data-ttu-id="545ee-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="545ee-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="545ee-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="545ee-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="545ee-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="545ee-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="545ee-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="545ee-149">This property is read-only.</span></span> <span data-ttu-id="545ee-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="545ee-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="545ee-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="545ee-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="545ee-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="545ee-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="545ee-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="545ee-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="545ee-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="545ee-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="545ee-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="545ee-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="545ee-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="545ee-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="545ee-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="545ee-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="545ee-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="545ee-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="545ee-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="545ee-163">createdDateTime</span></span>|<span data-ttu-id="545ee-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="545ee-164">DateTimeOffset</span></span>|<span data-ttu-id="545ee-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="545ee-165">DateTime the object was created.</span></span> <span data-ttu-id="545ee-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-167">description</span><span class="sxs-lookup"><span data-stu-id="545ee-167">description</span></span>|<span data-ttu-id="545ee-168">String</span><span class="sxs-lookup"><span data-stu-id="545ee-168">String</span></span>|<span data-ttu-id="545ee-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="545ee-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="545ee-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-171">displayName</span><span class="sxs-lookup"><span data-stu-id="545ee-171">displayName</span></span>|<span data-ttu-id="545ee-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="545ee-172">String</span></span>|<span data-ttu-id="545ee-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="545ee-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="545ee-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-175">versão</span><span class="sxs-lookup"><span data-stu-id="545ee-175">version</span></span>|<span data-ttu-id="545ee-176">Int32</span><span class="sxs-lookup"><span data-stu-id="545ee-176">Int32</span></span>|<span data-ttu-id="545ee-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="545ee-177">Version of the device configuration.</span></span> <span data-ttu-id="545ee-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-179">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="545ee-179">connectionName</span></span>|<span data-ttu-id="545ee-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="545ee-180">String</span></span>|<span data-ttu-id="545ee-181">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="545ee-181">Connection name displayed to the user.</span></span> <span data-ttu-id="545ee-182">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-183">Connection</span><span class="sxs-lookup"><span data-stu-id="545ee-183">connectionType</span></span>|[<span data-ttu-id="545ee-184">Enumeraçãoapplevpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="545ee-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="545ee-185">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="545ee-185">Connection type.</span></span> <span data-ttu-id="545ee-186">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="545ee-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="545ee-187">Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span><span class="sxs-lookup"><span data-stu-id="545ee-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span></span>|
|<span data-ttu-id="545ee-188">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="545ee-188">loginGroupOrDomain</span></span>|<span data-ttu-id="545ee-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="545ee-189">String</span></span>|<span data-ttu-id="545ee-190">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="545ee-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="545ee-191">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-192">role</span><span class="sxs-lookup"><span data-stu-id="545ee-192">role</span></span>|<span data-ttu-id="545ee-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="545ee-193">String</span></span>|<span data-ttu-id="545ee-194">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="545ee-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="545ee-195">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-196">esfera</span><span class="sxs-lookup"><span data-stu-id="545ee-196">realm</span></span>|<span data-ttu-id="545ee-197">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="545ee-197">String</span></span>|<span data-ttu-id="545ee-198">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="545ee-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="545ee-199">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-200">do</span><span class="sxs-lookup"><span data-stu-id="545ee-200">server</span></span>|[<span data-ttu-id="545ee-201">vpnServer</span><span class="sxs-lookup"><span data-stu-id="545ee-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="545ee-202">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="545ee-202">VPN Server on the network.</span></span> <span data-ttu-id="545ee-203">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="545ee-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="545ee-204">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-205">identificador</span><span class="sxs-lookup"><span data-stu-id="545ee-205">identifier</span></span>|<span data-ttu-id="545ee-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="545ee-206">String</span></span>|<span data-ttu-id="545ee-207">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="545ee-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="545ee-208">Por exemplo: o Cisco AnyConnect usa um identificador do formulário com. Cisco. AnyConnect. applevpn. plugin herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-209">customData</span><span class="sxs-lookup"><span data-stu-id="545ee-209">customData</span></span>|<span data-ttu-id="545ee-210">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="545ee-211">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="545ee-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="545ee-212">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="545ee-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="545ee-213">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="545ee-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="545ee-214">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="545ee-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="545ee-215">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-216">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="545ee-216">customKeyValueData</span></span>|<span data-ttu-id="545ee-217">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="545ee-218">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="545ee-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="545ee-219">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="545ee-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="545ee-220">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="545ee-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="545ee-221">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="545ee-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="545ee-222">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-223">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="545ee-223">enableSplitTunneling</span></span>|<span data-ttu-id="545ee-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="545ee-224">Boolean</span></span>|<span data-ttu-id="545ee-225">Enviar todo o tráfego de rede através da VPN.</span><span class="sxs-lookup"><span data-stu-id="545ee-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="545ee-226">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-227">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="545ee-227">authenticationMethod</span></span>|[<span data-ttu-id="545ee-228">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="545ee-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="545ee-229">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="545ee-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="545ee-230">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="545ee-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="545ee-231">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="545ee-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="545ee-232">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="545ee-232">enablePerApp</span></span>|<span data-ttu-id="545ee-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="545ee-233">Boolean</span></span>|<span data-ttu-id="545ee-234">A configuração dessa opção como true cria uma carga de VPN por aplicativo, que pode ser mais tarde associada aos aplicativos que podem acionar esta conexão VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="545ee-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="545ee-235">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-236">safariDomains</span><span class="sxs-lookup"><span data-stu-id="545ee-236">safariDomains</span></span>|<span data-ttu-id="545ee-237">String collection</span><span class="sxs-lookup"><span data-stu-id="545ee-237">String collection</span></span>|<span data-ttu-id="545ee-238">Domínios Safari quando esta configuração VPN por aplicativo estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="545ee-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="545ee-239">Além dos aplicativos associados a essa VPN, os domínios Safari especificados aqui também serão capazes de acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="545ee-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="545ee-240">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-241">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="545ee-241">onDemandRules</span></span>|<span data-ttu-id="545ee-242">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="545ee-243">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="545ee-243">On-Demand Rules.</span></span> <span data-ttu-id="545ee-244">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="545ee-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="545ee-245">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-246">proxyServer</span><span class="sxs-lookup"><span data-stu-id="545ee-246">proxyServer</span></span>|[<span data-ttu-id="545ee-247">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="545ee-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="545ee-248">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="545ee-248">Proxy Server.</span></span> <span data-ttu-id="545ee-249">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-250">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="545ee-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="545ee-251">Booliano</span><span class="sxs-lookup"><span data-stu-id="545ee-251">Boolean</span></span>|<span data-ttu-id="545ee-252">Optar por compartilhar a ID do dispositivo para clientes VPN de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="545ee-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="545ee-253">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-254">providerType</span><span class="sxs-lookup"><span data-stu-id="545ee-254">providerType</span></span>|[<span data-ttu-id="545ee-255">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="545ee-255">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="545ee-256">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="545ee-256">Provider type for per-app VPN.</span></span> <span data-ttu-id="545ee-257">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="545ee-257">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="545ee-258">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="545ee-258">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="545ee-259">UserDomain</span><span class="sxs-lookup"><span data-stu-id="545ee-259">userDomain</span></span>|<span data-ttu-id="545ee-260">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="545ee-260">String</span></span>|<span data-ttu-id="545ee-261">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="545ee-261">Zscaler only.</span></span> <span data-ttu-id="545ee-262">Insira um domínio estático para preencher previamente o campo de logon com no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="545ee-262">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="545ee-263">Se for deixado em branco, o domínio do Azure Active Directory do usuário será usado.</span><span class="sxs-lookup"><span data-stu-id="545ee-263">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="545ee-264">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-264">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-265">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="545ee-265">strictEnforcement</span></span>|<span data-ttu-id="545ee-266">Booliano</span><span class="sxs-lookup"><span data-stu-id="545ee-266">Boolean</span></span>|<span data-ttu-id="545ee-267">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="545ee-267">Zscaler only.</span></span> <span data-ttu-id="545ee-268">Bloqueia o tráfego de rede até que o usuário entre no Zscaler app.</span><span class="sxs-lookup"><span data-stu-id="545ee-268">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="545ee-269">"True" significa que o tráfego é bloqueado.</span><span class="sxs-lookup"><span data-stu-id="545ee-269">"True" means traffic is blocked.</span></span> <span data-ttu-id="545ee-270">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-270">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-271">cloudName</span><span class="sxs-lookup"><span data-stu-id="545ee-271">cloudName</span></span>|<span data-ttu-id="545ee-272">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="545ee-272">String</span></span>|<span data-ttu-id="545ee-273">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="545ee-273">Zscaler only.</span></span> <span data-ttu-id="545ee-274">Nuvem do Zscaler à qual o usuário está atribuído.</span><span class="sxs-lookup"><span data-stu-id="545ee-274">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="545ee-275">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-275">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-276">Excludelistpara</span><span class="sxs-lookup"><span data-stu-id="545ee-276">excludeList</span></span>|<span data-ttu-id="545ee-277">String collection</span><span class="sxs-lookup"><span data-stu-id="545ee-277">String collection</span></span>|<span data-ttu-id="545ee-278">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="545ee-278">Zscaler only.</span></span> <span data-ttu-id="545ee-279">Lista de endereços de rede que não são enviados pela nuvem do Zscaler.</span><span class="sxs-lookup"><span data-stu-id="545ee-279">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="545ee-280">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="545ee-280">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="545ee-281">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="545ee-281">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="545ee-282">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="545ee-282">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="545ee-283">Parâmetros da Associação de segurança filho</span><span class="sxs-lookup"><span data-stu-id="545ee-283">Child Security Association Parameters</span></span>|
|<span data-ttu-id="545ee-284">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="545ee-284">clientAuthenticationType</span></span>|[<span data-ttu-id="545ee-285">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="545ee-285">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="545ee-286">Tipo de autenticação de cliente que o cliente VPN usará.</span><span class="sxs-lookup"><span data-stu-id="545ee-286">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="545ee-287">Os valores possíveis são: `userAuthentication` e `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="545ee-287">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="545ee-288">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="545ee-288">deadPeerDetectionRate</span></span>|[<span data-ttu-id="545ee-289">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="545ee-289">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="545ee-290">Determinar a frequência de verificação de uma conexão de mesmo nível.</span><span class="sxs-lookup"><span data-stu-id="545ee-290">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="545ee-291">.</span><span class="sxs-lookup"><span data-stu-id="545ee-291">.</span></span> <span data-ttu-id="545ee-292">Os valores possíveis são: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="545ee-292">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="545ee-293">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="545ee-293">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="545ee-294">Booliano</span><span class="sxs-lookup"><span data-stu-id="545ee-294">Boolean</span></span>|<span data-ttu-id="545ee-295">Desabilitar MOBIKE</span><span class="sxs-lookup"><span data-stu-id="545ee-295">Disable MOBIKE</span></span>|
|<span data-ttu-id="545ee-296">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="545ee-296">disableRedirect</span></span>|<span data-ttu-id="545ee-297">Booliano</span><span class="sxs-lookup"><span data-stu-id="545ee-297">Boolean</span></span>|<span data-ttu-id="545ee-298">Desabilitar redirecionamento</span><span class="sxs-lookup"><span data-stu-id="545ee-298">Disable Redirect</span></span>|
|<span data-ttu-id="545ee-299">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="545ee-299">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="545ee-300">Booliano</span><span class="sxs-lookup"><span data-stu-id="545ee-300">Boolean</span></span>|<span data-ttu-id="545ee-301">Habilita uma verificação de revogação de melhor esforço; o tempo limite de resposta do servidor não causará falha</span><span class="sxs-lookup"><span data-stu-id="545ee-301">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="545ee-302">enableEAP</span><span class="sxs-lookup"><span data-stu-id="545ee-302">enableEAP</span></span>|<span data-ttu-id="545ee-303">Booliano</span><span class="sxs-lookup"><span data-stu-id="545ee-303">Boolean</span></span>|<span data-ttu-id="545ee-304">Habilita a autenticação somente EAP</span><span class="sxs-lookup"><span data-stu-id="545ee-304">Enables EAP only authentication</span></span>|
|<span data-ttu-id="545ee-305">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="545ee-305">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="545ee-306">Booliano</span><span class="sxs-lookup"><span data-stu-id="545ee-306">Boolean</span></span>|<span data-ttu-id="545ee-307">Habilitar sigilo total na transferência (PFS).</span><span class="sxs-lookup"><span data-stu-id="545ee-307">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="545ee-308">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="545ee-308">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="545ee-309">Booliano</span><span class="sxs-lookup"><span data-stu-id="545ee-309">Boolean</span></span>|<span data-ttu-id="545ee-310">Habilitar o uso de atributos de sub-rede interna.</span><span class="sxs-lookup"><span data-stu-id="545ee-310">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="545ee-311">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="545ee-311">localIdentifier</span></span>|[<span data-ttu-id="545ee-312">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="545ee-312">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="545ee-313">Método de identificação do cliente que está tentando se conectar via VPN.</span><span class="sxs-lookup"><span data-stu-id="545ee-313">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="545ee-314">.</span><span class="sxs-lookup"><span data-stu-id="545ee-314">.</span></span> <span data-ttu-id="545ee-315">Os valores possíveis são: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="545ee-315">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="545ee-316">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="545ee-316">remoteIdentifier</span></span>|<span data-ttu-id="545ee-317">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="545ee-317">String</span></span>|<span data-ttu-id="545ee-318">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="545ee-318">Address of the IKEv2 server.</span></span> <span data-ttu-id="545ee-319">Deve ser um FQDN, userfqdn, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="545ee-319">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="545ee-320">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="545ee-320">securityAssociationParameters</span></span>|[<span data-ttu-id="545ee-321">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="545ee-321">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="545ee-322">Parâmetros de associação de segurança</span><span class="sxs-lookup"><span data-stu-id="545ee-322">Security Association Parameters</span></span>|
|<span data-ttu-id="545ee-323">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="545ee-323">serverCertificateCommonName</span></span>|<span data-ttu-id="545ee-324">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="545ee-324">String</span></span>|<span data-ttu-id="545ee-325">Nome comum do certificado de servidor IKEv2 usado na autenticação de servidor</span><span class="sxs-lookup"><span data-stu-id="545ee-325">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="545ee-326">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="545ee-326">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="545ee-327">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="545ee-327">String</span></span>|<span data-ttu-id="545ee-328">Nome comum do emissor do emissor do certificado do servidor IKEv2 usado na autenticação</span><span class="sxs-lookup"><span data-stu-id="545ee-328">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="545ee-329">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="545ee-329">serverCertificateType</span></span>|[<span data-ttu-id="545ee-330">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="545ee-330">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="545ee-331">O tipo de certificado que o servidor VPN apresentará ao cliente VPN para autenticação.</span><span class="sxs-lookup"><span data-stu-id="545ee-331">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="545ee-332">Os valores possíveis são: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="545ee-332">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="545ee-333">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="545ee-333">sharedSecret</span></span>|<span data-ttu-id="545ee-334">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="545ee-334">String</span></span>|<span data-ttu-id="545ee-335">Usado quando a autenticação secreta compartilhada está selecionada</span><span class="sxs-lookup"><span data-stu-id="545ee-335">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="545ee-336">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="545ee-336">tlsMaximumVersion</span></span>|<span data-ttu-id="545ee-337">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="545ee-337">String</span></span>|<span data-ttu-id="545ee-338">A versão máxima do TLS a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="545ee-338">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="545ee-339">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="545ee-339">tlsMinimumVersion</span></span>|<span data-ttu-id="545ee-340">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="545ee-340">String</span></span>|<span data-ttu-id="545ee-341">A versão de TLS mínima a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="545ee-341">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="545ee-342">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="545ee-342">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="545ee-343">Booliano</span><span class="sxs-lookup"><span data-stu-id="545ee-343">Boolean</span></span>|<span data-ttu-id="545ee-344">Permite o uso de parâmetros de associação de segurança por meio da configuração de todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="545ee-344">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="545ee-345">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="545ee-345">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="545ee-346">Booliano</span><span class="sxs-lookup"><span data-stu-id="545ee-346">Boolean</span></span>|<span data-ttu-id="545ee-347">Permite o uso de parâmetros de associação de segurança filhos ao definir todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="545ee-347">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="545ee-348">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="545ee-348">alwaysOnConfiguration</span></span>|[<span data-ttu-id="545ee-349">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="545ee-349">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="545ee-350">Configuração do AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="545ee-350">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="545ee-351">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="545ee-351">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="545ee-352">Booliano</span><span class="sxs-lookup"><span data-stu-id="545ee-352">Boolean</span></span>|<span data-ttu-id="545ee-353">Determina se a VPN AlwaysOn está habilitada</span><span class="sxs-lookup"><span data-stu-id="545ee-353">Determines if Always on VPN is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="545ee-354">Resposta</span><span class="sxs-lookup"><span data-stu-id="545ee-354">Response</span></span>
<span data-ttu-id="545ee-355">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="545ee-355">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="545ee-356">Exemplo</span><span class="sxs-lookup"><span data-stu-id="545ee-356">Example</span></span>

### <a name="request"></a><span data-ttu-id="545ee-357">Solicitação</span><span class="sxs-lookup"><span data-stu-id="545ee-357">Request</span></span>
<span data-ttu-id="545ee-358">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="545ee-358">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="545ee-359">Resposta</span><span class="sxs-lookup"><span data-stu-id="545ee-359">Response</span></span>
<span data-ttu-id="545ee-p139">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="545ee-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





