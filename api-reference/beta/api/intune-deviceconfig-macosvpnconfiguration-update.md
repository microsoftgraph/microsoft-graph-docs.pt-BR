---
title: Atualizar macOSVpnConfiguration
description: Atualiza as propriedades de um objeto macOSVpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73fecc7200c6172b8edd22922d9d4a573659b9a2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156109"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="85e1c-103">Atualizar macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="85e1c-103">Update macOSVpnConfiguration</span></span>

> <span data-ttu-id="85e1c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="85e1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85e1c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="85e1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85e1c-106">Atualiza as propriedades de um objeto [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="85e1c-106">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85e1c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="85e1c-107">Prerequisites</span></span>
<span data-ttu-id="85e1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="85e1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="85e1c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="85e1c-110">Permission type</span></span>|<span data-ttu-id="85e1c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="85e1c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85e1c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="85e1c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85e1c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85e1c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85e1c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="85e1c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85e1c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85e1c-115">Not supported.</span></span>|
|<span data-ttu-id="85e1c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="85e1c-116">Application</span></span>|<span data-ttu-id="85e1c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="85e1c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85e1c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="85e1c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="85e1c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="85e1c-119">Request headers</span></span>
|<span data-ttu-id="85e1c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="85e1c-120">Header</span></span>|<span data-ttu-id="85e1c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="85e1c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85e1c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="85e1c-122">Authorization</span></span>|<span data-ttu-id="85e1c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="85e1c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85e1c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="85e1c-124">Accept</span></span>|<span data-ttu-id="85e1c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85e1c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85e1c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="85e1c-126">Request body</span></span>
<span data-ttu-id="85e1c-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="85e1c-127">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="85e1c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85e1c-128">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="85e1c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85e1c-129">Property</span></span>|<span data-ttu-id="85e1c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="85e1c-130">Type</span></span>|<span data-ttu-id="85e1c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="85e1c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85e1c-132">id</span><span class="sxs-lookup"><span data-stu-id="85e1c-132">id</span></span>|<span data-ttu-id="85e1c-133">String</span><span class="sxs-lookup"><span data-stu-id="85e1c-133">String</span></span>|<span data-ttu-id="85e1c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="85e1c-134">Key of the entity.</span></span> <span data-ttu-id="85e1c-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85e1c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="85e1c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85e1c-137">DateTimeOffset</span></span>|<span data-ttu-id="85e1c-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="85e1c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="85e1c-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="85e1c-140">roleScopeTagIds</span></span>|<span data-ttu-id="85e1c-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="85e1c-141">String collection</span></span>|<span data-ttu-id="85e1c-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="85e1c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="85e1c-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="85e1c-144">supportsScopeTags</span></span>|<span data-ttu-id="85e1c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e1c-145">Boolean</span></span>|<span data-ttu-id="85e1c-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="85e1c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="85e1c-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="85e1c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="85e1c-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="85e1c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="85e1c-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85e1c-149">This property is read-only.</span></span> <span data-ttu-id="85e1c-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85e1c-151">createdDateTime</span></span>|<span data-ttu-id="85e1c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85e1c-152">DateTimeOffset</span></span>|<span data-ttu-id="85e1c-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="85e1c-153">DateTime the object was created.</span></span> <span data-ttu-id="85e1c-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-155">description</span><span class="sxs-lookup"><span data-stu-id="85e1c-155">description</span></span>|<span data-ttu-id="85e1c-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85e1c-156">String</span></span>|<span data-ttu-id="85e1c-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="85e1c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="85e1c-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="85e1c-159">displayName</span></span>|<span data-ttu-id="85e1c-160">String</span><span class="sxs-lookup"><span data-stu-id="85e1c-160">String</span></span>|<span data-ttu-id="85e1c-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="85e1c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="85e1c-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-163">version</span><span class="sxs-lookup"><span data-stu-id="85e1c-163">version</span></span>|<span data-ttu-id="85e1c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="85e1c-164">Int32</span></span>|<span data-ttu-id="85e1c-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="85e1c-165">Version of the device configuration.</span></span> <span data-ttu-id="85e1c-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-167">ConnectionName</span><span class="sxs-lookup"><span data-stu-id="85e1c-167">connectionName</span></span>|<span data-ttu-id="85e1c-168">String</span><span class="sxs-lookup"><span data-stu-id="85e1c-168">String</span></span>|<span data-ttu-id="85e1c-169">Nome da conexão exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="85e1c-169">Connection name displayed to the user.</span></span> <span data-ttu-id="85e1c-170">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-170">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-171">Connection</span><span class="sxs-lookup"><span data-stu-id="85e1c-171">connectionType</span></span>|[<span data-ttu-id="85e1c-172">Enumeraçãoapplevpnconnectiontype</span><span class="sxs-lookup"><span data-stu-id="85e1c-172">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="85e1c-173">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="85e1c-173">Connection type.</span></span> <span data-ttu-id="85e1c-174">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85e1c-174">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="85e1c-175">Os valores possíveis são `ciscoAnyConnect`: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`,.</span><span class="sxs-lookup"><span data-stu-id="85e1c-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="85e1c-176">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="85e1c-176">loginGroupOrDomain</span></span>|<span data-ttu-id="85e1c-177">String</span><span class="sxs-lookup"><span data-stu-id="85e1c-177">String</span></span>|<span data-ttu-id="85e1c-178">Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="85e1c-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="85e1c-179">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-179">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-180">role</span><span class="sxs-lookup"><span data-stu-id="85e1c-180">role</span></span>|<span data-ttu-id="85e1c-181">String</span><span class="sxs-lookup"><span data-stu-id="85e1c-181">String</span></span>|<span data-ttu-id="85e1c-182">Função quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="85e1c-182">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="85e1c-183">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-184">esfera</span><span class="sxs-lookup"><span data-stu-id="85e1c-184">realm</span></span>|<span data-ttu-id="85e1c-185">String</span><span class="sxs-lookup"><span data-stu-id="85e1c-185">String</span></span>|<span data-ttu-id="85e1c-186">O realm quando o tipo de conexão é definido como pulsar seguro.</span><span class="sxs-lookup"><span data-stu-id="85e1c-186">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="85e1c-187">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-188">do</span><span class="sxs-lookup"><span data-stu-id="85e1c-188">server</span></span>|[<span data-ttu-id="85e1c-189">vpnServer</span><span class="sxs-lookup"><span data-stu-id="85e1c-189">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="85e1c-190">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="85e1c-190">VPN Server on the network.</span></span> <span data-ttu-id="85e1c-191">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="85e1c-191">Make sure end users can access this network location.</span></span> <span data-ttu-id="85e1c-192">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-193">identificador</span><span class="sxs-lookup"><span data-stu-id="85e1c-193">identifier</span></span>|<span data-ttu-id="85e1c-194">String</span><span class="sxs-lookup"><span data-stu-id="85e1c-194">String</span></span>|<span data-ttu-id="85e1c-195">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="85e1c-195">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="85e1c-196">Por exemplo: o Cisco AnyConnect usa um identificador do formulário com. Cisco. AnyConnect. applevpn. plugin herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-196">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-197">customData</span><span class="sxs-lookup"><span data-stu-id="85e1c-197">customData</span></span>|<span data-ttu-id="85e1c-198">Coleção [KeyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="85e1c-199">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="85e1c-199">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="85e1c-200">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="85e1c-200">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="85e1c-201">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="85e1c-201">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="85e1c-202">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="85e1c-202">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="85e1c-203">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-203">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-204">Customkeyvaluedata foi adicionada</span><span class="sxs-lookup"><span data-stu-id="85e1c-204">customKeyValueData</span></span>|<span data-ttu-id="85e1c-205">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="85e1c-206">Dados personalizados quando o tipo de conexão é definido como VPN personalizada.</span><span class="sxs-lookup"><span data-stu-id="85e1c-206">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="85e1c-207">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="85e1c-207">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="85e1c-208">Entre em contato com seu fornecedor VPN para saber como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="85e1c-208">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="85e1c-209">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="85e1c-209">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="85e1c-210">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-210">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-211">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="85e1c-211">enableSplitTunneling</span></span>|<span data-ttu-id="85e1c-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e1c-212">Boolean</span></span>|<span data-ttu-id="85e1c-213">Enviar todo o tráfego de rede através da VPN.</span><span class="sxs-lookup"><span data-stu-id="85e1c-213">Send all network traffic through VPN.</span></span> <span data-ttu-id="85e1c-214">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-214">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-215">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="85e1c-215">authenticationMethod</span></span>|[<span data-ttu-id="85e1c-216">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="85e1c-216">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="85e1c-217">Método de autenticação para esta conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="85e1c-217">Authentication method for this VPN connection.</span></span> <span data-ttu-id="85e1c-218">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="85e1c-218">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="85e1c-219">Os valores possíveis são: `certificate` e `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="85e1c-219">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="85e1c-220">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="85e1c-220">enablePerApp</span></span>|<span data-ttu-id="85e1c-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e1c-221">Boolean</span></span>|<span data-ttu-id="85e1c-222">A configuração dessa opção como true cria uma carga de VPN por aplicativo, que pode ser mais tarde associada aos aplicativos que podem acionar esta conexão VPN no dispositivo iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="85e1c-222">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="85e1c-223">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-224">safariDomains</span><span class="sxs-lookup"><span data-stu-id="85e1c-224">safariDomains</span></span>|<span data-ttu-id="85e1c-225">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="85e1c-225">String collection</span></span>|<span data-ttu-id="85e1c-226">Domínios Safari quando esta configuração VPN por aplicativo estiver habilitada.</span><span class="sxs-lookup"><span data-stu-id="85e1c-226">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="85e1c-227">Além dos aplicativos associados a essa VPN, os domínios Safari especificados aqui também serão capazes de acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="85e1c-227">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="85e1c-228">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-228">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-229">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="85e1c-229">onDemandRules</span></span>|<span data-ttu-id="85e1c-230">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="85e1c-231">Regras sob demanda.</span><span class="sxs-lookup"><span data-stu-id="85e1c-231">On-Demand Rules.</span></span> <span data-ttu-id="85e1c-232">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="85e1c-232">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="85e1c-233">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-233">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-234">proxyServer</span><span class="sxs-lookup"><span data-stu-id="85e1c-234">proxyServer</span></span>|[<span data-ttu-id="85e1c-235">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="85e1c-235">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="85e1c-236">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="85e1c-236">Proxy Server.</span></span> <span data-ttu-id="85e1c-237">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-237">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="85e1c-238">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="85e1c-238">optInToDeviceIdSharing</span></span>|<span data-ttu-id="85e1c-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="85e1c-239">Boolean</span></span>|<span data-ttu-id="85e1c-240">Optar por compartilhar a ID do dispositivo para clientes VPN de terceiros para uso durante a validação do controle de acesso à rede.</span><span class="sxs-lookup"><span data-stu-id="85e1c-240">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="85e1c-241">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="85e1c-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="85e1c-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="85e1c-242">Response</span></span>
<span data-ttu-id="85e1c-243">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="85e1c-243">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85e1c-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="85e1c-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="85e1c-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="85e1c-245">Request</span></span>
<span data-ttu-id="85e1c-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="85e1c-246">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1857

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="85e1c-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="85e1c-247">Response</span></span>
<span data-ttu-id="85e1c-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="85e1c-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2029

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




