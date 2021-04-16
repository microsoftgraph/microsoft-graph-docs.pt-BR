---
title: Criar iosVpnConfiguration
description: Crie um novo objeto iosVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bbc488742cc0cb94ca27a3a03f43e3fc99d72434
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868236"
---
# <a name="create-iosvpnconfiguration"></a><span data-ttu-id="57ed2-103">Criar iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="57ed2-103">Create iosVpnConfiguration</span></span>

<span data-ttu-id="57ed2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57ed2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57ed2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57ed2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57ed2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57ed2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57ed2-107">Crie um novo [objeto iosVpnConfiguration.](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-107">Create a new [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57ed2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57ed2-108">Prerequisites</span></span>
<span data-ttu-id="57ed2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57ed2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57ed2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57ed2-111">Permission type</span></span>|<span data-ttu-id="57ed2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57ed2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57ed2-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57ed2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57ed2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57ed2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57ed2-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57ed2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57ed2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57ed2-116">Not supported.</span></span>|
|<span data-ttu-id="57ed2-117">Application</span><span class="sxs-lookup"><span data-stu-id="57ed2-117">Application</span></span>|<span data-ttu-id="57ed2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57ed2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57ed2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57ed2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="57ed2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57ed2-120">Request headers</span></span>
|<span data-ttu-id="57ed2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57ed2-121">Header</span></span>|<span data-ttu-id="57ed2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="57ed2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57ed2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="57ed2-123">Authorization</span></span>|<span data-ttu-id="57ed2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57ed2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57ed2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57ed2-125">Accept</span></span>|<span data-ttu-id="57ed2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57ed2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57ed2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57ed2-127">Request body</span></span>
<span data-ttu-id="57ed2-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="57ed2-128">In the request body, supply a JSON representation for the iosVpnConfiguration object.</span></span>

<span data-ttu-id="57ed2-129">A tabela a seguir mostra as propriedades necessárias ao criar o iosVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="57ed2-129">The following table shows the properties that are required when you create the iosVpnConfiguration.</span></span>

|<span data-ttu-id="57ed2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57ed2-130">Property</span></span>|<span data-ttu-id="57ed2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="57ed2-131">Type</span></span>|<span data-ttu-id="57ed2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="57ed2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57ed2-133">id</span><span class="sxs-lookup"><span data-stu-id="57ed2-133">id</span></span>|<span data-ttu-id="57ed2-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57ed2-134">String</span></span>|<span data-ttu-id="57ed2-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="57ed2-135">Key of the entity.</span></span> <span data-ttu-id="57ed2-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="57ed2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="57ed2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57ed2-138">DateTimeOffset</span></span>|<span data-ttu-id="57ed2-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="57ed2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="57ed2-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="57ed2-141">roleScopeTagIds</span></span>|<span data-ttu-id="57ed2-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="57ed2-142">String collection</span></span>|<span data-ttu-id="57ed2-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="57ed2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="57ed2-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="57ed2-145">supportsScopeTags</span></span>|<span data-ttu-id="57ed2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="57ed2-146">Boolean</span></span>|<span data-ttu-id="57ed2-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="57ed2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="57ed2-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="57ed2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="57ed2-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="57ed2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="57ed2-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="57ed2-150">This property is read-only.</span></span> <span data-ttu-id="57ed2-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="57ed2-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="57ed2-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="57ed2-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="57ed2-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="57ed2-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="57ed2-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="57ed2-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="57ed2-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="57ed2-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="57ed2-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="57ed2-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="57ed2-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="57ed2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="57ed2-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="57ed2-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="57ed2-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="57ed2-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="57ed2-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="57ed2-164">createdDateTime</span></span>|<span data-ttu-id="57ed2-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57ed2-165">DateTimeOffset</span></span>|<span data-ttu-id="57ed2-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="57ed2-166">DateTime the object was created.</span></span> <span data-ttu-id="57ed2-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-168">description</span><span class="sxs-lookup"><span data-stu-id="57ed2-168">description</span></span>|<span data-ttu-id="57ed2-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57ed2-169">String</span></span>|<span data-ttu-id="57ed2-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="57ed2-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="57ed2-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-172">displayName</span><span class="sxs-lookup"><span data-stu-id="57ed2-172">displayName</span></span>|<span data-ttu-id="57ed2-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57ed2-173">String</span></span>|<span data-ttu-id="57ed2-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="57ed2-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="57ed2-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-176">versão</span><span class="sxs-lookup"><span data-stu-id="57ed2-176">version</span></span>|<span data-ttu-id="57ed2-177">Int32</span><span class="sxs-lookup"><span data-stu-id="57ed2-177">Int32</span></span>|<span data-ttu-id="57ed2-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="57ed2-178">Version of the device configuration.</span></span> <span data-ttu-id="57ed2-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="57ed2-180">connectionName</span></span>|<span data-ttu-id="57ed2-181">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="57ed2-181">String</span></span>|<span data-ttu-id="57ed2-182">Nome da conexão exibido ao usuário.</span><span class="sxs-lookup"><span data-stu-id="57ed2-182">Connection name displayed to the user.</span></span> <span data-ttu-id="57ed2-183">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-184">connectionType</span><span class="sxs-lookup"><span data-stu-id="57ed2-184">connectionType</span></span>|[<span data-ttu-id="57ed2-185">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="57ed2-185">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="57ed2-186">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="57ed2-186">Connection type.</span></span> <span data-ttu-id="57ed2-187">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="57ed2-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="57ed2-188">Os valores possíveis são: `ciscoAnyConnect` , , , , , , , , , `pulseSecure` , , , , `f5EdgeClient` , , , `dellSonicWallMobileConnect` , `checkPointCapsuleVpn` `customVpn` , `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `paloAltoGlobalProtect` `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2` `ikEv2` `alwaysOn` `microsoftTunnel` . `netMotionMobility` `microsoftProtect`</span><span class="sxs-lookup"><span data-stu-id="57ed2-188">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`, `microsoftTunnel`, `netMotionMobility`, `microsoftProtect`.</span></span>|
|<span data-ttu-id="57ed2-189">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="57ed2-189">loginGroupOrDomain</span></span>|<span data-ttu-id="57ed2-190">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="57ed2-190">String</span></span>|<span data-ttu-id="57ed2-191">Grupo de logon ou domínio quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="57ed2-191">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="57ed2-192">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-193">role</span><span class="sxs-lookup"><span data-stu-id="57ed2-193">role</span></span>|<span data-ttu-id="57ed2-194">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="57ed2-194">String</span></span>|<span data-ttu-id="57ed2-195">Função quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="57ed2-195">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="57ed2-196">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-196">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-197">realm</span><span class="sxs-lookup"><span data-stu-id="57ed2-197">realm</span></span>|<span data-ttu-id="57ed2-198">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="57ed2-198">String</span></span>|<span data-ttu-id="57ed2-199">Realm quando o tipo de conexão é definido como Pulse Secure.</span><span class="sxs-lookup"><span data-stu-id="57ed2-199">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="57ed2-200">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-200">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-201">server</span><span class="sxs-lookup"><span data-stu-id="57ed2-201">server</span></span>|[<span data-ttu-id="57ed2-202">vpnServer</span><span class="sxs-lookup"><span data-stu-id="57ed2-202">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="57ed2-203">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="57ed2-203">VPN Server on the network.</span></span> <span data-ttu-id="57ed2-204">Certifique-se de que os usuários finais possam acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="57ed2-204">Make sure end users can access this network location.</span></span> <span data-ttu-id="57ed2-205">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-205">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-206">identificador</span><span class="sxs-lookup"><span data-stu-id="57ed2-206">identifier</span></span>|<span data-ttu-id="57ed2-207">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="57ed2-207">String</span></span>|<span data-ttu-id="57ed2-208">Identificador fornecido pelo fornecedor vpn quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="57ed2-208">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="57ed2-209">Por exemplo: Cisco AnyConnect usa um identificador do formulário com.cisco.anyconnect.applevpn.plugin Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-209">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-210">customData</span><span class="sxs-lookup"><span data-stu-id="57ed2-210">customData</span></span>|<span data-ttu-id="57ed2-211">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-211">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="57ed2-212">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="57ed2-212">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="57ed2-213">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="57ed2-213">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="57ed2-214">Entre em contato com seu fornecedor vpn para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="57ed2-214">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="57ed2-215">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="57ed2-215">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="57ed2-216">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-216">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-217">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="57ed2-217">customKeyValueData</span></span>|<span data-ttu-id="57ed2-218">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-218">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="57ed2-219">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="57ed2-219">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="57ed2-220">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="57ed2-220">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="57ed2-221">Entre em contato com seu fornecedor vpn para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="57ed2-221">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="57ed2-222">Essa coleção pode conter no máximo 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="57ed2-222">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="57ed2-223">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-224">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="57ed2-224">enableSplitTunneling</span></span>|<span data-ttu-id="57ed2-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="57ed2-225">Boolean</span></span>|<span data-ttu-id="57ed2-226">Envie todo o tráfego de rede por meio de VPN.</span><span class="sxs-lookup"><span data-stu-id="57ed2-226">Send all network traffic through VPN.</span></span> <span data-ttu-id="57ed2-227">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-227">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-228">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="57ed2-228">authenticationMethod</span></span>|[<span data-ttu-id="57ed2-229">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="57ed2-229">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="57ed2-230">Método de autenticação para essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="57ed2-230">Authentication method for this VPN connection.</span></span> <span data-ttu-id="57ed2-231">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="57ed2-231">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="57ed2-232">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="57ed2-232">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="57ed2-233">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="57ed2-233">enablePerApp</span></span>|<span data-ttu-id="57ed2-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="57ed2-234">Boolean</span></span>|<span data-ttu-id="57ed2-235">Definir isso como Per-App true cria uma carga VPN que pode ser associada posteriormente a Aplicativos que podem disparar esse conneciton VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="57ed2-235">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="57ed2-236">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-236">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-237">safariDomains</span><span class="sxs-lookup"><span data-stu-id="57ed2-237">safariDomains</span></span>|<span data-ttu-id="57ed2-238">Coleção String</span><span class="sxs-lookup"><span data-stu-id="57ed2-238">String collection</span></span>|<span data-ttu-id="57ed2-239">Domínios safari quando essa configuração VPN por aplicativo está habilitada.</span><span class="sxs-lookup"><span data-stu-id="57ed2-239">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="57ed2-240">Além dos aplicativos associados a essa VPN, os domínios do Safari especificados aqui também poderão disparar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="57ed2-240">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="57ed2-241">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-242">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="57ed2-242">onDemandRules</span></span>|<span data-ttu-id="57ed2-243">[Coleção vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-243">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="57ed2-244">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="57ed2-244">On-Demand Rules.</span></span> <span data-ttu-id="57ed2-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="57ed2-245">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="57ed2-246">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-246">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-247">providerType</span><span class="sxs-lookup"><span data-stu-id="57ed2-247">providerType</span></span>|[<span data-ttu-id="57ed2-248">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="57ed2-248">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="57ed2-249">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="57ed2-249">Provider type for per-app VPN.</span></span> <span data-ttu-id="57ed2-250">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="57ed2-250">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="57ed2-251">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="57ed2-251">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="57ed2-252">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="57ed2-252">associatedDomains</span></span>|<span data-ttu-id="57ed2-253">Coleção String</span><span class="sxs-lookup"><span data-stu-id="57ed2-253">String collection</span></span>|<span data-ttu-id="57ed2-254">Domínios associados herdados de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-254">Associated Domains Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-255">excludedDomains</span><span class="sxs-lookup"><span data-stu-id="57ed2-255">excludedDomains</span></span>|<span data-ttu-id="57ed2-256">Coleção String</span><span class="sxs-lookup"><span data-stu-id="57ed2-256">String collection</span></span>|<span data-ttu-id="57ed2-257">Domínios acessados pela Internet pública em vez de por meio de VPN, mesmo quando a VPN por aplicativo é ativada Herdada de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-257">Domains that are accessed through the public internet instead of through VPN, even when per-app VPN is activated Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-258">disableOnDemandUserOverride</span><span class="sxs-lookup"><span data-stu-id="57ed2-258">disableOnDemandUserOverride</span></span>|<span data-ttu-id="57ed2-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="57ed2-259">Boolean</span></span>|<span data-ttu-id="57ed2-260">Alternar para impedir que o usuário desabilite a VPN automática no aplicativo Configurações Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-260">Toggle to prevent user from disabling automatic VPN in the Settings app Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-261">disconnectOnIdle</span><span class="sxs-lookup"><span data-stu-id="57ed2-261">disconnectOnIdle</span></span>|<span data-ttu-id="57ed2-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="57ed2-262">Boolean</span></span>|<span data-ttu-id="57ed2-263">Se deve desconectar após ociosos de conexão sob demanda Herdados de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-263">Whether to disconnect after on-demand connection idles Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-264">disconnectOnIdleTimerInSeconds</span><span class="sxs-lookup"><span data-stu-id="57ed2-264">disconnectOnIdleTimerInSeconds</span></span>|<span data-ttu-id="57ed2-265">Int32</span><span class="sxs-lookup"><span data-stu-id="57ed2-265">Int32</span></span>|<span data-ttu-id="57ed2-266">O tempo de espera em segundos antes de desconectar uma conexão sob demanda.</span><span class="sxs-lookup"><span data-stu-id="57ed2-266">The length of time in seconds to wait before disconnecting an on-demand connection.</span></span> <span data-ttu-id="57ed2-267">Valores válidos de 0 a 65535 Herdados [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-267">Valid values 0 to 65535 Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-268">proxyServer</span><span class="sxs-lookup"><span data-stu-id="57ed2-268">proxyServer</span></span>|[<span data-ttu-id="57ed2-269">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="57ed2-269">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="57ed2-270">Servidor Proxy.</span><span class="sxs-lookup"><span data-stu-id="57ed2-270">Proxy Server.</span></span> <span data-ttu-id="57ed2-271">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-271">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-272">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="57ed2-272">optInToDeviceIdSharing</span></span>|<span data-ttu-id="57ed2-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="57ed2-273">Boolean</span></span>|<span data-ttu-id="57ed2-274">Opt-In compartilhar a ID do dispositivo para clientes vpn de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="57ed2-274">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="57ed2-275">Herdado [de appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-275">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="57ed2-276">userDomain</span><span class="sxs-lookup"><span data-stu-id="57ed2-276">userDomain</span></span>|<span data-ttu-id="57ed2-277">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="57ed2-277">String</span></span>|<span data-ttu-id="57ed2-278">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="57ed2-278">Zscaler only.</span></span> <span data-ttu-id="57ed2-279">Insira um domínio estático para preencher previamente o campo de logon com no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="57ed2-279">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="57ed2-280">Se isso for deixado em branco, o domínio do Azure Active Directory do usuário será usado em vez disso.</span><span class="sxs-lookup"><span data-stu-id="57ed2-280">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="57ed2-281">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="57ed2-281">strictEnforcement</span></span>|<span data-ttu-id="57ed2-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="57ed2-282">Boolean</span></span>|<span data-ttu-id="57ed2-283">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="57ed2-283">Zscaler only.</span></span> <span data-ttu-id="57ed2-284">Bloqueia o tráfego de rede até que o usuário entre no aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="57ed2-284">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="57ed2-285">"True" significa que o tráfego está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="57ed2-285">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="57ed2-286">cloudName</span><span class="sxs-lookup"><span data-stu-id="57ed2-286">cloudName</span></span>|<span data-ttu-id="57ed2-287">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="57ed2-287">String</span></span>|<span data-ttu-id="57ed2-288">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="57ed2-288">Zscaler only.</span></span> <span data-ttu-id="57ed2-289">Nuvem Zscaler à qual o usuário é atribuído.</span><span class="sxs-lookup"><span data-stu-id="57ed2-289">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="57ed2-290">excludeList</span><span class="sxs-lookup"><span data-stu-id="57ed2-290">excludeList</span></span>|<span data-ttu-id="57ed2-291">Coleção String</span><span class="sxs-lookup"><span data-stu-id="57ed2-291">String collection</span></span>|<span data-ttu-id="57ed2-292">Somente Zscaler.</span><span class="sxs-lookup"><span data-stu-id="57ed2-292">Zscaler only.</span></span> <span data-ttu-id="57ed2-293">Lista de endereços de rede que não são enviados pela nuvem Zscaler.</span><span class="sxs-lookup"><span data-stu-id="57ed2-293">List of network addresses which are not sent through the Zscaler cloud.</span></span>|
|<span data-ttu-id="57ed2-294">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="57ed2-294">targetedMobileApps</span></span>|<span data-ttu-id="57ed2-295">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="57ed2-295">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="57ed2-296">Aplicativos móveis direcionados.</span><span class="sxs-lookup"><span data-stu-id="57ed2-296">Targeted mobile apps.</span></span> <span data-ttu-id="57ed2-297">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="57ed2-297">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="57ed2-298">microsoftTunnelSiteId</span><span class="sxs-lookup"><span data-stu-id="57ed2-298">microsoftTunnelSiteId</span></span>|<span data-ttu-id="57ed2-299">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="57ed2-299">String</span></span>|<span data-ttu-id="57ed2-300">ID do site do Túnel da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="57ed2-300">Microsoft Tunnel site ID.</span></span>|



## <a name="response"></a><span data-ttu-id="57ed2-301">Resposta</span><span class="sxs-lookup"><span data-stu-id="57ed2-301">Response</span></span>
<span data-ttu-id="57ed2-302">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57ed2-302">If successful, this method returns a `201 Created` response code and a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57ed2-303">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57ed2-303">Example</span></span>

### <a name="request"></a><span data-ttu-id="57ed2-304">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57ed2-304">Request</span></span>
<span data-ttu-id="57ed2-305">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57ed2-305">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3368

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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```

### <a name="response"></a><span data-ttu-id="57ed2-306">Resposta</span><span class="sxs-lookup"><span data-stu-id="57ed2-306">Response</span></span>
<span data-ttu-id="57ed2-p136">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57ed2-p136">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3540

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
  "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
}
```




