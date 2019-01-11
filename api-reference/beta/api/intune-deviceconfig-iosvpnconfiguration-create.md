---
title: Criar iosVpnConfiguration
description: Crie um novo objeto de iosVpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9276c36cdc281c7b535ef71e97a407b7848655ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819121"
---
# <a name="create-iosvpnconfiguration"></a><span data-ttu-id="09313-103">Criar iosVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="09313-103">Create iosVpnConfiguration</span></span>

> <span data-ttu-id="09313-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="09313-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09313-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="09313-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09313-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="09313-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09313-107">Crie um novo objeto de [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="09313-107">Create a new [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="09313-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="09313-108">Prerequisites</span></span>
<span data-ttu-id="09313-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09313-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09313-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09313-111">Permission type</span></span>|<span data-ttu-id="09313-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="09313-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09313-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09313-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09313-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09313-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09313-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09313-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09313-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09313-116">Not supported.</span></span>|
|<span data-ttu-id="09313-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09313-117">Application</span></span>|<span data-ttu-id="09313-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09313-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09313-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09313-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="09313-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09313-120">Request headers</span></span>
|<span data-ttu-id="09313-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="09313-121">Header</span></span>|<span data-ttu-id="09313-122">Valor</span><span class="sxs-lookup"><span data-stu-id="09313-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09313-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="09313-123">Authorization</span></span>|<span data-ttu-id="09313-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09313-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09313-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="09313-125">Accept</span></span>|<span data-ttu-id="09313-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09313-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09313-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09313-127">Request body</span></span>
<span data-ttu-id="09313-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="09313-128">In the request body, supply a JSON representation for the iosVpnConfiguration object.</span></span>

<span data-ttu-id="09313-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="09313-129">The following table shows the properties that are required when you create the iosVpnConfiguration.</span></span>

