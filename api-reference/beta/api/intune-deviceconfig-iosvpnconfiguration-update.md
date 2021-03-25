---
title: Atualizar iosVpnConfiguration
description: Atualize as propriedades de um objeto iosVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3509ffb3c401f187d935333418e47e3d91ec3c59
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151309"
---
# <a name="update-iosvpnconfiguration"></a><span data-ttu-id="565ad-103">Atualizar iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="565ad-103">Update iosVpnConfiguration</span></span>

<span data-ttu-id="565ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="565ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="565ad-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="565ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="565ad-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="565ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="565ad-107">Atualize as propriedades de um [objeto iosVpnConfiguration.](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-107">Update the properties of a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="565ad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="565ad-108">Prerequisites</span></span>
<span data-ttu-id="565ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="565ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="565ad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="565ad-111">Permission type</span></span>|<span data-ttu-id="565ad-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="565ad-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="565ad-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="565ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="565ad-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="565ad-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="565ad-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="565ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="565ad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="565ad-116">Not supported.</span></span>|
|<span data-ttu-id="565ad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="565ad-117">Application</span></span>|<span data-ttu-id="565ad-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="565ad-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="565ad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="565ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="565ad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="565ad-120">Request headers</span></span>
|<span data-ttu-id="565ad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="565ad-121">Header</span></span>|<span data-ttu-id="565ad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="565ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="565ad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="565ad-123">Authorization</span></span>|<span data-ttu-id="565ad-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="565ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="565ad-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="565ad-125">Accept</span></span>|<span data-ttu-id="565ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="565ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="565ad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="565ad-127">Request body</span></span>
<span data-ttu-id="565ad-128">No corpo da solicitação, fornece uma representação JSON para o [objeto iosVpnConfiguration.](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-128">In the request body, supply a JSON representation for the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="565ad-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="565ad-129">The following table shows the properties that are required when you create the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span>

|<span data-ttu-id="565ad-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="565ad-130">Property</span></span>|<span data-ttu-id="565ad-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="565ad-131">Type</span></span>|<span data-ttu-id="565ad-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="565ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="565ad-133">id</span><span class="sxs-lookup"><span data-stu-id="565ad-133">id</span></span>|<span data-ttu-id="565ad-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ad-134">String</span></span>|<span data-ttu-id="565ad-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="565ad-135">Key of the entity.</span></span> <span data-ttu-id="565ad-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="565ad-137">lastModifiedDateTime</span></span>|<span data-ttu-id="565ad-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="565ad-138">DateTimeOffset</span></span>|<span data-ttu-id="565ad-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="565ad-139">DateTime the object was last modified.</span></span> <span data-ttu-id="565ad-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="565ad-141">roleScopeTagIds</span></span>|<span data-ttu-id="565ad-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ad-142">String collection</span></span>|<span data-ttu-id="565ad-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="565ad-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="565ad-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="565ad-145">supportsScopeTags</span></span>|<span data-ttu-id="565ad-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="565ad-146">Boolean</span></span>|<span data-ttu-id="565ad-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="565ad-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="565ad-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="565ad-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="565ad-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="565ad-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="565ad-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="565ad-150">This property is read-only.</span></span> <span data-ttu-id="565ad-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="565ad-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="565ad-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="565ad-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="565ad-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="565ad-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="565ad-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="565ad-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="565ad-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="565ad-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="565ad-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="565ad-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="565ad-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="565ad-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="565ad-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="565ad-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="565ad-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="565ad-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="565ad-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="565ad-164">createdDateTime</span></span>|<span data-ttu-id="565ad-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="565ad-165">DateTimeOffset</span></span>|<span data-ttu-id="565ad-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="565ad-166">DateTime the object was created.</span></span> <span data-ttu-id="565ad-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-168">descrição</span><span class="sxs-lookup"><span data-stu-id="565ad-168">description</span></span>|<span data-ttu-id="565ad-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ad-169">String</span></span>|<span data-ttu-id="565ad-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="565ad-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="565ad-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-172">displayName</span><span class="sxs-lookup"><span data-stu-id="565ad-172">displayName</span></span>|<span data-ttu-id="565ad-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ad-173">String</span></span>|<span data-ttu-id="565ad-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="565ad-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="565ad-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-176">versão</span><span class="sxs-lookup"><span data-stu-id="565ad-176">version</span></span>|<span data-ttu-id="565ad-177">Int32</span><span class="sxs-lookup"><span data-stu-id="565ad-177">Int32</span></span>|<span data-ttu-id="565ad-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="565ad-178">Version of the device configuration.</span></span> <span data-ttu-id="565ad-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="565ad-180">connectionName</span></span>|<span data-ttu-id="565ad-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ad-181">String</span></span>|<span data-ttu-id="565ad-182">Nome da conexão exibido ao usuário.</span><span class="sxs-lookup"><span data-stu-id="565ad-182">Connection name displayed to the user.</span></span> <span data-ttu-id="565ad-183">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="565ad-184">connectionType</span></span>|[<span data-ttu-id="565ad-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="565ad-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="565ad-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="565ad-186">Connection type.</span></span> <span data-ttu-id="565ad-187">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="565ad-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="565ad-188">Os valores possíveis são: `ciscoAnyConnect` , , , , , , , , , `pulseSecure` , , , , `f5EdgeClient` , , , `dellSonicWallMobileConnect` , `checkPointCapsuleVpn` `customVpn` , `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` . `netMotionMobility` `microsoftProtect`</span><span class="sxs-lookup"><span data-stu-id="565ad-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="565ad-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="565ad-189">loginGroupOrDomain</span></span>|<span data-ttu-id="565ad-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ad-190">String</span></span>|<span data-ttu-id="565ad-191">Grupo de logon ou domínio quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="565ad-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="565ad-192">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-193">role</span><span class="sxs-lookup"><span data-stu-id="565ad-193">role</span></span>|<span data-ttu-id="565ad-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ad-194">String</span></span>|<span data-ttu-id="565ad-195">Função quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="565ad-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="565ad-196">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-197">realm</span><span class="sxs-lookup"><span data-stu-id="565ad-197">realm</span></span>|<span data-ttu-id="565ad-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ad-198">String</span></span>|<span data-ttu-id="565ad-199">Realm quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="565ad-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="565ad-200">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-201">server</span><span class="sxs-lookup"><span data-stu-id="565ad-201">server</span></span>|[<span data-ttu-id="565ad-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="565ad-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="565ad-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="565ad-203">VPN Server on the network.</span></span> <span data-ttu-id="565ad-204">Certifique-se de que os usuários finais possam acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="565ad-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="565ad-205">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-206">identificador</span><span class="sxs-lookup"><span data-stu-id="565ad-206">identifier</span></span>|<span data-ttu-id="565ad-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ad-207">String</span></span>|<span data-ttu-id="565ad-208">Identificador fornecido pelo fornecedor vpn quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="565ad-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="565ad-209">Por exemplo: Cisco AnyConnect usa um identificador do formulário com.cisco.anyconnect.applevpn.plugin Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-210">customData</span><span class="sxs-lookup"><span data-stu-id="565ad-210">customData</span></span>|<span data-ttu-id="565ad-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="565ad-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="565ad-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="565ad-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="565ad-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="565ad-214">Entre em contato com seu fornecedor vpn para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="565ad-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="565ad-215">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="565ad-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="565ad-216">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="565ad-217">customKeyValueData</span></span>|<span data-ttu-id="565ad-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="565ad-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="565ad-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="565ad-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="565ad-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="565ad-221">Entre em contato com seu fornecedor vpn para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="565ad-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="565ad-222">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="565ad-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="565ad-223">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="565ad-224">enableSplitTunneling</span></span>|<span data-ttu-id="565ad-225">Booleano</span><span class="sxs-lookup"><span data-stu-id="565ad-225">Boolean</span></span>|<span data-ttu-id="565ad-226">Envie todo o tráfego de rede por meio de VPN.</span><span class="sxs-lookup"><span data-stu-id="565ad-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="565ad-227">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="565ad-228">authenticationMethod</span></span>|[<span data-ttu-id="565ad-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="565ad-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="565ad-230">Método de autenticação para essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="565ad-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="565ad-231">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="565ad-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="565ad-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="565ad-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="565ad-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="565ad-233">enablePerApp</span></span>|<span data-ttu-id="565ad-234">Booleano</span><span class="sxs-lookup"><span data-stu-id="565ad-234">Boolean</span></span>|<span data-ttu-id="565ad-235">Definir isso como Per-App true cria uma carga VPN que pode ser associada posteriormente a Aplicativos que podem disparar esse conneciton VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="565ad-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="565ad-236">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="565ad-237">safariDomains</span></span>|<span data-ttu-id="565ad-238">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ad-238">String collection</span></span>|<span data-ttu-id="565ad-239">Domínios safari quando essa configuração VPN por aplicativo está habilitada.</span><span class="sxs-lookup"><span data-stu-id="565ad-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="565ad-240">Além dos aplicativos associados a essa VPN, os domínios do Safari especificados aqui também poderão disparar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="565ad-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="565ad-241">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="565ad-242">onDemandRules</span></span>|<span data-ttu-id="565ad-243">[Coleção vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="565ad-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="565ad-244">On-Demand Rules.</span></span> <span data-ttu-id="565ad-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="565ad-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="565ad-246">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-247">providerType</span><span class="sxs-lookup"><span data-stu-id="565ad-247">providerType</span></span>|[<span data-ttu-id="565ad-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="565ad-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="565ad-249">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="565ad-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="565ad-250">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="565ad-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="565ad-251">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="565ad-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="565ad-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="565ad-252">associatedDomains</span></span>|<span data-ttu-id="565ad-253">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ad-253">String collection</span></span>|<span data-ttu-id="565ad-254">Domínios associados herdados de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="565ad-255">excludedDomains</span></span>|<span data-ttu-id="565ad-256">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ad-256">String collection</span></span>|<span data-ttu-id="565ad-257">Domínios acessados pela Internet pública em vez de por meio de VPN, mesmo quando a VPN por aplicativo é ativada Herdada de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="565ad-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="565ad-259">Booleano</span><span class="sxs-lookup"><span data-stu-id="565ad-259">Boolean</span></span>|<span data-ttu-id="565ad-260">Alternar para impedir que o usuário desabilite a VPN automática no aplicativo Configurações Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-261">proxyServer</span><span class="sxs-lookup"><span data-stu-id="565ad-261">proxyServer</span></span>|[<span data-ttu-id="565ad-262">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="565ad-262">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="565ad-263">Servidor Proxy.</span><span class="sxs-lookup"><span data-stu-id="565ad-263">Proxy Server.</span></span> <span data-ttu-id="565ad-264">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-264">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-265">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="565ad-265">optInToDeviceIdSharing</span></span>|<span data-ttu-id="565ad-266">Booleano</span><span class="sxs-lookup"><span data-stu-id="565ad-266">Boolean</span></span>|<span data-ttu-id="565ad-267">Opt-In compartilhar a ID do dispositivo para clientes vpn de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="565ad-267">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="565ad-268">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-268">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="565ad-269">userDomain</span><span class="sxs-lookup"><span data-stu-id="565ad-269">userDomain</span></span>|<span data-ttu-id="565ad-270">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ad-270">String</span></span>|<span data-ttu-id="565ad-271">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="565ad-271">Zscaler only.</span></span> <span data-ttu-id="565ad-272">Insira um domínio estático para preencher previamente o campo de logon com no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="565ad-272">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="565ad-273">Se isso for deixado em branco, o domínio do Azure Active Directory do usuário será usado em vez disso.</span><span class="sxs-lookup"><span data-stu-id="565ad-273">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="565ad-274">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="565ad-274">strictEnforcement</span></span>|<span data-ttu-id="565ad-275">Booleano</span><span class="sxs-lookup"><span data-stu-id="565ad-275">Boolean</span></span>|<span data-ttu-id="565ad-276">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="565ad-276">Zscaler only.</span></span> <span data-ttu-id="565ad-277">Bloqueia o tráfego de rede até que o usuário entre no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="565ad-277">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="565ad-278">"True" significa que o tráfego está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="565ad-278">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="565ad-279">cloudName</span><span class="sxs-lookup"><span data-stu-id="565ad-279">cloudName</span></span>|<span data-ttu-id="565ad-280">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ad-280">String</span></span>|<span data-ttu-id="565ad-281">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="565ad-281">Zscaler only.</span></span> <span data-ttu-id="565ad-282">Nuvem Zscaler à qual o usuário é atribuído.</span><span class="sxs-lookup"><span data-stu-id="565ad-282">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="565ad-283">excludeList</span><span class="sxs-lookup"><span data-stu-id="565ad-283">excludeList</span></span>|<span data-ttu-id="565ad-284">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ad-284">String collection</span></span>|<span data-ttu-id="565ad-285">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="565ad-285">Zscaler only.</span></span> <span data-ttu-id="565ad-286">Lista de endereços de rede que não são enviados pela nuvem Zscaler.</span><span class="sxs-lookup"><span data-stu-id="565ad-286">List of network addresses which are not sent through the Zscaler cloud.</span></span>|
|<span data-ttu-id="565ad-287">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="565ad-287">targetedMobileApps</span></span>|<span data-ttu-id="565ad-288">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="565ad-288">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="565ad-289">Aplicativos móveis direcionados.</span><span class="sxs-lookup"><span data-stu-id="565ad-289">Targeted mobile apps.</span></span> <span data-ttu-id="565ad-290">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="565ad-290">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="565ad-291">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="565ad-291">microsoftTunnelSiteId</span></span>|<span data-ttu-id="565ad-292">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="565ad-292">String</span></span>|<span data-ttu-id="565ad-293">ID do site do Túnel da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="565ad-293">Microsoft Tunnel site ID.</span></span>|



## <a name="response"></a><span data-ttu-id="565ad-294">Resposta</span><span class="sxs-lookup"><span data-stu-id="565ad-294">Response</span></span>
<span data-ttu-id="565ad-295">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="565ad-295">If successful, this method returns a `200 OK` response code and an updated [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="565ad-296">Exemplo</span><span class="sxs-lookup"><span data-stu-id="565ad-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="565ad-297">Solicitação</span><span class="sxs-lookup"><span data-stu-id="565ad-297">Request</span></span>
<span data-ttu-id="565ad-298">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="565ad-298">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3298

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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```

### <a name="response"></a><span data-ttu-id="565ad-299">Resposta</span><span class="sxs-lookup"><span data-stu-id="565ad-299">Response</span></span>
<span data-ttu-id="565ad-p135">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="565ad-p135">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3470

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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```




