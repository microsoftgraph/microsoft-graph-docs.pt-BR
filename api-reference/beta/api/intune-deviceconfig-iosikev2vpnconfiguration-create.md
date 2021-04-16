---
title: Criar iosikEv2VpnConfiguration
description: Crie um novo objeto iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 46959bc18368658faff157cb592e8b23b505b70d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867215"
---
# <a name="create-iosikev2vpnconfiguration"></a><span data-ttu-id="d1bf8-103">Criar iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1bf8-103">Create iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="d1bf8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1bf8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1bf8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1bf8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1bf8-107">Crie um novo [objeto iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-107">Create a new [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1bf8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d1bf8-108">Prerequisites</span></span>
<span data-ttu-id="d1bf8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1bf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1bf8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1bf8-111">Permission type</span></span>|<span data-ttu-id="d1bf8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1bf8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d1bf8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1bf8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d1bf8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1bf8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-116">Not supported.</span></span>|
|<span data-ttu-id="d1bf8-117">Application</span><span class="sxs-lookup"><span data-stu-id="d1bf8-117">Application</span></span>|<span data-ttu-id="d1bf8-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1bf8-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1bf8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1bf8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d1bf8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1bf8-120">Request headers</span></span>
|<span data-ttu-id="d1bf8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1bf8-121">Header</span></span>|<span data-ttu-id="d1bf8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d1bf8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1bf8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1bf8-123">Authorization</span></span>|<span data-ttu-id="d1bf8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1bf8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d1bf8-125">Accept</span></span>|<span data-ttu-id="d1bf8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d1bf8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1bf8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1bf8-127">Request body</span></span>
<span data-ttu-id="d1bf8-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-128">In the request body, supply a JSON representation for the iosikEv2VpnConfiguration object.</span></span>

<span data-ttu-id="d1bf8-129">A tabela a seguir mostra as propriedades necessárias ao criar o iosikEv2VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-129">The following table shows the properties that are required when you create the iosikEv2VpnConfiguration.</span></span>

