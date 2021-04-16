---
title: Atualizar iosikEv2VpnConfiguration
description: Atualize as propriedades de um objeto iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 68893c36fc8fdf760c166f32e199f66130bb4edc
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867998"
---
# <a name="update-iosikev2vpnconfiguration"></a><span data-ttu-id="b44f0-103">Atualizar iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b44f0-103">Update iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="b44f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b44f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b44f0-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b44f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b44f0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b44f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b44f0-107">Atualize as propriedades de [um objeto iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-107">Update the properties of a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b44f0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b44f0-108">Prerequisites</span></span>
<span data-ttu-id="b44f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b44f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b44f0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b44f0-111">Permission type</span></span>|<span data-ttu-id="b44f0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b44f0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b44f0-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b44f0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b44f0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b44f0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b44f0-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b44f0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b44f0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b44f0-116">Not supported.</span></span>|
|<span data-ttu-id="b44f0-117">Application</span><span class="sxs-lookup"><span data-stu-id="b44f0-117">Application</span></span>|<span data-ttu-id="b44f0-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b44f0-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b44f0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b44f0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b44f0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b44f0-120">Request headers</span></span>
|<span data-ttu-id="b44f0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b44f0-121">Header</span></span>|<span data-ttu-id="b44f0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b44f0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b44f0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b44f0-123">Authorization</span></span>|<span data-ttu-id="b44f0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b44f0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b44f0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b44f0-125">Accept</span></span>|<span data-ttu-id="b44f0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b44f0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b44f0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b44f0-127">Request body</span></span>
<span data-ttu-id="b44f0-128">No corpo da solicitação, fornece uma representação JSON para o [objeto iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-128">In the request body, supply a JSON representation for the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

<span data-ttu-id="b44f0-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b44f0-129">The following table shows the properties that are required when you create the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md).</span></span>

