---
title: Criar iosikEv2VpnConfiguration
description: Criar um novo objeto iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b6ad2347590b17fac351cb178901230a77bba13
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43438971"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="75dc0-103">Criar iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="75dc0-103">Create iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="75dc0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75dc0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75dc0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75dc0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75dc0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75dc0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75dc0-107">Criar um novo objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="75dc0-107">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75dc0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="75dc0-108">Prerequisites</span></span>
<span data-ttu-id="75dc0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75dc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75dc0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75dc0-111">Permission type</span></span>|<span data-ttu-id="75dc0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="75dc0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75dc0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75dc0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75dc0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75dc0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75dc0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75dc0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75dc0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75dc0-116">Not supported.</span></span>|
|<span data-ttu-id="75dc0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75dc0-117">Application</span></span>|<span data-ttu-id="75dc0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75dc0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75dc0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75dc0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="75dc0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75dc0-120">Request headers</span></span>
|<span data-ttu-id="75dc0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75dc0-121">Header</span></span>|<span data-ttu-id="75dc0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="75dc0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75dc0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="75dc0-123">Authorization</span></span>|<span data-ttu-id="75dc0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75dc0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75dc0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="75dc0-125">Accept</span></span>|<span data-ttu-id="75dc0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75dc0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75dc0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75dc0-127">Request body</span></span>
<span data-ttu-id="75dc0-128">No corpo da solicitação, forneça uma representação JSON do objeto iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="75dc0-128">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="75dc0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="75dc0-129">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="75dc0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75dc0-130">Property</span></span>|<span data-ttu-id="75dc0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="75dc0-131">Type</span></span>|<span data-ttu-id="75dc0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="75dc0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75dc0-133">id</span><span class="sxs-lookup"><span data-stu-id="75dc0-133">id</span></span>|<span data-ttu-id="75dc0-134">String</span><span class="sxs-lookup"><span data-stu-id="75dc0-134">String</span></span>|<span data-ttu-id="75dc0-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="75dc0-135">Key of the entity.</span></span> <span data-ttu-id="75dc0-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75dc0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="75dc0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75dc0-138">DateTimeOffset</span></span>|<span data-ttu-id="75dc0-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="75dc0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="75dc0-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="75dc0-141">roleScopeTagIds</span></span>|<span data-ttu-id="75dc0-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="75dc0-142">String collection</span></span>|<span data-ttu-id="75dc0-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="75dc0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="75dc0-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="75dc0-145">supportsScopeTags</span></span>|<span data-ttu-id="75dc0-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="75dc0-146">Boolean</span></span>|<span data-ttu-id="75dc0-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="75dc0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="75dc0-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="75dc0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="75dc0-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="75dc0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="75dc0-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="75dc0-150">This property is read-only.</span></span> <span data-ttu-id="75dc0-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="75dc0-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="75dc0-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="75dc0-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="75dc0-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="75dc0-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="75dc0-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="75dc0-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="75dc0-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="75dc0-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="75dc0-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="75dc0-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="75dc0-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="75dc0-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="75dc0-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="75dc0-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="75dc0-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="75dc0-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="75dc0-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75dc0-164">createdDateTime</span></span>|<span data-ttu-id="75dc0-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75dc0-165">DateTimeOffset</span></span>|<span data-ttu-id="75dc0-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="75dc0-166">DateTime the object was created.</span></span> <span data-ttu-id="75dc0-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-168">description</span><span class="sxs-lookup"><span data-stu-id="75dc0-168">description</span></span>|<span data-ttu-id="75dc0-169">String</span><span class="sxs-lookup"><span data-stu-id="75dc0-169">String</span></span>|<span data-ttu-id="75dc0-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75dc0-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="75dc0-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-172">displayName</span><span class="sxs-lookup"><span data-stu-id="75dc0-172">displayName</span></span>|<span data-ttu-id="75dc0-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75dc0-173">String</span></span>|<span data-ttu-id="75dc0-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75dc0-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="75dc0-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-176">versão</span><span class="sxs-lookup"><span data-stu-id="75dc0-176">version</span></span>|<span data-ttu-id="75dc0-177">Int32</span><span class="sxs-lookup"><span data-stu-id="75dc0-177">Int32</span></span>|<span data-ttu-id="75dc0-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75dc0-178">Version of the device configuration.</span></span> <span data-ttu-id="75dc0-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-180">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="75dc0-180">connectionName</span></span>|<span data-ttu-id="75dc0-181">String</span><span class="sxs-lookup"><span data-stu-id="75dc0-181">String</span></span>|<span data-ttu-id="75dc0-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="75dc0-182">Connection name displayed to the user.</span></span> <span data-ttu-id="75dc0-183">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-184">Connection</span><span class="sxs-lookup"><span data-stu-id="75dc0-184">connectionType</span></span>|[<span data-ttu-id="75dc0-185">Enumeraçãoapplevpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="75dc0-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="75dc0-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="75dc0-186">Connection type.</span></span> <span data-ttu-id="75dc0-187">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="75dc0-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="75dc0-188">Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span><span class="sxs-lookup"><span data-stu-id="75dc0-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span></span>|
|<span data-ttu-id="75dc0-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="75dc0-189">loginGroupOrDomain</span></span>|<span data-ttu-id="75dc0-190">String</span><span class="sxs-lookup"><span data-stu-id="75dc0-190">String</span></span>|<span data-ttu-id="75dc0-191">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="75dc0-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="75dc0-192">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-193">role</span><span class="sxs-lookup"><span data-stu-id="75dc0-193">role</span></span>|<span data-ttu-id="75dc0-194">String</span><span class="sxs-lookup"><span data-stu-id="75dc0-194">String</span></span>|<span data-ttu-id="75dc0-195">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="75dc0-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="75dc0-196">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-197">esfera</span><span class="sxs-lookup"><span data-stu-id="75dc0-197">realm</span></span>|<span data-ttu-id="75dc0-198">String</span><span class="sxs-lookup"><span data-stu-id="75dc0-198">String</span></span>|<span data-ttu-id="75dc0-199">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="75dc0-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="75dc0-200">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-201">do</span><span class="sxs-lookup"><span data-stu-id="75dc0-201">server</span></span>|[<span data-ttu-id="75dc0-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="75dc0-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="75dc0-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="75dc0-203">VPN Server on the network.</span></span> <span data-ttu-id="75dc0-204">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="75dc0-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="75dc0-205">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-206">identificador</span><span class="sxs-lookup"><span data-stu-id="75dc0-206">identifier</span></span>|<span data-ttu-id="75dc0-207">String</span><span class="sxs-lookup"><span data-stu-id="75dc0-207">String</span></span>|<span data-ttu-id="75dc0-208">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="75dc0-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="75dc0-209">Por exemplo: o Cisco AnyConnect usa um identificador do formulário com. Cisco. AnyConnect. applevpn. plugin herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-210">customData</span><span class="sxs-lookup"><span data-stu-id="75dc0-210">customData</span></span>|<span data-ttu-id="75dc0-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="75dc0-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="75dc0-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="75dc0-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="75dc0-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="75dc0-214">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="75dc0-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="75dc0-215">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="75dc0-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="75dc0-216">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-217">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="75dc0-217">customKeyValueData</span></span>|<span data-ttu-id="75dc0-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="75dc0-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="75dc0-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="75dc0-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="75dc0-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="75dc0-221">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="75dc0-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="75dc0-222">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="75dc0-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="75dc0-223">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="75dc0-224">enableSplitTunneling</span></span>|<span data-ttu-id="75dc0-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="75dc0-225">Boolean</span></span>|<span data-ttu-id="75dc0-226">Enviar todo o tráfego de rede através da VPN.</span><span class="sxs-lookup"><span data-stu-id="75dc0-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="75dc0-227">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="75dc0-228">authenticationMethod</span></span>|[<span data-ttu-id="75dc0-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="75dc0-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="75dc0-230">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="75dc0-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="75dc0-231">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="75dc0-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="75dc0-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="75dc0-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="75dc0-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="75dc0-233">enablePerApp</span></span>|<span data-ttu-id="75dc0-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="75dc0-234">Boolean</span></span>|<span data-ttu-id="75dc0-235">A configuração dessa opção como true cria uma carga de VPN por aplicativo, que pode ser mais tarde associada aos aplicativos que podem acionar esta conexão VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="75dc0-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="75dc0-236">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="75dc0-237">safariDomains</span></span>|<span data-ttu-id="75dc0-238">Coleção String</span><span class="sxs-lookup"><span data-stu-id="75dc0-238">String collection</span></span>|<span data-ttu-id="75dc0-239">Domínios Safari quando esta configuração VPN por aplicativo estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="75dc0-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="75dc0-240">Além dos aplicativos associados a essa VPN, os domínios Safari especificados aqui também serão capazes de acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="75dc0-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="75dc0-241">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="75dc0-242">onDemandRules</span></span>|<span data-ttu-id="75dc0-243">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="75dc0-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="75dc0-244">On-Demand Rules.</span></span> <span data-ttu-id="75dc0-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="75dc0-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="75dc0-246">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-247">proxyServer</span><span class="sxs-lookup"><span data-stu-id="75dc0-247">proxyServer</span></span>|[<span data-ttu-id="75dc0-248">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="75dc0-248">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="75dc0-249">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="75dc0-249">Proxy Server.</span></span> <span data-ttu-id="75dc0-250">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-251">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="75dc0-251">optInToDeviceIdSharing</span></span>|<span data-ttu-id="75dc0-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="75dc0-252">Boolean</span></span>|<span data-ttu-id="75dc0-253">Optar por compartilhar a ID do dispositivo para clientes VPN de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="75dc0-253">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="75dc0-254">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-254">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-255">providerType</span><span class="sxs-lookup"><span data-stu-id="75dc0-255">providerType</span></span>|[<span data-ttu-id="75dc0-256">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="75dc0-256">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="75dc0-257">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75dc0-257">Provider type for per-app VPN.</span></span> <span data-ttu-id="75dc0-258">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="75dc0-258">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span> <span data-ttu-id="75dc0-259">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="75dc0-259">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="75dc0-260">UserDomain</span><span class="sxs-lookup"><span data-stu-id="75dc0-260">userDomain</span></span>|<span data-ttu-id="75dc0-261">String</span><span class="sxs-lookup"><span data-stu-id="75dc0-261">String</span></span>|<span data-ttu-id="75dc0-262">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="75dc0-262">Zscaler only.</span></span> <span data-ttu-id="75dc0-263">Insira um domínio estático para preencher previamente o campo de logon com no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="75dc0-263">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="75dc0-264">Se for deixado em branco, o domínio do Azure Active Directory do usuário será usado.</span><span class="sxs-lookup"><span data-stu-id="75dc0-264">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="75dc0-265">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-265">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-266">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="75dc0-266">strictEnforcement</span></span>|<span data-ttu-id="75dc0-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="75dc0-267">Boolean</span></span>|<span data-ttu-id="75dc0-268">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="75dc0-268">Zscaler only.</span></span> <span data-ttu-id="75dc0-269">Bloqueia o tráfego de rede até que o usuário entre no Zscaler app.</span><span class="sxs-lookup"><span data-stu-id="75dc0-269">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="75dc0-270">"True" significa que o tráfego é bloqueado.</span><span class="sxs-lookup"><span data-stu-id="75dc0-270">"True" means traffic is blocked.</span></span> <span data-ttu-id="75dc0-271">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-271">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-272">cloudName</span><span class="sxs-lookup"><span data-stu-id="75dc0-272">cloudName</span></span>|<span data-ttu-id="75dc0-273">String</span><span class="sxs-lookup"><span data-stu-id="75dc0-273">String</span></span>|<span data-ttu-id="75dc0-274">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="75dc0-274">Zscaler only.</span></span> <span data-ttu-id="75dc0-275">Nuvem do Zscaler à qual o usuário está atribuído.</span><span class="sxs-lookup"><span data-stu-id="75dc0-275">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="75dc0-276">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-276">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-277">Excludelistpara</span><span class="sxs-lookup"><span data-stu-id="75dc0-277">excludeList</span></span>|<span data-ttu-id="75dc0-278">Coleção String</span><span class="sxs-lookup"><span data-stu-id="75dc0-278">String collection</span></span>|<span data-ttu-id="75dc0-279">Zscaler apenas.</span><span class="sxs-lookup"><span data-stu-id="75dc0-279">Zscaler only.</span></span> <span data-ttu-id="75dc0-280">Lista de endereços de rede que não são enviados pela nuvem do Zscaler.</span><span class="sxs-lookup"><span data-stu-id="75dc0-280">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="75dc0-281">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75dc0-281">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="75dc0-282">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="75dc0-282">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="75dc0-283">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="75dc0-283">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="75dc0-284">Parâmetros da Associação de segurança filho</span><span class="sxs-lookup"><span data-stu-id="75dc0-284">Child Security Association Parameters</span></span>|
|<span data-ttu-id="75dc0-285">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="75dc0-285">clientAuthenticationType</span></span>|[<span data-ttu-id="75dc0-286">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="75dc0-286">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="75dc0-287">Tipo de autenticação de cliente que o cliente VPN usará.</span><span class="sxs-lookup"><span data-stu-id="75dc0-287">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="75dc0-288">Os valores possíveis são: `userAuthentication` e `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="75dc0-288">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="75dc0-289">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="75dc0-289">deadPeerDetectionRate</span></span>|[<span data-ttu-id="75dc0-290">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="75dc0-290">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="75dc0-291">Determinar a frequência de verificação de uma conexão de mesmo nível.</span><span class="sxs-lookup"><span data-stu-id="75dc0-291">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="75dc0-292">.</span><span class="sxs-lookup"><span data-stu-id="75dc0-292">.</span></span> <span data-ttu-id="75dc0-293">Os valores possíveis são: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="75dc0-293">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="75dc0-294">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="75dc0-294">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="75dc0-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="75dc0-295">Boolean</span></span>|<span data-ttu-id="75dc0-296">Desabilitar MOBIKE</span><span class="sxs-lookup"><span data-stu-id="75dc0-296">Disable MOBIKE</span></span>|
|<span data-ttu-id="75dc0-297">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="75dc0-297">disableRedirect</span></span>|<span data-ttu-id="75dc0-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="75dc0-298">Boolean</span></span>|<span data-ttu-id="75dc0-299">Desabilitar redirecionamento</span><span class="sxs-lookup"><span data-stu-id="75dc0-299">Disable Redirect</span></span>|
|<span data-ttu-id="75dc0-300">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="75dc0-300">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="75dc0-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="75dc0-301">Boolean</span></span>|<span data-ttu-id="75dc0-302">Habilita uma verificação de revogação de melhor esforço; o tempo limite de resposta do servidor não causará falha</span><span class="sxs-lookup"><span data-stu-id="75dc0-302">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="75dc0-303">enableEAP</span><span class="sxs-lookup"><span data-stu-id="75dc0-303">enableEAP</span></span>|<span data-ttu-id="75dc0-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="75dc0-304">Boolean</span></span>|<span data-ttu-id="75dc0-305">Habilita a autenticação somente EAP</span><span class="sxs-lookup"><span data-stu-id="75dc0-305">Enables EAP only authentication</span></span>|
|<span data-ttu-id="75dc0-306">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="75dc0-306">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="75dc0-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="75dc0-307">Boolean</span></span>|<span data-ttu-id="75dc0-308">Habilitar sigilo total na transferência (PFS).</span><span class="sxs-lookup"><span data-stu-id="75dc0-308">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="75dc0-309">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="75dc0-309">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="75dc0-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="75dc0-310">Boolean</span></span>|<span data-ttu-id="75dc0-311">Habilitar o uso de atributos de sub-rede interna.</span><span class="sxs-lookup"><span data-stu-id="75dc0-311">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="75dc0-312">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="75dc0-312">localIdentifier</span></span>|[<span data-ttu-id="75dc0-313">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="75dc0-313">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="75dc0-314">Método de identificação do cliente que está tentando se conectar via VPN.</span><span class="sxs-lookup"><span data-stu-id="75dc0-314">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="75dc0-315">.</span><span class="sxs-lookup"><span data-stu-id="75dc0-315">.</span></span> <span data-ttu-id="75dc0-316">Os valores possíveis são: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="75dc0-316">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="75dc0-317">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="75dc0-317">remoteIdentifier</span></span>|<span data-ttu-id="75dc0-318">String</span><span class="sxs-lookup"><span data-stu-id="75dc0-318">String</span></span>|<span data-ttu-id="75dc0-319">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="75dc0-319">Address of the IKEv2 server.</span></span> <span data-ttu-id="75dc0-320">Deve ser um FQDN, userfqdn, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="75dc0-320">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="75dc0-321">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="75dc0-321">securityAssociationParameters</span></span>|[<span data-ttu-id="75dc0-322">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="75dc0-322">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="75dc0-323">Parâmetros de associação de segurança</span><span class="sxs-lookup"><span data-stu-id="75dc0-323">Security Association Parameters</span></span>|
|<span data-ttu-id="75dc0-324">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="75dc0-324">serverCertificateCommonName</span></span>|<span data-ttu-id="75dc0-325">String</span><span class="sxs-lookup"><span data-stu-id="75dc0-325">String</span></span>|<span data-ttu-id="75dc0-326">Nome comum do certificado de servidor IKEv2 usado na autenticação de servidor</span><span class="sxs-lookup"><span data-stu-id="75dc0-326">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="75dc0-327">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="75dc0-327">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="75dc0-328">String</span><span class="sxs-lookup"><span data-stu-id="75dc0-328">String</span></span>|<span data-ttu-id="75dc0-329">Nome comum do emissor do emissor do certificado do servidor IKEv2 usado na autenticação</span><span class="sxs-lookup"><span data-stu-id="75dc0-329">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="75dc0-330">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="75dc0-330">serverCertificateType</span></span>|[<span data-ttu-id="75dc0-331">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="75dc0-331">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="75dc0-332">O tipo de certificado que o servidor VPN apresentará ao cliente VPN para autenticação.</span><span class="sxs-lookup"><span data-stu-id="75dc0-332">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="75dc0-333">Os valores possíveis são: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="75dc0-333">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="75dc0-334">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="75dc0-334">sharedSecret</span></span>|<span data-ttu-id="75dc0-335">String</span><span class="sxs-lookup"><span data-stu-id="75dc0-335">String</span></span>|<span data-ttu-id="75dc0-336">Usado quando a autenticação secreta compartilhada está selecionada</span><span class="sxs-lookup"><span data-stu-id="75dc0-336">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="75dc0-337">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="75dc0-337">tlsMaximumVersion</span></span>|<span data-ttu-id="75dc0-338">String</span><span class="sxs-lookup"><span data-stu-id="75dc0-338">String</span></span>|<span data-ttu-id="75dc0-339">A versão máxima do TLS a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="75dc0-339">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="75dc0-340">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="75dc0-340">tlsMinimumVersion</span></span>|<span data-ttu-id="75dc0-341">String</span><span class="sxs-lookup"><span data-stu-id="75dc0-341">String</span></span>|<span data-ttu-id="75dc0-342">A versão de TLS mínima a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="75dc0-342">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="75dc0-343">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="75dc0-343">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="75dc0-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="75dc0-344">Boolean</span></span>|<span data-ttu-id="75dc0-345">Permite o uso de parâmetros de associação de segurança por meio da configuração de todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="75dc0-345">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="75dc0-346">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="75dc0-346">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="75dc0-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="75dc0-347">Boolean</span></span>|<span data-ttu-id="75dc0-348">Permite o uso de parâmetros de associação de segurança filhos ao definir todos os parâmetros para o padrão do dispositivo, a menos que explicitamente especificado.</span><span class="sxs-lookup"><span data-stu-id="75dc0-348">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="75dc0-349">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="75dc0-349">alwaysOnConfiguration</span></span>|[<span data-ttu-id="75dc0-350">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="75dc0-350">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="75dc0-351">Configuração do AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="75dc0-351">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="75dc0-352">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="75dc0-352">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="75dc0-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="75dc0-353">Boolean</span></span>|<span data-ttu-id="75dc0-354">Determina se a VPN AlwaysOn está habilitada</span><span class="sxs-lookup"><span data-stu-id="75dc0-354">Determines if Always on VPN is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="75dc0-355">Resposta</span><span class="sxs-lookup"><span data-stu-id="75dc0-355">Response</span></span>
<span data-ttu-id="75dc0-356">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75dc0-356">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75dc0-357">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75dc0-357">Example</span></span>

### <a name="request"></a><span data-ttu-id="75dc0-358">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75dc0-358">Request</span></span>
<span data-ttu-id="75dc0-359">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75dc0-359">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="75dc0-360">Resposta</span><span class="sxs-lookup"><span data-stu-id="75dc0-360">Response</span></span>
<span data-ttu-id="75dc0-p139">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75dc0-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



