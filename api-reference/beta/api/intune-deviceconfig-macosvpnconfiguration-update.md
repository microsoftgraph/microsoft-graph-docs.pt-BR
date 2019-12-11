---
title: Atualizar macOSVpnConfiguration
description: Atualiza as propriedades de um objeto macOSVpnConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b1f22216017092e7159dd4dcde59557242ca026a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948069"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="9138d-103">Atualizar macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="9138d-103">Update macOSVpnConfiguration</span></span>

> <span data-ttu-id="9138d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9138d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9138d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9138d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9138d-106">Atualiza as propriedades de um objeto [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9138d-106">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9138d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9138d-107">Prerequisites</span></span>
<span data-ttu-id="9138d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9138d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9138d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9138d-110">Permission type</span></span>|<span data-ttu-id="9138d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9138d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9138d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9138d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9138d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9138d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9138d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9138d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9138d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9138d-115">Not supported.</span></span>|
|<span data-ttu-id="9138d-116">Application</span><span class="sxs-lookup"><span data-stu-id="9138d-116">Application</span></span>|<span data-ttu-id="9138d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9138d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9138d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9138d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9138d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9138d-119">Request headers</span></span>
|<span data-ttu-id="9138d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9138d-120">Header</span></span>|<span data-ttu-id="9138d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9138d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9138d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9138d-122">Authorization</span></span>|<span data-ttu-id="9138d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9138d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9138d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9138d-124">Accept</span></span>|<span data-ttu-id="9138d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9138d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9138d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9138d-126">Request body</span></span>
<span data-ttu-id="9138d-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9138d-127">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="9138d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9138d-128">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="9138d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9138d-129">Property</span></span>|<span data-ttu-id="9138d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9138d-130">Type</span></span>|<span data-ttu-id="9138d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9138d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9138d-132">id</span><span class="sxs-lookup"><span data-stu-id="9138d-132">id</span></span>|<span data-ttu-id="9138d-133">String</span><span class="sxs-lookup"><span data-stu-id="9138d-133">String</span></span>|<span data-ttu-id="9138d-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9138d-134">Key of the entity.</span></span> <span data-ttu-id="9138d-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9138d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9138d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9138d-137">DateTimeOffset</span></span>|<span data-ttu-id="9138d-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9138d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9138d-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9138d-140">roleScopeTagIds</span></span>|<span data-ttu-id="9138d-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9138d-141">String collection</span></span>|<span data-ttu-id="9138d-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="9138d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9138d-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9138d-144">supportsScopeTags</span></span>|<span data-ttu-id="9138d-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9138d-145">Boolean</span></span>|<span data-ttu-id="9138d-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9138d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9138d-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9138d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9138d-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9138d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9138d-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9138d-149">This property is read-only.</span></span> <span data-ttu-id="9138d-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9138d-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9138d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9138d-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9138d-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="9138d-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9138d-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9138d-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9138d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9138d-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9138d-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="9138d-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9138d-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9138d-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9138d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9138d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9138d-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="9138d-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9138d-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9138d-163">createdDateTime</span></span>|<span data-ttu-id="9138d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9138d-164">DateTimeOffset</span></span>|<span data-ttu-id="9138d-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9138d-165">DateTime the object was created.</span></span> <span data-ttu-id="9138d-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-167">description</span><span class="sxs-lookup"><span data-stu-id="9138d-167">description</span></span>|<span data-ttu-id="9138d-168">String</span><span class="sxs-lookup"><span data-stu-id="9138d-168">String</span></span>|<span data-ttu-id="9138d-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9138d-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9138d-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9138d-171">displayName</span></span>|<span data-ttu-id="9138d-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9138d-172">String</span></span>|<span data-ttu-id="9138d-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9138d-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9138d-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-175">versão</span><span class="sxs-lookup"><span data-stu-id="9138d-175">version</span></span>|<span data-ttu-id="9138d-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9138d-176">Int32</span></span>|<span data-ttu-id="9138d-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9138d-177">Version of the device configuration.</span></span> <span data-ttu-id="9138d-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-179">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="9138d-179">connectionName</span></span>|<span data-ttu-id="9138d-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="9138d-180">String</span></span>|<span data-ttu-id="9138d-181">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="9138d-181">Connection name displayed to the user.</span></span> <span data-ttu-id="9138d-182">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-183">Connection</span><span class="sxs-lookup"><span data-stu-id="9138d-183">connectionType</span></span>|[<span data-ttu-id="9138d-184">Enumeraçãoapplevpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="9138d-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="9138d-185">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="9138d-185">Connection type.</span></span> <span data-ttu-id="9138d-186">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9138d-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="9138d-187">Os valores possíveis são `ciscoAnyConnect`: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span><span class="sxs-lookup"><span data-stu-id="9138d-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`.</span></span>|
|<span data-ttu-id="9138d-188">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="9138d-188">loginGroupOrDomain</span></span>|<span data-ttu-id="9138d-189">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="9138d-189">String</span></span>|<span data-ttu-id="9138d-190">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="9138d-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="9138d-191">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-192">role</span><span class="sxs-lookup"><span data-stu-id="9138d-192">role</span></span>|<span data-ttu-id="9138d-193">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="9138d-193">String</span></span>|<span data-ttu-id="9138d-194">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="9138d-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="9138d-195">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-196">esfera</span><span class="sxs-lookup"><span data-stu-id="9138d-196">realm</span></span>|<span data-ttu-id="9138d-197">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="9138d-197">String</span></span>|<span data-ttu-id="9138d-198">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="9138d-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="9138d-199">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-200">do</span><span class="sxs-lookup"><span data-stu-id="9138d-200">server</span></span>|[<span data-ttu-id="9138d-201">vpnServer</span><span class="sxs-lookup"><span data-stu-id="9138d-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="9138d-202">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="9138d-202">VPN Server on the network.</span></span> <span data-ttu-id="9138d-203">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="9138d-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="9138d-204">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-205">identificador</span><span class="sxs-lookup"><span data-stu-id="9138d-205">identifier</span></span>|<span data-ttu-id="9138d-206">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="9138d-206">String</span></span>|<span data-ttu-id="9138d-207">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="9138d-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="9138d-208">Por exemplo: o Cisco AnyConnect usa um identificador do formulário com. Cisco. AnyConnect. applevpn. plugin herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-209">customData</span><span class="sxs-lookup"><span data-stu-id="9138d-209">customData</span></span>|<span data-ttu-id="9138d-210">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="9138d-211">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="9138d-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="9138d-212">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="9138d-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="9138d-213">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="9138d-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="9138d-214">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="9138d-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="9138d-215">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-216">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="9138d-216">customKeyValueData</span></span>|<span data-ttu-id="9138d-217">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="9138d-218">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="9138d-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="9138d-219">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="9138d-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="9138d-220">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="9138d-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="9138d-221">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="9138d-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="9138d-222">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-223">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="9138d-223">enableSplitTunneling</span></span>|<span data-ttu-id="9138d-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="9138d-224">Boolean</span></span>|<span data-ttu-id="9138d-225">Enviar todo o tráfego de rede através da VPN.</span><span class="sxs-lookup"><span data-stu-id="9138d-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="9138d-226">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-227">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9138d-227">authenticationMethod</span></span>|[<span data-ttu-id="9138d-228">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9138d-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="9138d-229">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="9138d-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="9138d-230">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9138d-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="9138d-231">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="9138d-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="9138d-232">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="9138d-232">enablePerApp</span></span>|<span data-ttu-id="9138d-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="9138d-233">Boolean</span></span>|<span data-ttu-id="9138d-234">A configuração dessa opção como true cria uma carga de VPN por aplicativo, que pode ser mais tarde associada aos aplicativos que podem acionar esta conexão VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="9138d-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="9138d-235">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-236">safariDomains</span><span class="sxs-lookup"><span data-stu-id="9138d-236">safariDomains</span></span>|<span data-ttu-id="9138d-237">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9138d-237">String collection</span></span>|<span data-ttu-id="9138d-238">Domínios Safari quando esta configuração VPN por aplicativo estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="9138d-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="9138d-239">Além dos aplicativos associados a essa VPN, os domínios Safari especificados aqui também serão capazes de acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="9138d-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="9138d-240">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-241">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="9138d-241">onDemandRules</span></span>|<span data-ttu-id="9138d-242">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="9138d-243">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="9138d-243">On-Demand Rules.</span></span> <span data-ttu-id="9138d-244">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="9138d-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="9138d-245">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-246">proxyServer</span><span class="sxs-lookup"><span data-stu-id="9138d-246">proxyServer</span></span>|[<span data-ttu-id="9138d-247">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="9138d-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="9138d-248">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="9138d-248">Proxy Server.</span></span> <span data-ttu-id="9138d-249">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="9138d-250">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="9138d-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="9138d-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="9138d-251">Boolean</span></span>|<span data-ttu-id="9138d-252">Optar por compartilhar a ID do dispositivo para clientes VPN de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="9138d-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="9138d-253">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9138d-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9138d-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="9138d-254">Response</span></span>
<span data-ttu-id="9138d-255">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9138d-255">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9138d-256">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9138d-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="9138d-257">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9138d-257">Request</span></span>
<span data-ttu-id="9138d-258">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9138d-258">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2630

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
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
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="9138d-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="9138d-259">Response</span></span>
<span data-ttu-id="9138d-p129">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9138d-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2802

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
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
  "optInToDeviceIdSharing": true
}
```





