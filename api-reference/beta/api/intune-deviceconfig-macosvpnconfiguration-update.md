---
title: Atualizar macOSVpnConfiguration
description: Atualize as propriedades de um objeto macOSVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: afb77e4976ac520bce392f19e1323cd94f4d39c8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132580"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="d8e61-103">Atualizar macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8e61-103">Update macOSVpnConfiguration</span></span>

<span data-ttu-id="d8e61-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8e61-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8e61-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d8e61-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8e61-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8e61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8e61-107">Atualize as propriedades de [um objeto macOSVpnConfiguration.](../resources/intune-deviceconfig-macosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-107">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8e61-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d8e61-108">Prerequisites</span></span>
<span data-ttu-id="d8e61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8e61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8e61-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8e61-111">Permission type</span></span>|<span data-ttu-id="d8e61-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8e61-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8e61-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8e61-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8e61-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8e61-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8e61-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8e61-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8e61-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8e61-116">Not supported.</span></span>|
|<span data-ttu-id="d8e61-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8e61-117">Application</span></span>|<span data-ttu-id="d8e61-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8e61-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8e61-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8e61-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d8e61-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8e61-120">Request headers</span></span>
|<span data-ttu-id="d8e61-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d8e61-121">Header</span></span>|<span data-ttu-id="d8e61-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d8e61-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8e61-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8e61-123">Authorization</span></span>|<span data-ttu-id="d8e61-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8e61-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8e61-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d8e61-125">Accept</span></span>|<span data-ttu-id="d8e61-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8e61-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8e61-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8e61-127">Request body</span></span>
<span data-ttu-id="d8e61-128">No corpo da solicitação, fornece uma representação JSON para o [objeto macOSVpnConfiguration.](../resources/intune-deviceconfig-macosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-128">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="d8e61-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8e61-129">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="d8e61-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8e61-130">Property</span></span>|<span data-ttu-id="d8e61-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8e61-131">Type</span></span>|<span data-ttu-id="d8e61-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8e61-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8e61-133">id</span><span class="sxs-lookup"><span data-stu-id="d8e61-133">id</span></span>|<span data-ttu-id="d8e61-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8e61-134">String</span></span>|<span data-ttu-id="d8e61-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d8e61-135">Key of the entity.</span></span> <span data-ttu-id="d8e61-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8e61-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d8e61-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8e61-138">DateTimeOffset</span></span>|<span data-ttu-id="d8e61-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d8e61-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d8e61-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d8e61-141">roleScopeTagIds</span></span>|<span data-ttu-id="d8e61-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8e61-142">String collection</span></span>|<span data-ttu-id="d8e61-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="d8e61-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d8e61-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d8e61-145">supportsScopeTags</span></span>|<span data-ttu-id="d8e61-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="d8e61-146">Boolean</span></span>|<span data-ttu-id="d8e61-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d8e61-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d8e61-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d8e61-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d8e61-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d8e61-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d8e61-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8e61-150">This property is read-only.</span></span> <span data-ttu-id="d8e61-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d8e61-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d8e61-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d8e61-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d8e61-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="d8e61-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d8e61-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d8e61-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d8e61-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d8e61-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d8e61-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="d8e61-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d8e61-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d8e61-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d8e61-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d8e61-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d8e61-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="d8e61-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d8e61-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8e61-164">createdDateTime</span></span>|<span data-ttu-id="d8e61-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8e61-165">DateTimeOffset</span></span>|<span data-ttu-id="d8e61-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d8e61-166">DateTime the object was created.</span></span> <span data-ttu-id="d8e61-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-168">descrição</span><span class="sxs-lookup"><span data-stu-id="d8e61-168">description</span></span>|<span data-ttu-id="d8e61-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8e61-169">String</span></span>|<span data-ttu-id="d8e61-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d8e61-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d8e61-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d8e61-172">displayName</span></span>|<span data-ttu-id="d8e61-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8e61-173">String</span></span>|<span data-ttu-id="d8e61-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d8e61-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d8e61-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-176">versão</span><span class="sxs-lookup"><span data-stu-id="d8e61-176">version</span></span>|<span data-ttu-id="d8e61-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d8e61-177">Int32</span></span>|<span data-ttu-id="d8e61-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d8e61-178">Version of the device configuration.</span></span> <span data-ttu-id="d8e61-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="d8e61-180">connectionName</span></span>|<span data-ttu-id="d8e61-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8e61-181">String</span></span>|<span data-ttu-id="d8e61-182">Nome da conexão exibido ao usuário.</span><span class="sxs-lookup"><span data-stu-id="d8e61-182">Connection name displayed to the user.</span></span> <span data-ttu-id="d8e61-183">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="d8e61-184">connectionType</span></span>|[<span data-ttu-id="d8e61-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="d8e61-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="d8e61-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="d8e61-186">Connection type.</span></span> <span data-ttu-id="d8e61-187">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8e61-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="d8e61-188">Os valores possíveis são: `ciscoAnyConnect` , , , , , , , , , `pulseSecure` , , , , `f5EdgeClient` , , , `dellSonicWallMobileConnect` , `checkPointCapsuleVpn` `customVpn` , `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` . `netMotionMobility` `microsoftProtect`</span><span class="sxs-lookup"><span data-stu-id="d8e61-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="d8e61-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="d8e61-189">loginGroupOrDomain</span></span>|<span data-ttu-id="d8e61-190">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8e61-190">String</span></span>|<span data-ttu-id="d8e61-191">Grupo de logon ou domínio quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="d8e61-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="d8e61-192">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-193">role</span><span class="sxs-lookup"><span data-stu-id="d8e61-193">role</span></span>|<span data-ttu-id="d8e61-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8e61-194">String</span></span>|<span data-ttu-id="d8e61-195">Função quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="d8e61-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="d8e61-196">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-197">realm</span><span class="sxs-lookup"><span data-stu-id="d8e61-197">realm</span></span>|<span data-ttu-id="d8e61-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8e61-198">String</span></span>|<span data-ttu-id="d8e61-199">Realm quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="d8e61-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="d8e61-200">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-201">server</span><span class="sxs-lookup"><span data-stu-id="d8e61-201">server</span></span>|[<span data-ttu-id="d8e61-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="d8e61-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="d8e61-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="d8e61-203">VPN Server on the network.</span></span> <span data-ttu-id="d8e61-204">Certifique-se de que os usuários finais possam acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="d8e61-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="d8e61-205">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-206">identificador</span><span class="sxs-lookup"><span data-stu-id="d8e61-206">identifier</span></span>|<span data-ttu-id="d8e61-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8e61-207">String</span></span>|<span data-ttu-id="d8e61-208">Identificador fornecido pelo fornecedor vpn quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="d8e61-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="d8e61-209">Por exemplo: Cisco AnyConnect usa um identificador do formulário com.cisco.anyconnect.applevpn.plugin Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-210">customData</span><span class="sxs-lookup"><span data-stu-id="d8e61-210">customData</span></span>|<span data-ttu-id="d8e61-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="d8e61-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="d8e61-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="d8e61-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="d8e61-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="d8e61-214">Entre em contato com seu fornecedor vpn para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="d8e61-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="d8e61-215">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="d8e61-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="d8e61-216">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="d8e61-217">customKeyValueData</span></span>|<span data-ttu-id="d8e61-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d8e61-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="d8e61-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="d8e61-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="d8e61-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="d8e61-221">Entre em contato com seu fornecedor vpn para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="d8e61-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="d8e61-222">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="d8e61-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="d8e61-223">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="d8e61-224">enableSplitTunneling</span></span>|<span data-ttu-id="d8e61-225">Booleano</span><span class="sxs-lookup"><span data-stu-id="d8e61-225">Boolean</span></span>|<span data-ttu-id="d8e61-226">Envie todo o tráfego de rede por meio de VPN.</span><span class="sxs-lookup"><span data-stu-id="d8e61-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="d8e61-227">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d8e61-228">authenticationMethod</span></span>|[<span data-ttu-id="d8e61-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d8e61-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="d8e61-230">Método de autenticação para essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="d8e61-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="d8e61-231">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8e61-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="d8e61-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="d8e61-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="d8e61-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="d8e61-233">enablePerApp</span></span>|<span data-ttu-id="d8e61-234">Booleano</span><span class="sxs-lookup"><span data-stu-id="d8e61-234">Boolean</span></span>|<span data-ttu-id="d8e61-235">Definir isso como Per-App true cria uma carga VPN que pode ser associada posteriormente a Aplicativos que podem disparar esse conneciton VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="d8e61-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="d8e61-236">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="d8e61-237">safariDomains</span></span>|<span data-ttu-id="d8e61-238">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8e61-238">String collection</span></span>|<span data-ttu-id="d8e61-239">Domínios safari quando essa configuração VPN por aplicativo está habilitada.</span><span class="sxs-lookup"><span data-stu-id="d8e61-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="d8e61-240">Além dos aplicativos associados a essa VPN, os domínios do Safari especificados aqui também poderão disparar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="d8e61-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="d8e61-241">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="d8e61-242">onDemandRules</span></span>|<span data-ttu-id="d8e61-243">[Coleção vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="d8e61-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="d8e61-244">On-Demand Rules.</span></span> <span data-ttu-id="d8e61-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d8e61-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d8e61-246">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-247">providerType</span><span class="sxs-lookup"><span data-stu-id="d8e61-247">providerType</span></span>|[<span data-ttu-id="d8e61-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="d8e61-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="d8e61-249">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d8e61-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="d8e61-250">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8e61-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="d8e61-251">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="d8e61-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="d8e61-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="d8e61-252">associatedDomains</span></span>|<span data-ttu-id="d8e61-253">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8e61-253">String collection</span></span>|<span data-ttu-id="d8e61-254">Domínios associados herdados de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="d8e61-255">excludedDomains</span></span>|<span data-ttu-id="d8e61-256">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8e61-256">String collection</span></span>|<span data-ttu-id="d8e61-257">Domínios acessados pela Internet pública em vez de por meio de VPN, mesmo quando a VPN por aplicativo é ativada Herdada de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="d8e61-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="d8e61-259">Booleano</span><span class="sxs-lookup"><span data-stu-id="d8e61-259">Boolean</span></span>|<span data-ttu-id="d8e61-260">Alternar para impedir que o usuário desabilite a VPN automática no aplicativo Configurações Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-261">proxyServer</span><span class="sxs-lookup"><span data-stu-id="d8e61-261">proxyServer</span></span>|[<span data-ttu-id="d8e61-262">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="d8e61-262">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="d8e61-263">Servidor Proxy.</span><span class="sxs-lookup"><span data-stu-id="d8e61-263">Proxy Server.</span></span> <span data-ttu-id="d8e61-264">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-264">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d8e61-265">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="d8e61-265">optInToDeviceIdSharing</span></span>|<span data-ttu-id="d8e61-266">Booleano</span><span class="sxs-lookup"><span data-stu-id="d8e61-266">Boolean</span></span>|<span data-ttu-id="d8e61-267">Opt-In compartilhar a ID do dispositivo para clientes vpn de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="d8e61-267">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="d8e61-268">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8e61-268">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d8e61-269">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8e61-269">Response</span></span>
<span data-ttu-id="d8e61-270">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8e61-270">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8e61-271">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8e61-271">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8e61-272">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8e61-272">Request</span></span>
<span data-ttu-id="d8e61-273">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8e61-273">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2825

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
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="d8e61-274">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8e61-274">Response</span></span>
<span data-ttu-id="d8e61-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8e61-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2997

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
  "optInToDeviceIdSharing": true
}
```




