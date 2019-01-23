---
title: Criar macOSVpnConfiguration
description: Crie um novo objeto de macOSVpnConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2c8e2aefb0aa7bfc3a73ac83d32823d9c3c44a3b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416010"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="2f92e-103">Criar macOSVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f92e-103">Create macOSVpnConfiguration</span></span>

> <span data-ttu-id="2f92e-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2f92e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2f92e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2f92e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f92e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2f92e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f92e-107">Crie um novo objeto de [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2f92e-107">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f92e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f92e-108">Prerequisites</span></span>
<span data-ttu-id="2f92e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f92e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2f92e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f92e-111">Permission type</span></span>|<span data-ttu-id="2f92e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f92e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f92e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f92e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f92e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f92e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f92e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f92e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f92e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f92e-116">Not supported.</span></span>|
|<span data-ttu-id="2f92e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f92e-117">Application</span></span>|<span data-ttu-id="2f92e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f92e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f92e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f92e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2f92e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f92e-120">Request headers</span></span>
|<span data-ttu-id="2f92e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f92e-121">Header</span></span>|<span data-ttu-id="2f92e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2f92e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f92e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f92e-123">Authorization</span></span>|<span data-ttu-id="2f92e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f92e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f92e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f92e-125">Accept</span></span>|<span data-ttu-id="2f92e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f92e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f92e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f92e-127">Request body</span></span>
<span data-ttu-id="2f92e-128">No corpo da solicitação, fornece uma representação JSON para o objeto macOSVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2f92e-128">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="2f92e-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o macOSVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2f92e-129">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="2f92e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f92e-130">Property</span></span>|<span data-ttu-id="2f92e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f92e-131">Type</span></span>|<span data-ttu-id="2f92e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f92e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f92e-133">id</span><span class="sxs-lookup"><span data-stu-id="2f92e-133">id</span></span>|<span data-ttu-id="2f92e-134">String</span><span class="sxs-lookup"><span data-stu-id="2f92e-134">String</span></span>|<span data-ttu-id="2f92e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2f92e-135">Key of the entity.</span></span> <span data-ttu-id="2f92e-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f92e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2f92e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f92e-138">DateTimeOffset</span></span>|<span data-ttu-id="2f92e-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2f92e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2f92e-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2f92e-141">roleScopeTagIds</span></span>|<span data-ttu-id="2f92e-142">String collection</span><span class="sxs-lookup"><span data-stu-id="2f92e-142">String collection</span></span>|<span data-ttu-id="2f92e-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="2f92e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2f92e-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2f92e-145">supportsScopeTags</span></span>|<span data-ttu-id="2f92e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f92e-146">Boolean</span></span>|<span data-ttu-id="2f92e-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="2f92e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2f92e-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="2f92e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2f92e-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="2f92e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2f92e-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f92e-150">This property is read-only.</span></span> <span data-ttu-id="2f92e-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f92e-152">createdDateTime</span></span>|<span data-ttu-id="2f92e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f92e-153">DateTimeOffset</span></span>|<span data-ttu-id="2f92e-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2f92e-154">DateTime the object was created.</span></span> <span data-ttu-id="2f92e-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-156">description</span><span class="sxs-lookup"><span data-stu-id="2f92e-156">description</span></span>|<span data-ttu-id="2f92e-157">String</span><span class="sxs-lookup"><span data-stu-id="2f92e-157">String</span></span>|<span data-ttu-id="2f92e-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f92e-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2f92e-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2f92e-160">displayName</span></span>|<span data-ttu-id="2f92e-161">String</span><span class="sxs-lookup"><span data-stu-id="2f92e-161">String</span></span>|<span data-ttu-id="2f92e-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f92e-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2f92e-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-164">version</span><span class="sxs-lookup"><span data-stu-id="2f92e-164">version</span></span>|<span data-ttu-id="2f92e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2f92e-165">Int32</span></span>|<span data-ttu-id="2f92e-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f92e-166">Version of the device configuration.</span></span> <span data-ttu-id="2f92e-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="2f92e-168">connectionName</span></span>|<span data-ttu-id="2f92e-169">String</span><span class="sxs-lookup"><span data-stu-id="2f92e-169">String</span></span>|<span data-ttu-id="2f92e-170">Nome da Conexão exibida para o usuário.</span><span class="sxs-lookup"><span data-stu-id="2f92e-170">Connection name displayed to the user.</span></span> <span data-ttu-id="2f92e-171">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-171">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-172">connectionType</span><span class="sxs-lookup"><span data-stu-id="2f92e-172">connectionType</span></span>|[<span data-ttu-id="2f92e-173">appleVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="2f92e-173">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="2f92e-174">Tipo de Conexão.</span><span class="sxs-lookup"><span data-stu-id="2f92e-174">Connection type.</span></span> <span data-ttu-id="2f92e-175">Herdada do [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f92e-175">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="2f92e-176">Os valores possíveis são: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span><span class="sxs-lookup"><span data-stu-id="2f92e-176">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="2f92e-177">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="2f92e-177">loginGroupOrDomain</span></span>|<span data-ttu-id="2f92e-178">String</span><span class="sxs-lookup"><span data-stu-id="2f92e-178">String</span></span>|<span data-ttu-id="2f92e-179">Grupo de login ou domínio quando o tipo de conexão está definida como Dell SonicWALL Mobile Conexão.</span><span class="sxs-lookup"><span data-stu-id="2f92e-179">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="2f92e-180">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-180">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-181">role</span><span class="sxs-lookup"><span data-stu-id="2f92e-181">role</span></span>|<span data-ttu-id="2f92e-182">String</span><span class="sxs-lookup"><span data-stu-id="2f92e-182">String</span></span>|<span data-ttu-id="2f92e-183">Função quando o tipo de conexão está definida como pulso seguro.</span><span class="sxs-lookup"><span data-stu-id="2f92e-183">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="2f92e-184">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-184">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-185">território</span><span class="sxs-lookup"><span data-stu-id="2f92e-185">realm</span></span>|<span data-ttu-id="2f92e-186">String</span><span class="sxs-lookup"><span data-stu-id="2f92e-186">String</span></span>|<span data-ttu-id="2f92e-187">Território quando o tipo de conexão está definida como pulso seguro.</span><span class="sxs-lookup"><span data-stu-id="2f92e-187">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="2f92e-188">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-188">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-189">servidor</span><span class="sxs-lookup"><span data-stu-id="2f92e-189">server</span></span>|[<span data-ttu-id="2f92e-190">vpnServer</span><span class="sxs-lookup"><span data-stu-id="2f92e-190">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="2f92e-191">Servidor VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="2f92e-191">VPN Server on the network.</span></span> <span data-ttu-id="2f92e-192">Verifique se os usuários finais podem acessar esse local de rede.</span><span class="sxs-lookup"><span data-stu-id="2f92e-192">Make sure end users can access this network location.</span></span> <span data-ttu-id="2f92e-193">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-193">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-194">identificador</span><span class="sxs-lookup"><span data-stu-id="2f92e-194">identifier</span></span>|<span data-ttu-id="2f92e-195">String</span><span class="sxs-lookup"><span data-stu-id="2f92e-195">String</span></span>|<span data-ttu-id="2f92e-196">Identificador fornecido pelo fornecedor VPN quando o tipo de conexão está definida como Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="2f92e-196">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2f92e-197">Por exemplo: AnyConnect do Cisco usa um identificador do formulário de com.cisco.anyconnect.applevpn.plugin Inherited de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-197">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-198">customData</span><span class="sxs-lookup"><span data-stu-id="2f92e-198">customData</span></span>|<span data-ttu-id="2f92e-199">coleção [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-199">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="2f92e-200">Dados personalizados quando o tipo de conexão está definida como Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="2f92e-200">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2f92e-201">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="2f92e-201">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="2f92e-202">Entre em contato com seu fornecedor VPN para aprender como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="2f92e-202">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="2f92e-203">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="2f92e-203">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="2f92e-204">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-205">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="2f92e-205">customKeyValueData</span></span>|<span data-ttu-id="2f92e-206">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-206">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="2f92e-207">Dados personalizados quando o tipo de conexão está definida como Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="2f92e-207">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="2f92e-208">Use este campo para habilitar a funcionalidade não suportada pelo Intune, mas disponível em sua solução VPN.</span><span class="sxs-lookup"><span data-stu-id="2f92e-208">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="2f92e-209">Entre em contato com seu fornecedor VPN para aprender como adicionar esses pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="2f92e-209">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="2f92e-210">Essa coleção pode conter um máximo de 25 elementos.</span><span class="sxs-lookup"><span data-stu-id="2f92e-210">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="2f92e-211">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-211">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-212">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="2f92e-212">enableSplitTunneling</span></span>|<span data-ttu-id="2f92e-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f92e-213">Boolean</span></span>|<span data-ttu-id="2f92e-214">Envie todo o tráfego de rede por meio da VPN.</span><span class="sxs-lookup"><span data-stu-id="2f92e-214">Send all network traffic through VPN.</span></span> <span data-ttu-id="2f92e-215">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-216">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2f92e-216">authenticationMethod</span></span>|[<span data-ttu-id="2f92e-217">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2f92e-217">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="2f92e-218">Método de autenticação para essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="2f92e-218">Authentication method for this VPN connection.</span></span> <span data-ttu-id="2f92e-219">Herdada do [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2f92e-219">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="2f92e-220">Os valores possíveis são: `certificate` e `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="2f92e-220">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="2f92e-221">enablePerApp</span><span class="sxs-lookup"><span data-stu-id="2f92e-221">enablePerApp</span></span>|<span data-ttu-id="2f92e-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f92e-222">Boolean</span></span>|<span data-ttu-id="2f92e-223">Essa configuração como true cria a carga de VPN-App que posteriormente pode ser associada aos aplicativos que podem disparar a esta conexão VPN no dispositivo de iOS do usuário final.</span><span class="sxs-lookup"><span data-stu-id="2f92e-223">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="2f92e-224">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-224">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-225">safariDomains</span><span class="sxs-lookup"><span data-stu-id="2f92e-225">safariDomains</span></span>|<span data-ttu-id="2f92e-226">String collection</span><span class="sxs-lookup"><span data-stu-id="2f92e-226">String collection</span></span>|<span data-ttu-id="2f92e-227">Domínios do Safari quando este VPN por configuração de App está habilitado.</span><span class="sxs-lookup"><span data-stu-id="2f92e-227">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="2f92e-228">Além de aplicativos associados a este VPN, domínios Safari especificado aqui também poderão acionar essa conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="2f92e-228">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="2f92e-229">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-229">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-230">onDemandRules</span><span class="sxs-lookup"><span data-stu-id="2f92e-230">onDemandRules</span></span>|<span data-ttu-id="2f92e-231">coleção [vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-231">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="2f92e-232">Regras de sob demanda.</span><span class="sxs-lookup"><span data-stu-id="2f92e-232">On-Demand Rules.</span></span> <span data-ttu-id="2f92e-233">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="2f92e-233">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="2f92e-234">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-234">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-235">proxyServer</span><span class="sxs-lookup"><span data-stu-id="2f92e-235">proxyServer</span></span>|[<span data-ttu-id="2f92e-236">vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="2f92e-236">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="2f92e-237">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="2f92e-237">Proxy Server.</span></span> <span data-ttu-id="2f92e-238">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-238">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="2f92e-239">optInToDeviceIdSharing</span><span class="sxs-lookup"><span data-stu-id="2f92e-239">optInToDeviceIdSharing</span></span>|<span data-ttu-id="2f92e-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f92e-240">Boolean</span></span>|<span data-ttu-id="2f92e-241">Opt-In de compartilhamento de Id do dispositivo para clientes de vpn de terceiros para uso durante a validação de controle de acesso de rede.</span><span class="sxs-lookup"><span data-stu-id="2f92e-241">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="2f92e-242">Herdado de [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f92e-242">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2f92e-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f92e-243">Response</span></span>
<span data-ttu-id="2f92e-244">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f92e-244">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f92e-245">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f92e-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f92e-246">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f92e-246">Request</span></span>
<span data-ttu-id="2f92e-247">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f92e-247">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="2f92e-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f92e-248">Response</span></span>
<span data-ttu-id="2f92e-p127">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f92e-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




