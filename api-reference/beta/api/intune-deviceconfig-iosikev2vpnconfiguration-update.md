---
title: Atualizar iosikEv2VpnConfiguration
description: Atualizar as propriedades de um objeto iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b7ad685e3bf5340e3026b5f3ccd07b217c809856
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156046"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="ae709-103">Atualizar iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae709-103">Update iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="ae709-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae709-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ae709-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae709-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae709-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae709-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae709-107">Atualizar as propriedades de um [objeto iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-107">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae709-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ae709-108">Prerequisites</span></span>
<span data-ttu-id="ae709-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae709-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae709-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ae709-111">Permission type</span></span>|<span data-ttu-id="ae709-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ae709-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae709-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ae709-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae709-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae709-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ae709-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ae709-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae709-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ae709-116">Not supported.</span></span>|
|<span data-ttu-id="ae709-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ae709-117">Application</span></span>|<span data-ttu-id="ae709-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae709-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae709-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ae709-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ae709-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ae709-120">Request headers</span></span>
|<span data-ttu-id="ae709-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ae709-121">Header</span></span>|<span data-ttu-id="ae709-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ae709-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae709-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ae709-123">Authorization</span></span>|<span data-ttu-id="ae709-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae709-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae709-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ae709-125">Accept</span></span>|<span data-ttu-id="ae709-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae709-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae709-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ae709-127">Request body</span></span>
<span data-ttu-id="ae709-128">No corpo da solicitação, fornece uma representação JSON do objeto [iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-128">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="ae709-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae709-129">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="ae709-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae709-130">Property</span></span>|<span data-ttu-id="ae709-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae709-131">Type</span></span>|<span data-ttu-id="ae709-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae709-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae709-133">id</span><span class="sxs-lookup"><span data-stu-id="ae709-133">id</span></span>|<span data-ttu-id="ae709-134">String</span><span class="sxs-lookup"><span data-stu-id="ae709-134">String</span></span>|<span data-ttu-id="ae709-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ae709-135">Key of the entity.</span></span> <span data-ttu-id="ae709-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae709-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ae709-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae709-138">DateTimeOffset</span></span>|<span data-ttu-id="ae709-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ae709-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ae709-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ae709-141">roleScopeTagIds</span></span>|<span data-ttu-id="ae709-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae709-142">String collection</span></span>|<span data-ttu-id="ae709-143">Lista de Marcas de Escopo para esta instância de Entidade.</span><span class="sxs-lookup"><span data-stu-id="ae709-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ae709-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ae709-145">supportsScopeTags</span></span>|<span data-ttu-id="ae709-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae709-146">Boolean</span></span>|<span data-ttu-id="ae709-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ae709-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ae709-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ae709-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ae709-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvida excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ae709-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ae709-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae709-150">This property is read-only.</span></span> <span data-ttu-id="ae709-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ae709-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ae709-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ae709-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ae709-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ae709-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ae709-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ae709-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ae709-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ae709-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ae709-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ae709-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ae709-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ae709-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ae709-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ae709-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ae709-162">A regra de aplicabilidade do modo de dispositivo para esta política.</span><span class="sxs-lookup"><span data-stu-id="ae709-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ae709-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae709-164">createdDateTime</span></span>|<span data-ttu-id="ae709-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae709-165">DateTimeOffset</span></span>|<span data-ttu-id="ae709-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ae709-166">DateTime the object was created.</span></span> <span data-ttu-id="ae709-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-168">description</span><span class="sxs-lookup"><span data-stu-id="ae709-168">description</span></span>|<span data-ttu-id="ae709-169">String</span><span class="sxs-lookup"><span data-stu-id="ae709-169">String</span></span>|<span data-ttu-id="ae709-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ae709-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ae709-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ae709-172">displayName</span></span>|<span data-ttu-id="ae709-173">String</span><span class="sxs-lookup"><span data-stu-id="ae709-173">String</span></span>|<span data-ttu-id="ae709-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ae709-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ae709-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-176">versão</span><span class="sxs-lookup"><span data-stu-id="ae709-176">version</span></span>|<span data-ttu-id="ae709-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ae709-177">Int32</span></span>|<span data-ttu-id="ae709-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ae709-178">Version of the device configuration.</span></span> <span data-ttu-id="ae709-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="ae709-180">connectionName</span></span>|<span data-ttu-id="ae709-181">String</span><span class="sxs-lookup"><span data-stu-id="ae709-181">String</span></span>|<span data-ttu-id="ae709-182">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="ae709-182">Connection name displayed to the user.</span></span> <span data-ttu-id="ae709-183">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="ae709-184">connectionType</span></span>|[<span data-ttu-id="ae709-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="ae709-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="ae709-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="ae709-186">Connection type.</span></span> <span data-ttu-id="ae709-187">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae709-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ae709-188">Os valores possíveis `ciscoAnyConnect` são: `pulseSecure` , , , , , , , , `f5EdgeClient` , , , , , , , `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` , `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` `netMotionMobility` `microsoftProtect` .</span><span class="sxs-lookup"><span data-stu-id="ae709-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="ae709-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="ae709-189">loginGroupOrDomain</span></span>|<span data-ttu-id="ae709-190">String</span><span class="sxs-lookup"><span data-stu-id="ae709-190">String</span></span>|<span data-ttu-id="ae709-191">Grupo de logon ou domínio quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="ae709-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="ae709-192">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-193">role</span><span class="sxs-lookup"><span data-stu-id="ae709-193">role</span></span>|<span data-ttu-id="ae709-194">String</span><span class="sxs-lookup"><span data-stu-id="ae709-194">String</span></span>|<span data-ttu-id="ae709-195">Função quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="ae709-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="ae709-196">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-197">realm</span><span class="sxs-lookup"><span data-stu-id="ae709-197">realm</span></span>|<span data-ttu-id="ae709-198">String</span><span class="sxs-lookup"><span data-stu-id="ae709-198">String</span></span>|<span data-ttu-id="ae709-199">Realm quando o tipo de conexão está definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="ae709-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="ae709-200">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-201">server</span><span class="sxs-lookup"><span data-stu-id="ae709-201">server</span></span>|[<span data-ttu-id="ae709-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="ae709-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="ae709-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="ae709-203">VPN Server on the network.</span></span> <span data-ttu-id="ae709-204">Certifique-se de que os usuários finais possam acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="ae709-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="ae709-205">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-206">identificador</span><span class="sxs-lookup"><span data-stu-id="ae709-206">identifier</span></span>|<span data-ttu-id="ae709-207">String</span><span class="sxs-lookup"><span data-stu-id="ae709-207">String</span></span>|<span data-ttu-id="ae709-208">Identificador fornecido pelo fornecedor de VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="ae709-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ae709-209">Por exemplo: Cisco AnyConnect usa um identificador do formulário com.cisco.anyconnect.applevpn.plugin Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-210">customData</span><span class="sxs-lookup"><span data-stu-id="ae709-210">customData</span></span>|<span data-ttu-id="ae709-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="ae709-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="ae709-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ae709-213">Use esse campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="ae709-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="ae709-214">Entre em contato com seu fornecedor de VPN para saber como adicionar esses pares chave/valor.</span><span class="sxs-lookup"><span data-stu-id="ae709-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="ae709-215">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="ae709-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="ae709-216">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="ae709-217">customKeyValueData</span></span>|<span data-ttu-id="ae709-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ae709-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="ae709-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="ae709-220">Use esse campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="ae709-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="ae709-221">Entre em contato com seu fornecedor de VPN para saber como adicionar esses pares chave/valor.</span><span class="sxs-lookup"><span data-stu-id="ae709-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="ae709-222">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="ae709-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="ae709-223">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="ae709-224">enableSplitTunneling</span></span>|<span data-ttu-id="ae709-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae709-225">Boolean</span></span>|<span data-ttu-id="ae709-226">Envie todo o tráfego de rede por meio da VPN.</span><span class="sxs-lookup"><span data-stu-id="ae709-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="ae709-227">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ae709-228">authenticationMethod</span></span>|[<span data-ttu-id="ae709-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ae709-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="ae709-230">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="ae709-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="ae709-231">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae709-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ae709-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="ae709-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="ae709-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="ae709-233">enablePerApp</span></span>|<span data-ttu-id="ae709-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae709-234">Boolean</span></span>|<span data-ttu-id="ae709-235">Definir isso como verdadeiro cria Per-App de VPN que pode ser associada posteriormente a aplicativos que podem disparar esse conneciton VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="ae709-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="ae709-236">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="ae709-237">safariDomains</span></span>|<span data-ttu-id="ae709-238">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae709-238">String collection</span></span>|<span data-ttu-id="ae709-239">Domínios do Safari quando essa configuração vpn por aplicativo está habilitada.</span><span class="sxs-lookup"><span data-stu-id="ae709-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="ae709-240">Além dos aplicativos associados a essa VPN, os domínios do Safari especificados aqui também poderão disparar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="ae709-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="ae709-241">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="ae709-242">onDemandRules</span></span>|<span data-ttu-id="ae709-243">[Coleção vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="ae709-244">Regras Sob Demanda.</span><span class="sxs-lookup"><span data-stu-id="ae709-244">On-Demand Rules.</span></span> <span data-ttu-id="ae709-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ae709-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ae709-246">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-247">providerType</span><span class="sxs-lookup"><span data-stu-id="ae709-247">providerType</span></span>|[<span data-ttu-id="ae709-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="ae709-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="ae709-249">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ae709-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="ae709-250">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ae709-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="ae709-251">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="ae709-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="ae709-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="ae709-252">associatedDomains</span></span>|<span data-ttu-id="ae709-253">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae709-253">String collection</span></span>|<span data-ttu-id="ae709-254">Domínios Associados Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="ae709-255">excludedDomains</span></span>|<span data-ttu-id="ae709-256">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae709-256">String collection</span></span>|<span data-ttu-id="ae709-257">Domínios que são acessados por meio da Internet pública em vez de através de VPN, mesmo quando a VPN por aplicativo é ativada Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="ae709-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="ae709-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae709-259">Boolean</span></span>|<span data-ttu-id="ae709-260">Alternar para impedir que o usuário desabilite a VPN automática no aplicativo Configurações Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-261">proxyServer</span><span class="sxs-lookup"><span data-stu-id="ae709-261">proxyServer</span></span>|[<span data-ttu-id="ae709-262">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="ae709-262">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="ae709-263">Servidor Proxy.</span><span class="sxs-lookup"><span data-stu-id="ae709-263">Proxy Server.</span></span> <span data-ttu-id="ae709-264">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-264">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-265">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="ae709-265">optInToDeviceIdSharing</span></span>|<span data-ttu-id="ae709-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae709-266">Boolean</span></span>|<span data-ttu-id="ae709-267">Opt-In compartilhar a ID do dispositivo com clientes vpn de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="ae709-267">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="ae709-268">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-268">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-269">userDomain</span><span class="sxs-lookup"><span data-stu-id="ae709-269">userDomain</span></span>|<span data-ttu-id="ae709-270">String</span><span class="sxs-lookup"><span data-stu-id="ae709-270">String</span></span>|<span data-ttu-id="ae709-271">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="ae709-271">Zscaler only.</span></span> <span data-ttu-id="ae709-272">Insira um domínio estático para pré-preencher o campo de logon no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="ae709-272">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="ae709-273">Se isso for deixado em branco, o domínio do Azure Active Directory do usuário será usado.</span><span class="sxs-lookup"><span data-stu-id="ae709-273">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="ae709-274">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-274">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-275">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="ae709-275">strictEnforcement</span></span>|<span data-ttu-id="ae709-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae709-276">Boolean</span></span>|<span data-ttu-id="ae709-277">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="ae709-277">Zscaler only.</span></span> <span data-ttu-id="ae709-278">Bloqueia o tráfego de rede até que o usuário entre no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="ae709-278">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="ae709-279">"True" significa que o tráfego está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ae709-279">"True" means traffic is blocked.</span></span> <span data-ttu-id="ae709-280">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-280">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-281">cloudName</span><span class="sxs-lookup"><span data-stu-id="ae709-281">cloudName</span></span>|<span data-ttu-id="ae709-282">String</span><span class="sxs-lookup"><span data-stu-id="ae709-282">String</span></span>|<span data-ttu-id="ae709-283">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="ae709-283">Zscaler only.</span></span> <span data-ttu-id="ae709-284">Nuvem Zscaler à qual o usuário está atribuído.</span><span class="sxs-lookup"><span data-stu-id="ae709-284">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="ae709-285">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-285">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-286">excludeList</span><span class="sxs-lookup"><span data-stu-id="ae709-286">excludeList</span></span>|<span data-ttu-id="ae709-287">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae709-287">String collection</span></span>|<span data-ttu-id="ae709-288">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="ae709-288">Zscaler only.</span></span> <span data-ttu-id="ae709-289">Lista de endereços de rede que não são enviados pela nuvem Zscaler.</span><span class="sxs-lookup"><span data-stu-id="ae709-289">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="ae709-290">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-290">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-291">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="ae709-291">targetedMobileApps</span></span>|<span data-ttu-id="ae709-292">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-292">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ae709-293">Aplicativos móveis direcionados.</span><span class="sxs-lookup"><span data-stu-id="ae709-293">Targeted mobile apps.</span></span> <span data-ttu-id="ae709-294">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ae709-294">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="ae709-295">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-295">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-296">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="ae709-296">microsoftTunnelSiteId</span></span>|<span data-ttu-id="ae709-297">String</span><span class="sxs-lookup"><span data-stu-id="ae709-297">String</span></span>|<span data-ttu-id="ae709-298">ID do site de túnel da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ae709-298">Microsoft Tunnel site ID.</span></span> <span data-ttu-id="ae709-299">Herdado de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ae709-299">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="ae709-300">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="ae709-300">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="ae709-301">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="ae709-301">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="ae709-302">Parâmetros de associação de segurança filho</span><span class="sxs-lookup"><span data-stu-id="ae709-302">Child Security Association Parameters</span></span>|
|<span data-ttu-id="ae709-303">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="ae709-303">clientAuthenticationType</span></span>|[<span data-ttu-id="ae709-304">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="ae709-304">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="ae709-305">Tipo de autenticação de cliente que o cliente VPN usará.</span><span class="sxs-lookup"><span data-stu-id="ae709-305">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="ae709-306">Os valores possíveis são: `userAuthentication` e `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="ae709-306">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="ae709-307">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="ae709-307">deadPeerDetectionRate</span></span>|[<span data-ttu-id="ae709-308">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="ae709-308">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="ae709-309">Determine com que frequência verificar se uma conexão de par ainda está ativa.</span><span class="sxs-lookup"><span data-stu-id="ae709-309">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="ae709-310">.</span><span class="sxs-lookup"><span data-stu-id="ae709-310">.</span></span> <span data-ttu-id="ae709-311">Os valores possíveis são: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="ae709-311">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="ae709-312">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="ae709-312">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="ae709-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae709-313">Boolean</span></span>|<span data-ttu-id="ae709-314">Desabilitar MOBIKE</span><span class="sxs-lookup"><span data-stu-id="ae709-314">Disable MOBIKE</span></span>|
|<span data-ttu-id="ae709-315">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="ae709-315">disableRedirect</span></span>|<span data-ttu-id="ae709-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae709-316">Boolean</span></span>|<span data-ttu-id="ae709-317">Desabilitar Redirecionamento</span><span class="sxs-lookup"><span data-stu-id="ae709-317">Disable Redirect</span></span>|
|<span data-ttu-id="ae709-318">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="ae709-318">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="ae709-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae709-319">Boolean</span></span>|<span data-ttu-id="ae709-320">Permite uma verificação de revogação de melhor esforço; tempos tempos de resposta do servidor não causarão falha</span><span class="sxs-lookup"><span data-stu-id="ae709-320">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="ae709-321">enableEAP</span><span class="sxs-lookup"><span data-stu-id="ae709-321">enableEAP</span></span>|<span data-ttu-id="ae709-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae709-322">Boolean</span></span>|<span data-ttu-id="ae709-323">Habilita a autenticação somente EAP</span><span class="sxs-lookup"><span data-stu-id="ae709-323">Enables EAP only authentication</span></span>|
|<span data-ttu-id="ae709-324">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="ae709-324">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="ae709-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae709-325">Boolean</span></span>|<span data-ttu-id="ae709-326">Habilitar PFS (Sigilo Direto).</span><span class="sxs-lookup"><span data-stu-id="ae709-326">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="ae709-327">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="ae709-327">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="ae709-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae709-328">Boolean</span></span>|<span data-ttu-id="ae709-329">Habilitar o uso de atributos de sub-rede internos.</span><span class="sxs-lookup"><span data-stu-id="ae709-329">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="ae709-330">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="ae709-330">localIdentifier</span></span>|[<span data-ttu-id="ae709-331">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="ae709-331">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="ae709-332">Método de identificar o cliente que está tentando se conectar via VPN.</span><span class="sxs-lookup"><span data-stu-id="ae709-332">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="ae709-333">.</span><span class="sxs-lookup"><span data-stu-id="ae709-333">.</span></span> <span data-ttu-id="ae709-334">Os valores possíveis são: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="ae709-334">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="ae709-335">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="ae709-335">remoteIdentifier</span></span>|<span data-ttu-id="ae709-336">String</span><span class="sxs-lookup"><span data-stu-id="ae709-336">String</span></span>|<span data-ttu-id="ae709-337">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="ae709-337">Address of the IKEv2 server.</span></span> <span data-ttu-id="ae709-338">Deve ser um FQDN, UserFQDN, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="ae709-338">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="ae709-339">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="ae709-339">securityAssociationParameters</span></span>|[<span data-ttu-id="ae709-340">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="ae709-340">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="ae709-341">Parâmetros de associação de segurança</span><span class="sxs-lookup"><span data-stu-id="ae709-341">Security Association Parameters</span></span>|
|<span data-ttu-id="ae709-342">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="ae709-342">serverCertificateCommonName</span></span>|<span data-ttu-id="ae709-343">String</span><span class="sxs-lookup"><span data-stu-id="ae709-343">String</span></span>|<span data-ttu-id="ae709-344">Nome comum do Certificado do Servidor IKEv2 usado na Autenticação do Servidor</span><span class="sxs-lookup"><span data-stu-id="ae709-344">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="ae709-345">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="ae709-345">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="ae709-346">String</span><span class="sxs-lookup"><span data-stu-id="ae709-346">String</span></span>|<span data-ttu-id="ae709-347">Nome comum do emissor do Certificado do Servidor IKEv2 usado na Autenticação</span><span class="sxs-lookup"><span data-stu-id="ae709-347">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="ae709-348">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="ae709-348">serverCertificateType</span></span>|[<span data-ttu-id="ae709-349">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="ae709-349">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="ae709-350">O tipo de certificado que o servidor VPN apresentará ao cliente VPN para autenticação.</span><span class="sxs-lookup"><span data-stu-id="ae709-350">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="ae709-351">Os valores possíveis são: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="ae709-351">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="ae709-352">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="ae709-352">sharedSecret</span></span>|<span data-ttu-id="ae709-353">String</span><span class="sxs-lookup"><span data-stu-id="ae709-353">String</span></span>|<span data-ttu-id="ae709-354">Usado quando a Autenticação Secreta Compartilhada é selecionada</span><span class="sxs-lookup"><span data-stu-id="ae709-354">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="ae709-355">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="ae709-355">tlsMaximumVersion</span></span>|<span data-ttu-id="ae709-356">String</span><span class="sxs-lookup"><span data-stu-id="ae709-356">String</span></span>|<span data-ttu-id="ae709-357">A versão TLS máxima a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="ae709-357">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="ae709-358">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="ae709-358">tlsMinimumVersion</span></span>|<span data-ttu-id="ae709-359">String</span><span class="sxs-lookup"><span data-stu-id="ae709-359">String</span></span>|<span data-ttu-id="ae709-360">A versão mínima do TLS a ser usada com a autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="ae709-360">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="ae709-361">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="ae709-361">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="ae709-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae709-362">Boolean</span></span>|<span data-ttu-id="ae709-363">Permite o uso de parâmetros de associação de segurança definindo todos os parâmetros para o padrão do dispositivo, a menos que especificado explicitamente.</span><span class="sxs-lookup"><span data-stu-id="ae709-363">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="ae709-364">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="ae709-364">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="ae709-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae709-365">Boolean</span></span>|<span data-ttu-id="ae709-366">Permite o uso de parâmetros de associação de segurança filho definindo todos os parâmetros para o padrão do dispositivo, a menos que especificado explicitamente.</span><span class="sxs-lookup"><span data-stu-id="ae709-366">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="ae709-367">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae709-367">alwaysOnConfiguration</span></span>|[<span data-ttu-id="ae709-368">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae709-368">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="ae709-369">Configuração AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="ae709-369">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="ae709-370">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="ae709-370">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="ae709-371">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae709-371">Boolean</span></span>|<span data-ttu-id="ae709-372">Determina se a VPN Always On está habilitada</span><span class="sxs-lookup"><span data-stu-id="ae709-372">Determines if Always on VPN is enabled</span></span>|
|<span data-ttu-id="ae709-373">mtuSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="ae709-373">mtuSizeInBytes</span></span>|<span data-ttu-id="ae709-374">Int32</span><span class="sxs-lookup"><span data-stu-id="ae709-374">Int32</span></span>|<span data-ttu-id="ae709-375">Unidade de transmissão máxima.</span><span class="sxs-lookup"><span data-stu-id="ae709-375">Maximum transmission unit.</span></span> <span data-ttu-id="ae709-376">Valores válidos de 1280 a 1400</span><span class="sxs-lookup"><span data-stu-id="ae709-376">Valid values 1280 to 1400</span></span>|



## <a name="response"></a><span data-ttu-id="ae709-377">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae709-377">Response</span></span>
<span data-ttu-id="ae709-378">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae709-378">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae709-379">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae709-379">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae709-380">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae709-380">Request</span></span>
<span data-ttu-id="ae709-381">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae709-381">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 5492

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
  "associatedDomains": [
    "Associated Domains value"
  ],
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

### <a name="response"></a><span data-ttu-id="ae709-382">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae709-382">Response</span></span>
<span data-ttu-id="ae709-p142">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ae709-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5664

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
  "associatedDomains": [
    "Associated Domains value"
  ],
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