|<span data-ttu-id="09313-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09313-130">Property</span></span>|<span data-ttu-id="09313-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="09313-131">Type</span></span>|<span data-ttu-id="09313-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="09313-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09313-133">id</span><span class="sxs-lookup"><span data-stu-id="09313-133">id</span></span>|<span data-ttu-id="09313-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09313-134">String</span></span>|<span data-ttu-id="09313-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="09313-135">Key of the entity.</span></span> <span data-ttu-id="09313-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09313-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09313-137">lastModifiedDateTime</span></span>|<span data-ttu-id="09313-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09313-138">DateTimeOffset</span></span>|<span data-ttu-id="09313-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="09313-139">DateTime the object was last modified.</span></span> <span data-ttu-id="09313-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09313-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="09313-141">roleScopeTagIds</span></span>|<span data-ttu-id="09313-142">String collection</span><span class="sxs-lookup"><span data-stu-id="09313-142">String collection</span></span>|<span data-ttu-id="09313-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="09313-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="09313-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09313-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="09313-145">supportsScopeTags</span></span>|<span data-ttu-id="09313-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="09313-146">Boolean</span></span>|<span data-ttu-id="09313-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="09313-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="09313-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="09313-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="09313-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="09313-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="09313-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="09313-150">This property is read-only.</span></span> <span data-ttu-id="09313-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09313-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09313-152">createdDateTime</span></span>|<span data-ttu-id="09313-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09313-153">DateTimeOffset</span></span>|<span data-ttu-id="09313-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="09313-154">DateTime the object was created.</span></span> <span data-ttu-id="09313-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09313-156">description</span><span class="sxs-lookup"><span data-stu-id="09313-156">description</span></span>|<span data-ttu-id="09313-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09313-157">String</span></span>|<span data-ttu-id="09313-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="09313-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="09313-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09313-160">displayName</span><span class="sxs-lookup"><span data-stu-id="09313-160">displayName</span></span>|<span data-ttu-id="09313-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09313-161">String</span></span>|<span data-ttu-id="09313-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="09313-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="09313-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09313-164">version</span><span class="sxs-lookup"><span data-stu-id="09313-164">version</span></span>|<span data-ttu-id="09313-165">Int32</span><span class="sxs-lookup"><span data-stu-id="09313-165">Int32</span></span>|<span data-ttu-id="09313-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="09313-166">Version of the device configuration.</span></span> <span data-ttu-id="09313-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="09313-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="09313-168">connectionName</span></span>|<span data-ttu-id="09313-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09313-169">String</span></span>|<span data-ttu-id="09313-170">Nome da Conexão exibida para o usuário.</span><span class="sxs-lookup"><span data-stu-id="09313-170">Connection name displayed to the user.</span></span> <span data-ttu-id="09313-171">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-171">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="09313-172">connectionType</span><span class="sxs-lookup"><span data-stu-id="09313-172">connectionType</span></span>|[<span data-ttu-id="09313-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="09313-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="09313-174">Tipo de Conexão.</span><span class="sxs-lookup"><span data-stu-id="09313-174">Connection type.</span></span> <span data-ttu-id="09313-175">Herdada do [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09313-175">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="09313-176">Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="09313-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="09313-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="09313-177">loginGroupOrDomain</span></span>|<span data-ttu-id="09313-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09313-178">String</span></span>|<span data-ttu-id="09313-179">Grupo de login ou domínio quando o tipo de conexão está definida como Dell SonicWALL Mobile Conexão.</span><span class="sxs-lookup"><span data-stu-id="09313-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="09313-180">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-180">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="09313-181">role</span><span class="sxs-lookup"><span data-stu-id="09313-181">role</span></span>|<span data-ttu-id="09313-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09313-182">String</span></span>|<span data-ttu-id="09313-183">Função quando o tipo de conexão está definida como pulso seguro.</span><span class="sxs-lookup"><span data-stu-id="09313-183">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="09313-184">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-184">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="09313-185">território</span><span class="sxs-lookup"><span data-stu-id="09313-185">realm</span></span>|<span data-ttu-id="09313-186">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09313-186">String</span></span>|<span data-ttu-id="09313-187">Território quando o tipo de conexão está definida como pulso seguro.</span><span class="sxs-lookup"><span data-stu-id="09313-187">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="09313-188">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-188">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="09313-189">servidor</span><span class="sxs-lookup"><span data-stu-id="09313-189">server</span></span>|[<span data-ttu-id="09313-190">vpnServer</span><span class="sxs-lookup"><span data-stu-id="09313-190">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="09313-191">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="09313-191">VPN Server on the network.</span></span> <span data-ttu-id="09313-192">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="09313-192">Make sure end users can access this network location.</span></span> <span data-ttu-id="09313-193">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-193">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="09313-194">identificador</span><span class="sxs-lookup"><span data-stu-id="09313-194">identifier</span></span>|<span data-ttu-id="09313-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09313-195">String</span></span>|<span data-ttu-id="09313-196">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão está definida como Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="09313-196">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="09313-197">Por exemplo: AnyConnect do Cisco usa um identificador do formulário de com.cisco.anyconnect.applevpn.plugin Inherited de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-197">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="09313-198">customData</span><span class="sxs-lookup"><span data-stu-id="09313-198">customData</span></span>|<span data-ttu-id="09313-199">coleção [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="09313-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="09313-200">Dados personalizados quando o tipo de conexão está definida como Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="09313-200">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="09313-201">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="09313-201">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="09313-202">Entre em contato com seu fornecedor VPN para aprender como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="09313-202">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="09313-203">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="09313-203">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="09313-204">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="09313-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="09313-205">customKeyValueData</span></span>|<span data-ttu-id="09313-206">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="09313-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="09313-207">Dados personalizados quando o tipo de conexão está definida como Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="09313-207">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="09313-208">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="09313-208">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="09313-209">Entre em contato com seu fornecedor VPN para aprender como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="09313-209">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="09313-210">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="09313-210">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="09313-211">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-211">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="09313-212">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="09313-212">enableSplitTunneling</span></span>|<span data-ttu-id="09313-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="09313-213">Boolean</span></span>|<span data-ttu-id="09313-214">Envie todo o tráfego de rede por meio da VPN.</span><span class="sxs-lookup"><span data-stu-id="09313-214">Send all network traffic through VPN.</span></span> <span data-ttu-id="09313-215">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="09313-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="09313-216">authenticationMethod</span></span>|[<span data-ttu-id="09313-217">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="09313-217">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="09313-218">Método de autenticação para essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="09313-218">Authentication method for this VPN connection.</span></span> <span data-ttu-id="09313-219">Herdada do [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="09313-219">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="09313-220">Os valores possíveis são: `certificate` e `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="09313-220">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="09313-221">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="09313-221">enablePerApp</span></span>|<span data-ttu-id="09313-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="09313-222">Boolean</span></span>|<span data-ttu-id="09313-223">Essa configuração como true cria a carga de VPN-App que posteriormente pode ser associada aos aplicativos que podem disparar a esta conexão VPN no dispositivo de iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="09313-223">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="09313-224">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-224">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="09313-225">safariDomains</span><span class="sxs-lookup"><span data-stu-id="09313-225">safariDomains</span></span>|<span data-ttu-id="09313-226">String collection</span><span class="sxs-lookup"><span data-stu-id="09313-226">String collection</span></span>|<span data-ttu-id="09313-227">Domínios do Safari quando este VPN por configuração de App está habilitado.</span><span class="sxs-lookup"><span data-stu-id="09313-227">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="09313-228">Além de aplicativos associados a este VPN, domínios Safari especificado aqui também poderão acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="09313-228">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="09313-229">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-229">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="09313-230">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="09313-230">onDemandRules</span></span>|<span data-ttu-id="09313-231">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="09313-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="09313-232">Regras de sob demanda.</span><span class="sxs-lookup"><span data-stu-id="09313-232">On-Demand Rules.</span></span> <span data-ttu-id="09313-233">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="09313-233">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="09313-234">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-234">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="09313-235">proxyServer</span><span class="sxs-lookup"><span data-stu-id="09313-235">proxyServer</span></span>|[<span data-ttu-id="09313-236">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="09313-236">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="09313-237">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="09313-237">Proxy Server.</span></span> <span data-ttu-id="09313-238">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-238">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="09313-239">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="09313-239">optInToDeviceIdSharing</span></span>|<span data-ttu-id="09313-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="09313-240">Boolean</span></span>|<span data-ttu-id="09313-241">Opt-In de compartilhamento de Id do dispositivo para clientes de vpn de terceiros para uso durante a validação de controle de acesso de rede.</span><span class="sxs-lookup"><span data-stu-id="09313-241">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="09313-242">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="09313-242">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="09313-243">providerType</span><span class="sxs-lookup"><span data-stu-id="09313-243">providerType</span></span>|[<span data-ttu-id="09313-244">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="09313-244">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="09313-245">Tipo de provedor para VPN-app.</span><span class="sxs-lookup"><span data-stu-id="09313-245">Provider type for per-app VPN.</span></span> <span data-ttu-id="09313-246">Os valores possíveis são: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="09313-246">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="09313-247">userDomain</span><span class="sxs-lookup"><span data-stu-id="09313-247">userDomain</span></span>|<span data-ttu-id="09313-248">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09313-248">String</span></span>|<span data-ttu-id="09313-249">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="09313-249">Zscaler only.</span></span> <span data-ttu-id="09313-250">Digite um domínio estático para preencher previamente o campo de logon com o aplicativo Zscaler.</span><span class="sxs-lookup"><span data-stu-id="09313-250">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="09313-251">Se isso estiver vazio, domínio do Active Directory do Azure o usuário do será usado.</span><span class="sxs-lookup"><span data-stu-id="09313-251">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="09313-252">strictEnforcement</span><span class="sxs-lookup"><span data-stu-id="09313-252">strictEnforcement</span></span>|<span data-ttu-id="09313-253">Booliano</span><span class="sxs-lookup"><span data-stu-id="09313-253">Boolean</span></span>|<span data-ttu-id="09313-254">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="09313-254">Zscaler only.</span></span> <span data-ttu-id="09313-255">Bloqueia o tráfego de rede até que o usuário se conecta em Zscaler app.</span><span class="sxs-lookup"><span data-stu-id="09313-255">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="09313-256">"True" significa que o tráfego será bloqueado.</span><span class="sxs-lookup"><span data-stu-id="09313-256">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="09313-257">cloudName</span><span class="sxs-lookup"><span data-stu-id="09313-257">cloudName</span></span>|<span data-ttu-id="09313-258">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="09313-258">String</span></span>|<span data-ttu-id="09313-259">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="09313-259">Zscaler only.</span></span> <span data-ttu-id="09313-260">Nuvem de Zscaler que o usuário é atribuído.</span><span class="sxs-lookup"><span data-stu-id="09313-260">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="09313-261">excludeList</span><span class="sxs-lookup"><span data-stu-id="09313-261">excludeList</span></span>|<span data-ttu-id="09313-262">String collection</span><span class="sxs-lookup"><span data-stu-id="09313-262">String collection</span></span>|<span data-ttu-id="09313-263">Zscaler.</span><span class="sxs-lookup"><span data-stu-id="09313-263">Zscaler only.</span></span> <span data-ttu-id="09313-264">Lista de endereços de rede que não são enviados através da nuvem Zscaler.</span><span class="sxs-lookup"><span data-stu-id="09313-264">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="09313-265">Resposta</span><span class="sxs-lookup"><span data-stu-id="09313-265">Response</span></span>
<span data-ttu-id="09313-266">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09313-266">If successful, this method returns a `201 Created` response code and a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09313-267">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09313-267">Example</span></span>
### <a name="request"></a><span data-ttu-id="09313-268">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09313-268">Request</span></span>
<span data-ttu-id="09313-269">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09313-269">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2106

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="09313-270">Resposta</span><span class="sxs-lookup"><span data-stu-id="09313-270">Response</span></span>
<span data-ttu-id="09313-p132">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09313-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2214

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
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
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ]
}
```





