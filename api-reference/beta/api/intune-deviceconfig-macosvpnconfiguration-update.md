---
title: Atualizar macOSVpnConfiguration
description: Atualiza as propriedades de um objeto macOSVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6487799442fe1b2601d9f5420a677bf6289c6a19
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708442"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="ab567-103">Atualizar macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ab567-103">Update macOSVpnConfiguration</span></span>

<span data-ttu-id="ab567-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab567-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab567-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ab567-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab567-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ab567-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab567-107">Atualiza as propriedades de um objeto [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ab567-107">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab567-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ab567-108">Prerequisites</span></span>
<span data-ttu-id="ab567-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab567-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab567-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab567-111">Permission type</span></span>|<span data-ttu-id="ab567-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ab567-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab567-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab567-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab567-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab567-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ab567-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab567-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab567-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab567-116">Not supported.</span></span>|
|<span data-ttu-id="ab567-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab567-117">Application</span></span>|<span data-ttu-id="ab567-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab567-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab567-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab567-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ab567-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab567-120">Request headers</span></span>
|<span data-ttu-id="ab567-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab567-121">Header</span></span>|<span data-ttu-id="ab567-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ab567-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab567-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab567-123">Authorization</span></span>|<span data-ttu-id="ab567-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab567-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab567-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ab567-125">Accept</span></span>|<span data-ttu-id="ab567-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab567-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab567-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab567-127">Request body</span></span>
<span data-ttu-id="ab567-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ab567-128">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="ab567-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab567-129">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="ab567-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab567-130">Property</span></span>|<span data-ttu-id="ab567-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab567-131">Type</span></span>|<span data-ttu-id="ab567-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab567-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab567-133">id</span><span class="sxs-lookup"><span data-stu-id="ab567-133">id</span></span>|<span data-ttu-id="ab567-134">String</span><span class="sxs-lookup"><span data-stu-id="ab567-134">String</span></span>|<span data-ttu-id="ab567-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ab567-135">Key of the entity.</span></span> <span data-ttu-id="ab567-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab567-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ab567-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab567-138">DateTimeOffset</span></span>|<span data-ttu-id="ab567-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ab567-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ab567-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ab567-141">roleScopeTagIds</span></span>|<span data-ttu-id="ab567-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab567-142">String collection</span></span>|<span data-ttu-id="ab567-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="ab567-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ab567-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ab567-145">supportsScopeTags</span></span>|<span data-ttu-id="ab567-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab567-146">Boolean</span></span>|<span data-ttu-id="ab567-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ab567-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ab567-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ab567-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ab567-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ab567-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ab567-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab567-150">This property is read-only.</span></span> <span data-ttu-id="ab567-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ab567-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ab567-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ab567-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ab567-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="ab567-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ab567-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ab567-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ab567-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ab567-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ab567-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="ab567-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ab567-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ab567-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ab567-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ab567-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ab567-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="ab567-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ab567-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab567-164">createdDateTime</span></span>|<span data-ttu-id="ab567-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab567-165">DateTimeOffset</span></span>|<span data-ttu-id="ab567-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ab567-166">DateTime the object was created.</span></span> <span data-ttu-id="ab567-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-168">description</span><span class="sxs-lookup"><span data-stu-id="ab567-168">description</span></span>|<span data-ttu-id="ab567-169">String</span><span class="sxs-lookup"><span data-stu-id="ab567-169">String</span></span>|<span data-ttu-id="ab567-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab567-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ab567-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ab567-172">displayName</span></span>|<span data-ttu-id="ab567-173">String</span><span class="sxs-lookup"><span data-stu-id="ab567-173">String</span></span>|<span data-ttu-id="ab567-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab567-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ab567-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-176">versão</span><span class="sxs-lookup"><span data-stu-id="ab567-176">version</span></span>|<span data-ttu-id="ab567-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ab567-177">Int32</span></span>|<span data-ttu-id="ab567-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab567-178">Version of the device configuration.</span></span> <span data-ttu-id="ab567-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="ab567-180">connectionName</span></span>|<span data-ttu-id="ab567-181">String</span><span class="sxs-lookup"><span data-stu-id="ab567-181">String</span></span>|<span data-ttu-id="ab567-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="ab567-182">Connection name displayed to the user.</span></span> <span data-ttu-id="ab567-183">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-184">Connection</span><span class="sxs-lookup"><span data-stu-id="ab567-184">connectionType</span></span>|[<span data-ttu-id="ab567-185">Enumeraçãoapplevpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="ab567-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="ab567-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="ab567-186">Connection type.</span></span> <span data-ttu-id="ab567-187">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab567-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ab567-188">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,,,,, `ciscoAnyConnect` `pulseSecure` `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` , `alwaysOn` , `microsoftTunnel` , `netMotionMobility` .</span><span class="sxs-lookup"><span data-stu-id="ab567-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`.</span></span>|
|<span data-ttu-id="ab567-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="ab567-189">loginGroupOrDomain</span></span>|<span data-ttu-id="ab567-190">String</span><span class="sxs-lookup"><span data-stu-id="ab567-190">String</span></span>|<span data-ttu-id="ab567-191">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="ab567-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="ab567-192">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-193">role</span><span class="sxs-lookup"><span data-stu-id="ab567-193">role</span></span>|<span data-ttu-id="ab567-194">String</span><span class="sxs-lookup"><span data-stu-id="ab567-194">String</span></span>|<span data-ttu-id="ab567-195">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="ab567-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="ab567-196">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-197">esfera</span><span class="sxs-lookup"><span data-stu-id="ab567-197">realm</span></span>|<span data-ttu-id="ab567-198">String</span><span class="sxs-lookup"><span data-stu-id="ab567-198">String</span></span>|<span data-ttu-id="ab567-199">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="ab567-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="ab567-200">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-201">do</span><span class="sxs-lookup"><span data-stu-id="ab567-201">server</span></span>|[<span data-ttu-id="ab567-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="ab567-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="ab567-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="ab567-203">VPN Server on the network.</span></span> <span data-ttu-id="ab567-204">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="ab567-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="ab567-205">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-206">identificador</span><span class="sxs-lookup"><span data-stu-id="ab567-206">identifier</span></span>|<span data-ttu-id="ab567-207">String</span><span class="sxs-lookup"><span data-stu-id="ab567-207">String</span></span>|<span data-ttu-id="ab567-208">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="ab567-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ab567-209">Por exemplo: o Cisco AnyConnect usa um identificador do formulário com. Cisco. AnyConnect. applevpn. plugin herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-210">customData</span><span class="sxs-lookup"><span data-stu-id="ab567-210">customData</span></span>|<span data-ttu-id="ab567-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="ab567-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="ab567-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ab567-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="ab567-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="ab567-214">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="ab567-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="ab567-215">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="ab567-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="ab567-216">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-217">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="ab567-217">customKeyValueData</span></span>|<span data-ttu-id="ab567-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ab567-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="ab567-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ab567-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="ab567-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="ab567-221">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="ab567-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="ab567-222">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="ab567-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="ab567-223">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="ab567-224">enableSplitTunneling</span></span>|<span data-ttu-id="ab567-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab567-225">Boolean</span></span>|<span data-ttu-id="ab567-226">Enviar todo o tráfego de rede através da VPN.</span><span class="sxs-lookup"><span data-stu-id="ab567-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="ab567-227">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ab567-228">authenticationMethod</span></span>|[<span data-ttu-id="ab567-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ab567-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="ab567-230">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="ab567-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="ab567-231">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab567-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ab567-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="ab567-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="ab567-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="ab567-233">enablePerApp</span></span>|<span data-ttu-id="ab567-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab567-234">Boolean</span></span>|<span data-ttu-id="ab567-235">Definir isso como true cria Per-App carga de VPN que pode ser associada posteriormente a aplicativos que podem acionar esta VPN conexão no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="ab567-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="ab567-236">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="ab567-237">safariDomains</span></span>|<span data-ttu-id="ab567-238">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab567-238">String collection</span></span>|<span data-ttu-id="ab567-239">Domínios Safari quando esta configuração VPN por aplicativo estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="ab567-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="ab567-240">Além dos aplicativos associados a essa VPN, os domínios Safari especificados aqui também serão capazes de acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="ab567-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="ab567-241">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="ab567-242">onDemandRules</span></span>|<span data-ttu-id="ab567-243">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="ab567-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="ab567-244">On-Demand Rules.</span></span> <span data-ttu-id="ab567-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ab567-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ab567-246">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-247">providerType</span><span class="sxs-lookup"><span data-stu-id="ab567-247">providerType</span></span>|[<span data-ttu-id="ab567-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="ab567-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="ab567-249">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ab567-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="ab567-250">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab567-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ab567-251">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="ab567-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="ab567-252">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="ab567-252">excludedDomains</span></span>|<span data-ttu-id="ab567-253">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab567-253">String collection</span></span>|<span data-ttu-id="ab567-254">Domínios que são acessados por meio da Internet pública em vez de via VPN, mesmo quando a VPN por aplicativo é ativada herdada de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-254">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-255">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="ab567-255">disableOnDemandUserOverride</span></span>|<span data-ttu-id="ab567-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab567-256">Boolean</span></span>|<span data-ttu-id="ab567-257">Alternar para impedir que o usuário desabilite a VPN automática no aplicativo de configurações herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-257">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-258">proxyServer</span><span class="sxs-lookup"><span data-stu-id="ab567-258">proxyServer</span></span>|[<span data-ttu-id="ab567-259">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="ab567-259">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="ab567-260">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="ab567-260">Proxy Server.</span></span> <span data-ttu-id="ab567-261">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-261">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ab567-262">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="ab567-262">optInToDeviceIdSharing</span></span>|<span data-ttu-id="ab567-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab567-263">Boolean</span></span>|<span data-ttu-id="ab567-264">Opt-In compartilhar a ID do dispositivo para clientes VPN de terceiros para uso durante a validação do controle de acesso de rede.</span><span class="sxs-lookup"><span data-stu-id="ab567-264">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="ab567-265">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab567-265">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ab567-266">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab567-266">Response</span></span>
<span data-ttu-id="ab567-267">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab567-267">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab567-268">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab567-268">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab567-269">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab567-269">Request</span></span>
<span data-ttu-id="ab567-270">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab567-270">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2761

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
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="ab567-271">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab567-271">Response</span></span>
<span data-ttu-id="ab567-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab567-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2933

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
  "optInToDeviceIdSharing": true
}
```