|<span data-ttu-id="b44f0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b44f0-130">Property</span></span>|<span data-ttu-id="b44f0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b44f0-131">Type</span></span>|<span data-ttu-id="b44f0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b44f0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b44f0-133">id</span><span class="sxs-lookup"><span data-stu-id="b44f0-133">id</span></span>|<span data-ttu-id="b44f0-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-134">String</span></span>|<span data-ttu-id="b44f0-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b44f0-135">Key of the entity.</span></span> <span data-ttu-id="b44f0-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b44f0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b44f0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b44f0-138">DateTimeOffset</span></span>|<span data-ttu-id="b44f0-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b44f0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b44f0-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b44f0-141">roleScopeTagIds</span></span>|<span data-ttu-id="b44f0-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b44f0-142">String collection</span></span>|<span data-ttu-id="b44f0-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="b44f0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b44f0-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b44f0-145">supportsScopeTags</span></span>|<span data-ttu-id="b44f0-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44f0-146">Boolean</span></span>|<span data-ttu-id="b44f0-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b44f0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b44f0-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b44f0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b44f0-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b44f0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b44f0-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b44f0-150">This property is read-only.</span></span> <span data-ttu-id="b44f0-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b44f0-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b44f0-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b44f0-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b44f0-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="b44f0-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b44f0-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b44f0-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b44f0-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b44f0-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b44f0-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="b44f0-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b44f0-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b44f0-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b44f0-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b44f0-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b44f0-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="b44f0-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b44f0-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b44f0-164">createdDateTime</span></span>|<span data-ttu-id="b44f0-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b44f0-165">DateTimeOffset</span></span>|<span data-ttu-id="b44f0-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b44f0-166">DateTime the object was created.</span></span> <span data-ttu-id="b44f0-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-168">description</span><span class="sxs-lookup"><span data-stu-id="b44f0-168">description</span></span>|<span data-ttu-id="b44f0-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-169">String</span></span>|<span data-ttu-id="b44f0-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b44f0-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b44f0-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b44f0-172">displayName</span></span>|<span data-ttu-id="b44f0-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-173">String</span></span>|<span data-ttu-id="b44f0-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b44f0-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b44f0-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-176">versão</span><span class="sxs-lookup"><span data-stu-id="b44f0-176">version</span></span>|<span data-ttu-id="b44f0-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b44f0-177">Int32</span></span>|<span data-ttu-id="b44f0-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b44f0-178">Version of the device configuration.</span></span> <span data-ttu-id="b44f0-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="b44f0-180">connectionName</span></span>|<span data-ttu-id="b44f0-181">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-181">String</span></span>|<span data-ttu-id="b44f0-182">Nome da conexão exibido ao usuário.</span><span class="sxs-lookup"><span data-stu-id="b44f0-182">Connection name displayed to the user.</span></span> <span data-ttu-id="b44f0-183">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="b44f0-184">connectionType</span></span>|[<span data-ttu-id="b44f0-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="b44f0-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="b44f0-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="b44f0-186">Connection type.</span></span> <span data-ttu-id="b44f0-187">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b44f0-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="b44f0-188">Os valores possíveis são: `ciscoAnyConnect` , , , , , , , , , `pulseSecure` , , , , `f5EdgeClient` , , , `dellSonicWallMobileConnect` , `checkPointCapsuleVpn` `customVpn` , `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` . `netMotionMobility` `microsoftProtect`</span><span class="sxs-lookup"><span data-stu-id="b44f0-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="b44f0-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="b44f0-189">loginGroupOrDomain</span></span>|<span data-ttu-id="b44f0-190">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-190">String</span></span>|<span data-ttu-id="b44f0-191">Grupo de logon ou domínio quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="b44f0-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="b44f0-192">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-193">role</span><span class="sxs-lookup"><span data-stu-id="b44f0-193">role</span></span>|<span data-ttu-id="b44f0-194">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-194">String</span></span>|<span data-ttu-id="b44f0-195">Função quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="b44f0-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="b44f0-196">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-197">realm</span><span class="sxs-lookup"><span data-stu-id="b44f0-197">realm</span></span>|<span data-ttu-id="b44f0-198">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-198">String</span></span>|<span data-ttu-id="b44f0-199">Realm quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="b44f0-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="b44f0-200">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-201">server</span><span class="sxs-lookup"><span data-stu-id="b44f0-201">server</span></span>|[<span data-ttu-id="b44f0-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="b44f0-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="b44f0-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="b44f0-203">VPN Server on the network.</span></span> <span data-ttu-id="b44f0-204">Certifique-se de que os usuários finais possam acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="b44f0-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="b44f0-205">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-206">identificador</span><span class="sxs-lookup"><span data-stu-id="b44f0-206">identifier</span></span>|<span data-ttu-id="b44f0-207">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-207">String</span></span>|<span data-ttu-id="b44f0-208">Identificador fornecido pelo fornecedor vpn quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="b44f0-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b44f0-209">Por exemplo: Cisco AnyConnect usa um identificador do formulário com.cisco.anyconnect.applevpn.plugin Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-210">customData</span><span class="sxs-lookup"><span data-stu-id="b44f0-210">customData</span></span>|<span data-ttu-id="b44f0-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="b44f0-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="b44f0-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b44f0-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="b44f0-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="b44f0-214">Entre em contato com seu fornecedor vpn para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="b44f0-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="b44f0-215">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="b44f0-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="b44f0-216">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="b44f0-217">customKeyValueData</span></span>|<span data-ttu-id="b44f0-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b44f0-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="b44f0-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="b44f0-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="b44f0-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="b44f0-221">Entre em contato com seu fornecedor vpn para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="b44f0-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="b44f0-222">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="b44f0-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="b44f0-223">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="b44f0-224">enableSplitTunneling</span></span>|<span data-ttu-id="b44f0-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44f0-225">Boolean</span></span>|<span data-ttu-id="b44f0-226">Envie todo o tráfego de rede por meio de VPN.</span><span class="sxs-lookup"><span data-stu-id="b44f0-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="b44f0-227">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b44f0-228">authenticationMethod</span></span>|[<span data-ttu-id="b44f0-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b44f0-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="b44f0-230">Método de autenticação para essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="b44f0-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="b44f0-231">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b44f0-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="b44f0-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="b44f0-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="b44f0-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="b44f0-233">enablePerApp</span></span>|<span data-ttu-id="b44f0-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44f0-234">Boolean</span></span>|<span data-ttu-id="b44f0-235">Definir isso como Per-App true cria uma carga VPN que pode ser associada posteriormente a Aplicativos que podem disparar esse conneciton VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="b44f0-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="b44f0-236">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="b44f0-237">safariDomains</span></span>|<span data-ttu-id="b44f0-238">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b44f0-238">String collection</span></span>|<span data-ttu-id="b44f0-239">Domínios safari quando essa configuração VPN por aplicativo está habilitada.</span><span class="sxs-lookup"><span data-stu-id="b44f0-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="b44f0-240">Além dos aplicativos associados a essa VPN, os domínios do Safari especificados aqui também poderão disparar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="b44f0-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="b44f0-241">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="b44f0-242">onDemandRules</span></span>|<span data-ttu-id="b44f0-243">[Coleção vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="b44f0-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="b44f0-244">On-Demand Rules.</span></span> <span data-ttu-id="b44f0-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b44f0-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b44f0-246">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-247">providerType</span><span class="sxs-lookup"><span data-stu-id="b44f0-247">providerType</span></span>|[<span data-ttu-id="b44f0-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="b44f0-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="b44f0-249">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b44f0-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="b44f0-250">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b44f0-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="b44f0-251">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="b44f0-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="b44f0-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="b44f0-252">associatedDomains</span></span>|<span data-ttu-id="b44f0-253">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b44f0-253">String collection</span></span>|<span data-ttu-id="b44f0-254">Domínios associados herdados de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="b44f0-255">excludedDomains</span></span>|<span data-ttu-id="b44f0-256">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b44f0-256">String collection</span></span>|<span data-ttu-id="b44f0-257">Domínios acessados pela Internet pública em vez de por meio de VPN, mesmo quando a VPN por aplicativo é ativada Herdada de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="b44f0-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="b44f0-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44f0-259">Boolean</span></span>|<span data-ttu-id="b44f0-260">Alternar para impedir que o usuário desabilite a VPN automática no aplicativo Configurações Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-261">disconnectOnIdle</span><span class="sxs-lookup"><span data-stu-id="b44f0-261">disconnectOnIdle</span></span>|<span data-ttu-id="b44f0-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44f0-262">Boolean</span></span>|<span data-ttu-id="b44f0-263">Se deve desconectar após ociosos de conexão sob demanda Herdados de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-263">Whether to disconnect after on-demand connection idles Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-264">disconnectOnIdleTimerInSeconds</span><span class="sxs-lookup"><span data-stu-id="b44f0-264">disconnectOnIdleTimerInSeconds</span></span>|<span data-ttu-id="b44f0-265">Int32</span><span class="sxs-lookup"><span data-stu-id="b44f0-265">Int32</span></span>|<span data-ttu-id="b44f0-266">O tempo de espera em segundos antes de desconectar uma conexão sob demanda.</span><span class="sxs-lookup"><span data-stu-id="b44f0-266">The length of time in seconds to wait before disconnecting an on-demand connection.</span></span> <span data-ttu-id="b44f0-267">Valores válidos de 0 a 65535 Herdados [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-267">Valid values 0 to 65535 Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-268">proxyServer</span><span class="sxs-lookup"><span data-stu-id="b44f0-268">proxyServer</span></span>|[<span data-ttu-id="b44f0-269">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="b44f0-269">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="b44f0-270">Servidor Proxy.</span><span class="sxs-lookup"><span data-stu-id="b44f0-270">Proxy Server.</span></span> <span data-ttu-id="b44f0-271">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-271">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-272">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="b44f0-272">optInToDeviceIdSharing</span></span>|<span data-ttu-id="b44f0-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44f0-273">Boolean</span></span>|<span data-ttu-id="b44f0-274">Opt-In compartilhar a ID do dispositivo para clientes vpn de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="b44f0-274">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="b44f0-275">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-275">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-276">userDomain</span><span class="sxs-lookup"><span data-stu-id="b44f0-276">userDomain</span></span>|<span data-ttu-id="b44f0-277">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-277">String</span></span>|<span data-ttu-id="b44f0-278">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="b44f0-278">Zscaler only.</span></span> <span data-ttu-id="b44f0-279">Insira um domínio estático para preencher previamente o campo de logon com no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="b44f0-279">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="b44f0-280">Se isso for deixado em branco, o domínio do Azure Active Directory do usuário será usado em vez disso.</span><span class="sxs-lookup"><span data-stu-id="b44f0-280">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="b44f0-281">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-281">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-282">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="b44f0-282">strictEnforcement</span></span>|<span data-ttu-id="b44f0-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44f0-283">Boolean</span></span>|<span data-ttu-id="b44f0-284">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="b44f0-284">Zscaler only.</span></span> <span data-ttu-id="b44f0-285">Bloqueia o tráfego de rede até que o usuário entre no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="b44f0-285">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="b44f0-286">"True" significa que o tráfego está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b44f0-286">"True" means traffic is blocked.</span></span> <span data-ttu-id="b44f0-287">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-287">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-288">cloudName</span><span class="sxs-lookup"><span data-stu-id="b44f0-288">cloudName</span></span>|<span data-ttu-id="b44f0-289">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-289">String</span></span>|<span data-ttu-id="b44f0-290">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="b44f0-290">Zscaler only.</span></span> <span data-ttu-id="b44f0-291">Nuvem Zscaler à qual o usuário é atribuído.</span><span class="sxs-lookup"><span data-stu-id="b44f0-291">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="b44f0-292">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-292">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-293">excludeList</span><span class="sxs-lookup"><span data-stu-id="b44f0-293">excludeList</span></span>|<span data-ttu-id="b44f0-294">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b44f0-294">String collection</span></span>|<span data-ttu-id="b44f0-295">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="b44f0-295">Zscaler only.</span></span> <span data-ttu-id="b44f0-296">Lista de endereços de rede que não são enviados pela nuvem Zscaler.</span><span class="sxs-lookup"><span data-stu-id="b44f0-296">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="b44f0-297">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-297">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-298">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="b44f0-298">targetedMobileApps</span></span>|<span data-ttu-id="b44f0-299">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-299">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b44f0-300">Aplicativos móveis direcionados.</span><span class="sxs-lookup"><span data-stu-id="b44f0-300">Targeted mobile apps.</span></span> <span data-ttu-id="b44f0-301">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b44f0-301">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b44f0-302">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-302">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-303">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="b44f0-303">microsoftTunnelSiteId</span></span>|<span data-ttu-id="b44f0-304">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-304">String</span></span>|<span data-ttu-id="b44f0-305">ID do site do Túnel da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b44f0-305">Microsoft Tunnel site ID.</span></span> <span data-ttu-id="b44f0-306">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b44f0-306">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b44f0-307">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="b44f0-307">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="b44f0-308">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="b44f0-308">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="b44f0-309">Parâmetros de associação de segurança filho</span><span class="sxs-lookup"><span data-stu-id="b44f0-309">Child Security Association Parameters</span></span>|
|<span data-ttu-id="b44f0-310">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="b44f0-310">clientAuthenticationType</span></span>|[<span data-ttu-id="b44f0-311">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="b44f0-311">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="b44f0-312">Tipo de Autenticação de Cliente que o cliente VPN usará.</span><span class="sxs-lookup"><span data-stu-id="b44f0-312">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="b44f0-313">Os valores possíveis são: `userAuthentication` e `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="b44f0-313">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="b44f0-314">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="b44f0-314">deadPeerDetectionRate</span></span>|[<span data-ttu-id="b44f0-315">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="b44f0-315">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="b44f0-316">Determine com que frequência verificar se uma conexão de par ainda está ativa.</span><span class="sxs-lookup"><span data-stu-id="b44f0-316">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="b44f0-317">.</span><span class="sxs-lookup"><span data-stu-id="b44f0-317">.</span></span> <span data-ttu-id="b44f0-318">Os valores possíveis são: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="b44f0-318">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="b44f0-319">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="b44f0-319">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="b44f0-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44f0-320">Boolean</span></span>|<span data-ttu-id="b44f0-321">Desabilitar MOBIKE</span><span class="sxs-lookup"><span data-stu-id="b44f0-321">Disable MOBIKE</span></span>|
|<span data-ttu-id="b44f0-322">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="b44f0-322">disableRedirect</span></span>|<span data-ttu-id="b44f0-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44f0-323">Boolean</span></span>|<span data-ttu-id="b44f0-324">Desabilitar Redirecionamento</span><span class="sxs-lookup"><span data-stu-id="b44f0-324">Disable Redirect</span></span>|
|<span data-ttu-id="b44f0-325">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="b44f0-325">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="b44f0-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44f0-326">Boolean</span></span>|<span data-ttu-id="b44f0-327">Habilita uma verificação de revogação de melhor esforço; tempo-de-tempo de resposta do servidor não fará com que ele falhe</span><span class="sxs-lookup"><span data-stu-id="b44f0-327">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="b44f0-328">enableEAP</span><span class="sxs-lookup"><span data-stu-id="b44f0-328">enableEAP</span></span>|<span data-ttu-id="b44f0-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44f0-329">Boolean</span></span>|<span data-ttu-id="b44f0-330">Habilita a autenticação somente EAP</span><span class="sxs-lookup"><span data-stu-id="b44f0-330">Enables EAP only authentication</span></span>|
|<span data-ttu-id="b44f0-331">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="b44f0-331">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="b44f0-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44f0-332">Boolean</span></span>|<span data-ttu-id="b44f0-333">Habilitar o PFS (Segredo de Encaminhamento Perfeito).</span><span class="sxs-lookup"><span data-stu-id="b44f0-333">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="b44f0-334">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="b44f0-334">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="b44f0-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44f0-335">Boolean</span></span>|<span data-ttu-id="b44f0-336">Habilitar usar atributos de sub-rede internas.</span><span class="sxs-lookup"><span data-stu-id="b44f0-336">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="b44f0-337">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="b44f0-337">localIdentifier</span></span>|[<span data-ttu-id="b44f0-338">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="b44f0-338">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="b44f0-339">Método de identificar o cliente que está tentando se conectar via VPN.</span><span class="sxs-lookup"><span data-stu-id="b44f0-339">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="b44f0-340">.</span><span class="sxs-lookup"><span data-stu-id="b44f0-340">.</span></span> <span data-ttu-id="b44f0-341">Os valores possíveis são: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="b44f0-341">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="b44f0-342">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="b44f0-342">remoteIdentifier</span></span>|<span data-ttu-id="b44f0-343">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-343">String</span></span>|<span data-ttu-id="b44f0-344">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="b44f0-344">Address of the IKEv2 server.</span></span> <span data-ttu-id="b44f0-345">Deve ser um FQDN, UserFQDN, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="b44f0-345">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="b44f0-346">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="b44f0-346">securityAssociationParameters</span></span>|[<span data-ttu-id="b44f0-347">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="b44f0-347">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="b44f0-348">Parâmetros de Associação de Segurança</span><span class="sxs-lookup"><span data-stu-id="b44f0-348">Security Association Parameters</span></span>|
|<span data-ttu-id="b44f0-349">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="b44f0-349">serverCertificateCommonName</span></span>|<span data-ttu-id="b44f0-350">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-350">String</span></span>|<span data-ttu-id="b44f0-351">Nome comum do Certificado de Servidor IKEv2 usado na Autenticação do Servidor</span><span class="sxs-lookup"><span data-stu-id="b44f0-351">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="b44f0-352">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="b44f0-352">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="b44f0-353">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-353">String</span></span>|<span data-ttu-id="b44f0-354">Nome comum do emissor do emissor de Certificado do Servidor IKEv2 usado na Autenticação</span><span class="sxs-lookup"><span data-stu-id="b44f0-354">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="b44f0-355">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="b44f0-355">serverCertificateType</span></span>|[<span data-ttu-id="b44f0-356">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="b44f0-356">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="b44f0-357">O tipo de certificado que o servidor VPN apresentará ao cliente VPN para autenticação.</span><span class="sxs-lookup"><span data-stu-id="b44f0-357">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="b44f0-358">Os valores possíveis são: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="b44f0-358">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="b44f0-359">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="b44f0-359">sharedSecret</span></span>|<span data-ttu-id="b44f0-360">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-360">String</span></span>|<span data-ttu-id="b44f0-361">Usado quando a Autenticação Secreta Compartilhada está selecionada</span><span class="sxs-lookup"><span data-stu-id="b44f0-361">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="b44f0-362">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="b44f0-362">tlsMaximumVersion</span></span>|<span data-ttu-id="b44f0-363">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-363">String</span></span>|<span data-ttu-id="b44f0-364">A versão TLS máxima a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="b44f0-364">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="b44f0-365">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="b44f0-365">tlsMinimumVersion</span></span>|<span data-ttu-id="b44f0-366">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="b44f0-366">String</span></span>|<span data-ttu-id="b44f0-367">A versão TLS mínima a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="b44f0-367">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="b44f0-368">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="b44f0-368">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="b44f0-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44f0-369">Boolean</span></span>|<span data-ttu-id="b44f0-370">Permite o uso de parâmetros de associação de segurança definindo todos os parâmetros para o padrão do dispositivo, a menos que especificado explicitamente.</span><span class="sxs-lookup"><span data-stu-id="b44f0-370">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="b44f0-371">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="b44f0-371">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="b44f0-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44f0-372">Boolean</span></span>|<span data-ttu-id="b44f0-373">Permite o uso de parâmetros de associação de segurança filho definindo todos os parâmetros para o padrão do dispositivo, a menos que especificado explicitamente.</span><span class="sxs-lookup"><span data-stu-id="b44f0-373">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="b44f0-374">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b44f0-374">alwaysOnConfiguration</span></span>|[<span data-ttu-id="b44f0-375">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b44f0-375">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="b44f0-376">Configuração AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="b44f0-376">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="b44f0-377">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b44f0-377">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="b44f0-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="b44f0-378">Boolean</span></span>|<span data-ttu-id="b44f0-379">Determina se a VPN Always on está habilitada</span><span class="sxs-lookup"><span data-stu-id="b44f0-379">Determines if Always on VPN is enabled</span></span>|
|<span data-ttu-id="b44f0-380">mtuSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="b44f0-380">mtuSizeInBytes</span></span>|<span data-ttu-id="b44f0-381">Int32</span><span class="sxs-lookup"><span data-stu-id="b44f0-381">Int32</span></span>|<span data-ttu-id="b44f0-382">Unidade de transmissão máxima.</span><span class="sxs-lookup"><span data-stu-id="b44f0-382">Maximum transmission unit.</span></span> <span data-ttu-id="b44f0-383">Valores válidos de 1280 a 1400</span><span class="sxs-lookup"><span data-stu-id="b44f0-383">Valid values 1280 to 1400</span></span>|



## <a name="response"></a><span data-ttu-id="b44f0-384">Resposta</span><span class="sxs-lookup"><span data-stu-id="b44f0-384">Response</span></span>
<span data-ttu-id="b44f0-385">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b44f0-385">If successful, this method returns a `200 OK` response code and an updated [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b44f0-386">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b44f0-386">Example</span></span>

### <a name="request"></a><span data-ttu-id="b44f0-387">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b44f0-387">Request</span></span>
<span data-ttu-id="b44f0-388">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b44f0-388">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 5562

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
  "disconnectOnIdle": true,
  "disconnectOnIdleTimerInSeconds": 14,
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

### <a name="response"></a><span data-ttu-id="b44f0-389">Resposta</span><span class="sxs-lookup"><span data-stu-id="b44f0-389">Response</span></span>
<span data-ttu-id="b44f0-p143">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b44f0-p143">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5734

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
  "disconnectOnIdle": true,
  "disconnectOnIdleTimerInSeconds": 14,
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