|<span data-ttu-id="d1bf8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1bf8-130">Property</span></span>|<span data-ttu-id="d1bf8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1bf8-131">Type</span></span>|<span data-ttu-id="d1bf8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1bf8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1bf8-133">id</span><span class="sxs-lookup"><span data-stu-id="d1bf8-133">id</span></span>|<span data-ttu-id="d1bf8-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-134">String</span></span>|<span data-ttu-id="d1bf8-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-135">Key of the entity.</span></span> <span data-ttu-id="d1bf8-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d1bf8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d1bf8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1bf8-138">DateTimeOffset</span></span>|<span data-ttu-id="d1bf8-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d1bf8-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d1bf8-141">roleScopeTagIds</span></span>|<span data-ttu-id="d1bf8-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d1bf8-142">String collection</span></span>|<span data-ttu-id="d1bf8-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d1bf8-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d1bf8-145">supportsScopeTags</span></span>|<span data-ttu-id="d1bf8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1bf8-146">Boolean</span></span>|<span data-ttu-id="d1bf8-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d1bf8-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d1bf8-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d1bf8-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-150">This property is read-only.</span></span> <span data-ttu-id="d1bf8-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d1bf8-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d1bf8-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d1bf8-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d1bf8-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d1bf8-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d1bf8-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d1bf8-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d1bf8-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d1bf8-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d1bf8-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d1bf8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d1bf8-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d1bf8-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d1bf8-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d1bf8-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d1bf8-164">createdDateTime</span></span>|<span data-ttu-id="d1bf8-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d1bf8-165">DateTimeOffset</span></span>|<span data-ttu-id="d1bf8-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-166">DateTime the object was created.</span></span> <span data-ttu-id="d1bf8-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-168">description</span><span class="sxs-lookup"><span data-stu-id="d1bf8-168">description</span></span>|<span data-ttu-id="d1bf8-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-169">String</span></span>|<span data-ttu-id="d1bf8-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d1bf8-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d1bf8-172">displayName</span></span>|<span data-ttu-id="d1bf8-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-173">String</span></span>|<span data-ttu-id="d1bf8-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d1bf8-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-176">versão</span><span class="sxs-lookup"><span data-stu-id="d1bf8-176">version</span></span>|<span data-ttu-id="d1bf8-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d1bf8-177">Int32</span></span>|<span data-ttu-id="d1bf8-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-178">Version of the device configuration.</span></span> <span data-ttu-id="d1bf8-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="d1bf8-180">connectionName</span></span>|<span data-ttu-id="d1bf8-181">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-181">String</span></span>|<span data-ttu-id="d1bf8-182">Nome da conexão exibido ao usuário.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-182">Connection name displayed to the user.</span></span> <span data-ttu-id="d1bf8-183">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="d1bf8-184">connectionType</span></span>|[<span data-ttu-id="d1bf8-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="d1bf8-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="d1bf8-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-186">Connection type.</span></span> <span data-ttu-id="d1bf8-187">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d1bf8-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="d1bf8-188">Os valores possíveis são: `ciscoAnyConnect` , , , , , , , , , `pulseSecure` , , , , `f5EdgeClient` , , , `dellSonicWallMobileConnect` , `checkPointCapsuleVpn` `customVpn` , `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` . `netMotionMobility` `microsoftProtect`</span><span class="sxs-lookup"><span data-stu-id="d1bf8-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="d1bf8-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="d1bf8-189">loginGroupOrDomain</span></span>|<span data-ttu-id="d1bf8-190">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-190">String</span></span>|<span data-ttu-id="d1bf8-191">Grupo de logon ou domínio quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="d1bf8-192">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-193">role</span><span class="sxs-lookup"><span data-stu-id="d1bf8-193">role</span></span>|<span data-ttu-id="d1bf8-194">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-194">String</span></span>|<span data-ttu-id="d1bf8-195">Função quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="d1bf8-196">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-197">realm</span><span class="sxs-lookup"><span data-stu-id="d1bf8-197">realm</span></span>|<span data-ttu-id="d1bf8-198">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-198">String</span></span>|<span data-ttu-id="d1bf8-199">Realm quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="d1bf8-200">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-201">server</span><span class="sxs-lookup"><span data-stu-id="d1bf8-201">server</span></span>|[<span data-ttu-id="d1bf8-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="d1bf8-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="d1bf8-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-203">VPN Server on the network.</span></span> <span data-ttu-id="d1bf8-204">Certifique-se de que os usuários finais possam acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="d1bf8-205">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-206">identificador</span><span class="sxs-lookup"><span data-stu-id="d1bf8-206">identifier</span></span>|<span data-ttu-id="d1bf8-207">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-207">String</span></span>|<span data-ttu-id="d1bf8-208">Identificador fornecido pelo fornecedor vpn quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="d1bf8-209">Por exemplo: Cisco AnyConnect usa um identificador do formulário com.cisco.anyconnect.applevpn.plugin Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-210">customData</span><span class="sxs-lookup"><span data-stu-id="d1bf8-210">customData</span></span>|<span data-ttu-id="d1bf8-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="d1bf8-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="d1bf8-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="d1bf8-214">Entre em contato com seu fornecedor vpn para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="d1bf8-215">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="d1bf8-216">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="d1bf8-217">customKeyValueData</span></span>|<span data-ttu-id="d1bf8-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="d1bf8-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="d1bf8-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="d1bf8-221">Entre em contato com seu fornecedor vpn para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="d1bf8-222">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="d1bf8-223">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="d1bf8-224">enableSplitTunneling</span></span>|<span data-ttu-id="d1bf8-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1bf8-225">Boolean</span></span>|<span data-ttu-id="d1bf8-226">Envie todo o tráfego de rede por meio de VPN.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="d1bf8-227">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d1bf8-228">authenticationMethod</span></span>|[<span data-ttu-id="d1bf8-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d1bf8-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="d1bf8-230">Método de autenticação para essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="d1bf8-231">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d1bf8-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="d1bf8-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="d1bf8-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="d1bf8-233">enablePerApp</span></span>|<span data-ttu-id="d1bf8-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1bf8-234">Boolean</span></span>|<span data-ttu-id="d1bf8-235">Definir isso como Per-App true cria uma carga VPN que pode ser associada posteriormente a Aplicativos que podem disparar esse conneciton VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="d1bf8-236">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="d1bf8-237">safariDomains</span></span>|<span data-ttu-id="d1bf8-238">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d1bf8-238">String collection</span></span>|<span data-ttu-id="d1bf8-239">Domínios safari quando essa configuração VPN por aplicativo está habilitada.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="d1bf8-240">Além dos aplicativos associados a essa VPN, os domínios do Safari especificados aqui também poderão disparar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="d1bf8-241">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="d1bf8-242">onDemandRules</span></span>|<span data-ttu-id="d1bf8-243">[Coleção vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="d1bf8-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-244">On-Demand Rules.</span></span> <span data-ttu-id="d1bf8-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d1bf8-246">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-247">providerType</span><span class="sxs-lookup"><span data-stu-id="d1bf8-247">providerType</span></span>|[<span data-ttu-id="d1bf8-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="d1bf8-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="d1bf8-249">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="d1bf8-250">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d1bf8-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="d1bf8-251">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="d1bf8-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="d1bf8-252">associatedDomains</span></span>|<span data-ttu-id="d1bf8-253">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d1bf8-253">String collection</span></span>|<span data-ttu-id="d1bf8-254">Domínios associados herdados de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="d1bf8-255">excludedDomains</span></span>|<span data-ttu-id="d1bf8-256">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d1bf8-256">String collection</span></span>|<span data-ttu-id="d1bf8-257">Domínios acessados pela Internet pública em vez de por meio de VPN, mesmo quando a VPN por aplicativo é ativada Herdada de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="d1bf8-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="d1bf8-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1bf8-259">Boolean</span></span>|<span data-ttu-id="d1bf8-260">Alternar para impedir que o usuário desabilite a VPN automática no aplicativo Configurações Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-261">disconnectOnIdle</span><span class="sxs-lookup"><span data-stu-id="d1bf8-261">disconnectOnIdle</span></span>|<span data-ttu-id="d1bf8-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1bf8-262">Boolean</span></span>|<span data-ttu-id="d1bf8-263">Se deve desconectar após ociosos de conexão sob demanda Herdados de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-263">Whether to disconnect after on-demand connection idles Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-264">disconnectOnIdleTimerInSeconds</span><span class="sxs-lookup"><span data-stu-id="d1bf8-264">disconnectOnIdleTimerInSeconds</span></span>|<span data-ttu-id="d1bf8-265">Int32</span><span class="sxs-lookup"><span data-stu-id="d1bf8-265">Int32</span></span>|<span data-ttu-id="d1bf8-266">O tempo de espera em segundos antes de desconectar uma conexão sob demanda.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-266">The length of time in seconds to wait before disconnecting an on-demand connection.</span></span> <span data-ttu-id="d1bf8-267">Valores válidos de 0 a 65535 Herdados [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-267">Valid values 0 to 65535 Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-268">proxyServer</span><span class="sxs-lookup"><span data-stu-id="d1bf8-268">proxyServer</span></span>|[<span data-ttu-id="d1bf8-269">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="d1bf8-269">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="d1bf8-270">Servidor Proxy.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-270">Proxy Server.</span></span> <span data-ttu-id="d1bf8-271">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-271">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-272">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="d1bf8-272">optInToDeviceIdSharing</span></span>|<span data-ttu-id="d1bf8-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1bf8-273">Boolean</span></span>|<span data-ttu-id="d1bf8-274">Opt-In compartilhar a ID do dispositivo para clientes vpn de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-274">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="d1bf8-275">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-275">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-276">userDomain</span><span class="sxs-lookup"><span data-stu-id="d1bf8-276">userDomain</span></span>|<span data-ttu-id="d1bf8-277">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-277">String</span></span>|<span data-ttu-id="d1bf8-278">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-278">Zscaler only.</span></span> <span data-ttu-id="d1bf8-279">Insira um domínio estático para preencher previamente o campo de logon com no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-279">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="d1bf8-280">Se isso for deixado em branco, o domínio do Azure Active Directory do usuário será usado em vez disso.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-280">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span> <span data-ttu-id="d1bf8-281">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-281">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-282">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="d1bf8-282">strictEnforcement</span></span>|<span data-ttu-id="d1bf8-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1bf8-283">Boolean</span></span>|<span data-ttu-id="d1bf8-284">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-284">Zscaler only.</span></span> <span data-ttu-id="d1bf8-285">Bloqueia o tráfego de rede até que o usuário entre no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-285">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="d1bf8-286">"True" significa que o tráfego está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-286">"True" means traffic is blocked.</span></span> <span data-ttu-id="d1bf8-287">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-287">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-288">cloudName</span><span class="sxs-lookup"><span data-stu-id="d1bf8-288">cloudName</span></span>|<span data-ttu-id="d1bf8-289">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-289">String</span></span>|<span data-ttu-id="d1bf8-290">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-290">Zscaler only.</span></span> <span data-ttu-id="d1bf8-291">Nuvem Zscaler à qual o usuário é atribuído.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-291">Zscaler cloud which the user is assigned to.</span></span> <span data-ttu-id="d1bf8-292">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-292">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-293">excludeList</span><span class="sxs-lookup"><span data-stu-id="d1bf8-293">excludeList</span></span>|<span data-ttu-id="d1bf8-294">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d1bf8-294">String collection</span></span>|<span data-ttu-id="d1bf8-295">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-295">Zscaler only.</span></span> <span data-ttu-id="d1bf8-296">Lista de endereços de rede que não são enviados pela nuvem Zscaler.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-296">List of network addresses which are not sent through the Zscaler cloud.</span></span> <span data-ttu-id="d1bf8-297">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-297">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-298">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="d1bf8-298">targetedMobileApps</span></span>|<span data-ttu-id="d1bf8-299">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-299">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d1bf8-300">Aplicativos móveis direcionados.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-300">Targeted mobile apps.</span></span> <span data-ttu-id="d1bf8-301">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-301">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d1bf8-302">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-302">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-303">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="d1bf8-303">microsoftTunnelSiteId</span></span>|<span data-ttu-id="d1bf8-304">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-304">String</span></span>|<span data-ttu-id="d1bf8-305">ID do site do Túnel da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-305">Microsoft Tunnel site ID.</span></span> <span data-ttu-id="d1bf8-306">Herdado [do iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d1bf8-306">Inherited from [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span></span>|
|<span data-ttu-id="d1bf8-307">childSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="d1bf8-307">childSecurityAssociationParameters</span></span>|[<span data-ttu-id="d1bf8-308">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="d1bf8-308">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="d1bf8-309">Parâmetros de associação de segurança filho</span><span class="sxs-lookup"><span data-stu-id="d1bf8-309">Child Security Association Parameters</span></span>|
|<span data-ttu-id="d1bf8-310">clientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="d1bf8-310">clientAuthenticationType</span></span>|[<span data-ttu-id="d1bf8-311">vpnClientAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="d1bf8-311">vpnClientAuthenticationType</span></span>](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|<span data-ttu-id="d1bf8-312">Tipo de Autenticação de Cliente que o cliente VPN usará.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-312">Type of Client Authentication the VPN client will use.</span></span> <span data-ttu-id="d1bf8-313">Os valores possíveis são: `userAuthentication` e `deviceAuthentication`.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-313">Possible values are: `userAuthentication`, `deviceAuthentication`.</span></span>|
|<span data-ttu-id="d1bf8-314">deadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="d1bf8-314">deadPeerDetectionRate</span></span>|[<span data-ttu-id="d1bf8-315">vpnDeadPeerDetectionRate</span><span class="sxs-lookup"><span data-stu-id="d1bf8-315">vpnDeadPeerDetectionRate</span></span>](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|<span data-ttu-id="d1bf8-316">Determine com que frequência verificar se uma conexão de par ainda está ativa.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-316">Determine how often to check if a peer connection is still active.</span></span> <span data-ttu-id="d1bf8-317">.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-317">.</span></span> <span data-ttu-id="d1bf8-318">Os valores possíveis são: `medium`, `none`, `low`, `high`.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-318">Possible values are: `medium`, `none`, `low`, `high`.</span></span>|
|<span data-ttu-id="d1bf8-319">disableMobilityAndMultihoming</span><span class="sxs-lookup"><span data-stu-id="d1bf8-319">disableMobilityAndMultihoming</span></span>|<span data-ttu-id="d1bf8-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1bf8-320">Boolean</span></span>|<span data-ttu-id="d1bf8-321">Desabilitar MOBIKE</span><span class="sxs-lookup"><span data-stu-id="d1bf8-321">Disable MOBIKE</span></span>|
|<span data-ttu-id="d1bf8-322">disableRedirect</span><span class="sxs-lookup"><span data-stu-id="d1bf8-322">disableRedirect</span></span>|<span data-ttu-id="d1bf8-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1bf8-323">Boolean</span></span>|<span data-ttu-id="d1bf8-324">Desabilitar Redirecionamento</span><span class="sxs-lookup"><span data-stu-id="d1bf8-324">Disable Redirect</span></span>|
|<span data-ttu-id="d1bf8-325">enableCertificateRevocationCheck</span><span class="sxs-lookup"><span data-stu-id="d1bf8-325">enableCertificateRevocationCheck</span></span>|<span data-ttu-id="d1bf8-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1bf8-326">Boolean</span></span>|<span data-ttu-id="d1bf8-327">Habilita uma verificação de revogação de melhor esforço; tempo-de-tempo de resposta do servidor não fará com que ele falhe</span><span class="sxs-lookup"><span data-stu-id="d1bf8-327">Enables a best-effort revocation check; server response timeouts will not cause it to fail</span></span>|
|<span data-ttu-id="d1bf8-328">enableEAP</span><span class="sxs-lookup"><span data-stu-id="d1bf8-328">enableEAP</span></span>|<span data-ttu-id="d1bf8-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1bf8-329">Boolean</span></span>|<span data-ttu-id="d1bf8-330">Habilita a autenticação somente EAP</span><span class="sxs-lookup"><span data-stu-id="d1bf8-330">Enables EAP only authentication</span></span>|
|<span data-ttu-id="d1bf8-331">enablePerfectForwardSecrecy</span><span class="sxs-lookup"><span data-stu-id="d1bf8-331">enablePerfectForwardSecrecy</span></span>|<span data-ttu-id="d1bf8-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1bf8-332">Boolean</span></span>|<span data-ttu-id="d1bf8-333">Habilitar o PFS (Segredo de Encaminhamento Perfeito).</span><span class="sxs-lookup"><span data-stu-id="d1bf8-333">Enable Perfect Forward Secrecy (PFS).</span></span>|
|<span data-ttu-id="d1bf8-334">enableUseInternalSubnetAttributes</span><span class="sxs-lookup"><span data-stu-id="d1bf8-334">enableUseInternalSubnetAttributes</span></span>|<span data-ttu-id="d1bf8-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1bf8-335">Boolean</span></span>|<span data-ttu-id="d1bf8-336">Habilitar usar atributos de sub-rede internas.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-336">Enable Use Internal Subnet Attributes.</span></span>|
|<span data-ttu-id="d1bf8-337">localIdentifier</span><span class="sxs-lookup"><span data-stu-id="d1bf8-337">localIdentifier</span></span>|[<span data-ttu-id="d1bf8-338">vpnLocalIdentifier</span><span class="sxs-lookup"><span data-stu-id="d1bf8-338">vpnLocalIdentifier</span></span>](../resources/intune-deviceconfig-vpnlocalidentifier.md)|<span data-ttu-id="d1bf8-339">Método de identificar o cliente que está tentando se conectar via VPN.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-339">Method of identifying the client that is trying to connect via VPN.</span></span> <span data-ttu-id="d1bf8-340">.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-340">.</span></span> <span data-ttu-id="d1bf8-341">Os valores possíveis são: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-341">Possible values are: `deviceFQDN`, `empty`, `clientCertificateSubjectName`.</span></span>|
|<span data-ttu-id="d1bf8-342">remoteIdentifier</span><span class="sxs-lookup"><span data-stu-id="d1bf8-342">remoteIdentifier</span></span>|<span data-ttu-id="d1bf8-343">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-343">String</span></span>|<span data-ttu-id="d1bf8-344">Endereço do servidor IKEv2.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-344">Address of the IKEv2 server.</span></span> <span data-ttu-id="d1bf8-345">Deve ser um FQDN, UserFQDN, endereço de rede ou ASN1DN</span><span class="sxs-lookup"><span data-stu-id="d1bf8-345">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|
|<span data-ttu-id="d1bf8-346">securityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="d1bf8-346">securityAssociationParameters</span></span>|[<span data-ttu-id="d1bf8-347">iosVpnSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="d1bf8-347">iosVpnSecurityAssociationParameters</span></span>](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|<span data-ttu-id="d1bf8-348">Parâmetros de Associação de Segurança</span><span class="sxs-lookup"><span data-stu-id="d1bf8-348">Security Association Parameters</span></span>|
|<span data-ttu-id="d1bf8-349">serverCertificateCommonName</span><span class="sxs-lookup"><span data-stu-id="d1bf8-349">serverCertificateCommonName</span></span>|<span data-ttu-id="d1bf8-350">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-350">String</span></span>|<span data-ttu-id="d1bf8-351">Nome comum do Certificado de Servidor IKEv2 usado na Autenticação do Servidor</span><span class="sxs-lookup"><span data-stu-id="d1bf8-351">Common name of the IKEv2 Server Certificate used in Server Authentication</span></span>|
|<span data-ttu-id="d1bf8-352">serverCertificateIssuerCommonName</span><span class="sxs-lookup"><span data-stu-id="d1bf8-352">serverCertificateIssuerCommonName</span></span>|<span data-ttu-id="d1bf8-353">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-353">String</span></span>|<span data-ttu-id="d1bf8-354">Nome comum do emissor do emissor de Certificado do Servidor IKEv2 usado na Autenticação</span><span class="sxs-lookup"><span data-stu-id="d1bf8-354">Issuer Common name of the IKEv2 Server Certificate issuer used in Authentication</span></span>|
|<span data-ttu-id="d1bf8-355">serverCertificateType</span><span class="sxs-lookup"><span data-stu-id="d1bf8-355">serverCertificateType</span></span>|[<span data-ttu-id="d1bf8-356">vpnServerCertificateType</span><span class="sxs-lookup"><span data-stu-id="d1bf8-356">vpnServerCertificateType</span></span>](../resources/intune-deviceconfig-vpnservercertificatetype.md)|<span data-ttu-id="d1bf8-357">O tipo de certificado que o servidor VPN apresentará ao cliente VPN para autenticação.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-357">The type of certificate the VPN server will present to the VPN client for authentication.</span></span> <span data-ttu-id="d1bf8-358">Os valores possíveis são: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-358">Possible values are: `rsa`, `ecdsa256`, `ecdsa384`, `ecdsa521`.</span></span>|
|<span data-ttu-id="d1bf8-359">sharedSecret</span><span class="sxs-lookup"><span data-stu-id="d1bf8-359">sharedSecret</span></span>|<span data-ttu-id="d1bf8-360">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-360">String</span></span>|<span data-ttu-id="d1bf8-361">Usado quando a Autenticação Secreta Compartilhada está selecionada</span><span class="sxs-lookup"><span data-stu-id="d1bf8-361">Used when Shared Secret Authentication is selected</span></span>|
|<span data-ttu-id="d1bf8-362">tlsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="d1bf8-362">tlsMaximumVersion</span></span>|<span data-ttu-id="d1bf8-363">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-363">String</span></span>|<span data-ttu-id="d1bf8-364">A versão TLS máxima a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="d1bf8-364">The maximum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="d1bf8-365">tlsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="d1bf8-365">tlsMinimumVersion</span></span>|<span data-ttu-id="d1bf8-366">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d1bf8-366">String</span></span>|<span data-ttu-id="d1bf8-367">A versão TLS mínima a ser usada com autenticação EAP-TLS</span><span class="sxs-lookup"><span data-stu-id="d1bf8-367">The minimum TLS version to be used with EAP-TLS authentication</span></span>|
|<span data-ttu-id="d1bf8-368">allowDefaultSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="d1bf8-368">allowDefaultSecurityAssociationParameters</span></span>|<span data-ttu-id="d1bf8-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1bf8-369">Boolean</span></span>|<span data-ttu-id="d1bf8-370">Permite o uso de parâmetros de associação de segurança definindo todos os parâmetros para o padrão do dispositivo, a menos que especificado explicitamente.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-370">Allows the use of security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="d1bf8-371">allowDefaultChildSecurityAssociationParameters</span><span class="sxs-lookup"><span data-stu-id="d1bf8-371">allowDefaultChildSecurityAssociationParameters</span></span>|<span data-ttu-id="d1bf8-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1bf8-372">Boolean</span></span>|<span data-ttu-id="d1bf8-373">Permite o uso de parâmetros de associação de segurança filho definindo todos os parâmetros para o padrão do dispositivo, a menos que especificado explicitamente.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-373">Allows the use of child security association parameters by setting all parameters to the device's default unless explicitly specified.</span></span>|
|<span data-ttu-id="d1bf8-374">alwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1bf8-374">alwaysOnConfiguration</span></span>|[<span data-ttu-id="d1bf8-375">appleVpnAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1bf8-375">appleVpnAlwaysOnConfiguration</span></span>](../resources/intune-deviceconfig-applevpnalwaysonconfiguration.md)|<span data-ttu-id="d1bf8-376">Configuração AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="d1bf8-376">AlwaysOn Configuration</span></span>|
|<span data-ttu-id="d1bf8-377">enableAlwaysOnConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1bf8-377">enableAlwaysOnConfiguration</span></span>|<span data-ttu-id="d1bf8-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1bf8-378">Boolean</span></span>|<span data-ttu-id="d1bf8-379">Determina se a VPN Always on está habilitada</span><span class="sxs-lookup"><span data-stu-id="d1bf8-379">Determines if Always on VPN is enabled</span></span>|
|<span data-ttu-id="d1bf8-380">mtuSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="d1bf8-380">mtuSizeInBytes</span></span>|<span data-ttu-id="d1bf8-381">Int32</span><span class="sxs-lookup"><span data-stu-id="d1bf8-381">Int32</span></span>|<span data-ttu-id="d1bf8-382">Unidade de transmissão máxima.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-382">Maximum transmission unit.</span></span> <span data-ttu-id="d1bf8-383">Valores válidos de 1280 a 1400</span><span class="sxs-lookup"><span data-stu-id="d1bf8-383">Valid values 1280 to 1400</span></span>|



## <a name="response"></a><span data-ttu-id="d1bf8-384">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1bf8-384">Response</span></span>
<span data-ttu-id="d1bf8-385">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-385">If successful, this method returns a `201 Created` response code and a [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1bf8-386">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1bf8-386">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1bf8-387">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1bf8-387">Request</span></span>
<span data-ttu-id="d1bf8-388">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-388">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="d1bf8-389">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1bf8-389">Response</span></span>
<span data-ttu-id="d1bf8-p143">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1bf8-p143">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




