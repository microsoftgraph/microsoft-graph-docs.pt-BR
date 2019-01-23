---
title: Criar windows10VpnConfiguration
description: Crie um novo objeto de windows10VpnConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 72264db454928358068f31dc5a439a5e74ce1da6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412041"
---
# <a name="create-windows10vpnconfiguration"></a><span data-ttu-id="22a54-103">Criar windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="22a54-103">Create windows10VpnConfiguration</span></span>

> <span data-ttu-id="22a54-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="22a54-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="22a54-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="22a54-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22a54-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="22a54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22a54-107">Crie um novo objeto de [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="22a54-107">Create a new [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22a54-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22a54-108">Prerequisites</span></span>
<span data-ttu-id="22a54-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="22a54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="22a54-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22a54-111">Permission type</span></span>|<span data-ttu-id="22a54-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22a54-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22a54-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22a54-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22a54-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22a54-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22a54-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22a54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22a54-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22a54-116">Not supported.</span></span>|
|<span data-ttu-id="22a54-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22a54-117">Application</span></span>|<span data-ttu-id="22a54-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22a54-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22a54-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22a54-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="22a54-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22a54-120">Request headers</span></span>
|<span data-ttu-id="22a54-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22a54-121">Header</span></span>|<span data-ttu-id="22a54-122">Valor</span><span class="sxs-lookup"><span data-stu-id="22a54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22a54-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="22a54-123">Authorization</span></span>|<span data-ttu-id="22a54-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22a54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22a54-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22a54-125">Accept</span></span>|<span data-ttu-id="22a54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22a54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22a54-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22a54-127">Request body</span></span>
<span data-ttu-id="22a54-128">No corpo da solicitação, fornece uma representação JSON para o objeto windows10VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="22a54-128">In the request body, supply a JSON representation for the windows10VpnConfiguration object.</span></span>

<span data-ttu-id="22a54-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windows10VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="22a54-129">The following table shows the properties that are required when you create the windows10VpnConfiguration.</span></span>

|<span data-ttu-id="22a54-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22a54-130">Property</span></span>|<span data-ttu-id="22a54-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="22a54-131">Type</span></span>|<span data-ttu-id="22a54-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="22a54-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22a54-133">id</span><span class="sxs-lookup"><span data-stu-id="22a54-133">id</span></span>|<span data-ttu-id="22a54-134">String</span><span class="sxs-lookup"><span data-stu-id="22a54-134">String</span></span>|<span data-ttu-id="22a54-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="22a54-135">Key of the entity.</span></span> <span data-ttu-id="22a54-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a54-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a54-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22a54-137">lastModifiedDateTime</span></span>|<span data-ttu-id="22a54-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22a54-138">DateTimeOffset</span></span>|<span data-ttu-id="22a54-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="22a54-139">DateTime the object was last modified.</span></span> <span data-ttu-id="22a54-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a54-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a54-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="22a54-141">roleScopeTagIds</span></span>|<span data-ttu-id="22a54-142">String collection</span><span class="sxs-lookup"><span data-stu-id="22a54-142">String collection</span></span>|<span data-ttu-id="22a54-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="22a54-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="22a54-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a54-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a54-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="22a54-145">supportsScopeTags</span></span>|<span data-ttu-id="22a54-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="22a54-146">Boolean</span></span>|<span data-ttu-id="22a54-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="22a54-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="22a54-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="22a54-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="22a54-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="22a54-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="22a54-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22a54-150">This property is read-only.</span></span> <span data-ttu-id="22a54-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a54-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a54-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22a54-152">createdDateTime</span></span>|<span data-ttu-id="22a54-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22a54-153">DateTimeOffset</span></span>|<span data-ttu-id="22a54-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="22a54-154">DateTime the object was created.</span></span> <span data-ttu-id="22a54-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a54-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a54-156">description</span><span class="sxs-lookup"><span data-stu-id="22a54-156">description</span></span>|<span data-ttu-id="22a54-157">String</span><span class="sxs-lookup"><span data-stu-id="22a54-157">String</span></span>|<span data-ttu-id="22a54-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22a54-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="22a54-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a54-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a54-160">displayName</span><span class="sxs-lookup"><span data-stu-id="22a54-160">displayName</span></span>|<span data-ttu-id="22a54-161">String</span><span class="sxs-lookup"><span data-stu-id="22a54-161">String</span></span>|<span data-ttu-id="22a54-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22a54-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="22a54-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a54-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a54-164">version</span><span class="sxs-lookup"><span data-stu-id="22a54-164">version</span></span>|<span data-ttu-id="22a54-165">Int32</span><span class="sxs-lookup"><span data-stu-id="22a54-165">Int32</span></span>|<span data-ttu-id="22a54-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22a54-166">Version of the device configuration.</span></span> <span data-ttu-id="22a54-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a54-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a54-168">connectionName</span><span class="sxs-lookup"><span data-stu-id="22a54-168">connectionName</span></span>|<span data-ttu-id="22a54-169">String</span><span class="sxs-lookup"><span data-stu-id="22a54-169">String</span></span>|<span data-ttu-id="22a54-170">Nome da Conexão exibida para o usuário.</span><span class="sxs-lookup"><span data-stu-id="22a54-170">Connection name displayed to the user.</span></span> <span data-ttu-id="22a54-171">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a54-171">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="22a54-172">servidores</span><span class="sxs-lookup"><span data-stu-id="22a54-172">servers</span></span>|<span data-ttu-id="22a54-173">coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="22a54-173">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="22a54-174">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="22a54-174">List of VPN Servers on the network.</span></span> <span data-ttu-id="22a54-175">Verifique se os usuários finais podem acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="22a54-175">Make sure end users can access these network locations.</span></span> <span data-ttu-id="22a54-176">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="22a54-176">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="22a54-177">Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a54-177">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="22a54-178">customXml</span><span class="sxs-lookup"><span data-stu-id="22a54-178">customXml</span></span>|<span data-ttu-id="22a54-179">Binária</span><span class="sxs-lookup"><span data-stu-id="22a54-179">Binary</span></span>|<span data-ttu-id="22a54-180">Comandos XML personalizados que configura a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="22a54-180">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="22a54-181">(Array de byte codificado UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="22a54-181">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="22a54-182">profileTarget</span><span class="sxs-lookup"><span data-stu-id="22a54-182">profileTarget</span></span>|[<span data-ttu-id="22a54-183">windows10VpnProfileTarget</span><span class="sxs-lookup"><span data-stu-id="22a54-183">windows10VpnProfileTarget</span></span>](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|<span data-ttu-id="22a54-184">Tipo de perfil de destino.</span><span class="sxs-lookup"><span data-stu-id="22a54-184">Profile target type.</span></span> <span data-ttu-id="22a54-185">Os valores possíveis são: `user`, `device`, `autoPilotDevice`.</span><span class="sxs-lookup"><span data-stu-id="22a54-185">Possible values are: `user`, `device`, `autoPilotDevice`.</span></span>|
|<span data-ttu-id="22a54-186">connectionType</span><span class="sxs-lookup"><span data-stu-id="22a54-186">connectionType</span></span>|[<span data-ttu-id="22a54-187">windows10VpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="22a54-187">windows10VpnConnectionType</span></span>](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|<span data-ttu-id="22a54-188">Tipo de Conexão.</span><span class="sxs-lookup"><span data-stu-id="22a54-188">Connection type.</span></span> <span data-ttu-id="22a54-189">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="22a54-189">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `automatic`, `ikEv2`, `l2tp`, `pptp`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="22a54-190">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="22a54-190">enableSplitTunneling</span></span>|<span data-ttu-id="22a54-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="22a54-191">Boolean</span></span>|<span data-ttu-id="22a54-192">Habilite o túnel em divisão.</span><span class="sxs-lookup"><span data-stu-id="22a54-192">Enable split tunneling.</span></span>|
|<span data-ttu-id="22a54-193">enableAlwaysOn</span><span class="sxs-lookup"><span data-stu-id="22a54-193">enableAlwaysOn</span></span>|<span data-ttu-id="22a54-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="22a54-194">Boolean</span></span>|<span data-ttu-id="22a54-195">Habilite o modo Always On.</span><span class="sxs-lookup"><span data-stu-id="22a54-195">Enable Always On mode.</span></span>|
|<span data-ttu-id="22a54-196">enableDeviceTunnel</span><span class="sxs-lookup"><span data-stu-id="22a54-196">enableDeviceTunnel</span></span>|<span data-ttu-id="22a54-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="22a54-197">Boolean</span></span>|<span data-ttu-id="22a54-198">Habilite o túnel de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22a54-198">Enable device tunnel.</span></span>|
|<span data-ttu-id="22a54-199">enableDnsRegistration</span><span class="sxs-lookup"><span data-stu-id="22a54-199">enableDnsRegistration</span></span>|<span data-ttu-id="22a54-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="22a54-200">Boolean</span></span>|<span data-ttu-id="22a54-201">Habilite o registro de endereço IP com DNS interno.</span><span class="sxs-lookup"><span data-stu-id="22a54-201">Enable IP address registration with internal DNS.</span></span>|
|<span data-ttu-id="22a54-202">dnsSuffixes</span><span class="sxs-lookup"><span data-stu-id="22a54-202">dnsSuffixes</span></span>|<span data-ttu-id="22a54-203">String collection</span><span class="sxs-lookup"><span data-stu-id="22a54-203">String collection</span></span>|<span data-ttu-id="22a54-204">Especifica os sufixos DNS para adicionar à lista de pesquisa de DNS para rotear corretamente nomes curtos.</span><span class="sxs-lookup"><span data-stu-id="22a54-204">Specify DNS suffixes to add to the DNS search list to properly route short names.</span></span>|
|<span data-ttu-id="22a54-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="22a54-205">authenticationMethod</span></span>|[<span data-ttu-id="22a54-206">windows10VpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="22a54-206">windows10VpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|<span data-ttu-id="22a54-207">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="22a54-207">Authentication method.</span></span> <span data-ttu-id="22a54-208">Os valores possíveis são: `certificate`, `usernameAndPassword`, `customEapXml`.</span><span class="sxs-lookup"><span data-stu-id="22a54-208">Possible values are: `certificate`, `usernameAndPassword`, `customEapXml`.</span></span>|
|<span data-ttu-id="22a54-209">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="22a54-209">rememberUserCredentials</span></span>|<span data-ttu-id="22a54-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="22a54-210">Boolean</span></span>|<span data-ttu-id="22a54-211">Lembre-se as credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="22a54-211">Remember user credentials.</span></span>|
|<span data-ttu-id="22a54-212">enableConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="22a54-212">enableConditionalAccess</span></span>|<span data-ttu-id="22a54-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="22a54-213">Boolean</span></span>|<span data-ttu-id="22a54-214">Habilite o acesso condicional.</span><span class="sxs-lookup"><span data-stu-id="22a54-214">Enable conditional access.</span></span>|
|<span data-ttu-id="22a54-215">enableSingleSignOnWithAlternateCertificate</span><span class="sxs-lookup"><span data-stu-id="22a54-215">enableSingleSignOnWithAlternateCertificate</span></span>|<span data-ttu-id="22a54-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="22a54-216">Boolean</span></span>|<span data-ttu-id="22a54-217">Habilite logon único (SSO) com o certificado alternativo.</span><span class="sxs-lookup"><span data-stu-id="22a54-217">Enable single sign-on (SSO) with alternate certificate.</span></span>|
|<span data-ttu-id="22a54-218">singleSignOnEku</span><span class="sxs-lookup"><span data-stu-id="22a54-218">singleSignOnEku</span></span>|[<span data-ttu-id="22a54-219">extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="22a54-219">extendedKeyUsage</span></span>](../resources/intune-deviceconfig-extendedkeyusage.md)|<span data-ttu-id="22a54-220">Single sign-on chave EKU (uso estendido).</span><span class="sxs-lookup"><span data-stu-id="22a54-220">Single sign-on Extended Key Usage (EKU).</span></span>|
|<span data-ttu-id="22a54-221">singleSignOnIssuerHash</span><span class="sxs-lookup"><span data-stu-id="22a54-221">singleSignOnIssuerHash</span></span>|<span data-ttu-id="22a54-222">String</span><span class="sxs-lookup"><span data-stu-id="22a54-222">String</span></span>|<span data-ttu-id="22a54-223">Hash de emissor de logon único.</span><span class="sxs-lookup"><span data-stu-id="22a54-223">Single sign-on issuer hash.</span></span>|
|<span data-ttu-id="22a54-224">eapXml</span><span class="sxs-lookup"><span data-stu-id="22a54-224">eapXml</span></span>|<span data-ttu-id="22a54-225">Binária</span><span class="sxs-lookup"><span data-stu-id="22a54-225">Binary</span></span>|<span data-ttu-id="22a54-226">Protocolo de autenticação extensível (EAP) XML.</span><span class="sxs-lookup"><span data-stu-id="22a54-226">Extensible Authentication Protocol (EAP) XML.</span></span> <span data-ttu-id="22a54-227">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="22a54-227">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="22a54-228">proxyServer</span><span class="sxs-lookup"><span data-stu-id="22a54-228">proxyServer</span></span>|[<span data-ttu-id="22a54-229">windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="22a54-229">windows10VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|<span data-ttu-id="22a54-230">Servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="22a54-230">Proxy Server.</span></span>|
|<span data-ttu-id="22a54-231">associatedApps</span><span class="sxs-lookup"><span data-stu-id="22a54-231">associatedApps</span></span>|<span data-ttu-id="22a54-232">coleção [windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)</span><span class="sxs-lookup"><span data-stu-id="22a54-232">[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md) collection</span></span>|<span data-ttu-id="22a54-233">Aplicativos associados.</span><span class="sxs-lookup"><span data-stu-id="22a54-233">Associated Apps.</span></span> <span data-ttu-id="22a54-234">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="22a54-234">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="22a54-235">onlyAssociatedAppsCanUseConnection</span><span class="sxs-lookup"><span data-stu-id="22a54-235">onlyAssociatedAppsCanUseConnection</span></span>|<span data-ttu-id="22a54-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="22a54-236">Boolean</span></span>|<span data-ttu-id="22a54-237">Apenas os aplicativos associados podem usar a conexão (-app VPN).</span><span class="sxs-lookup"><span data-stu-id="22a54-237">Only associated Apps can use connection (per-app VPN).</span></span>|
|<span data-ttu-id="22a54-238">windowsInformationProtectionDomain</span><span class="sxs-lookup"><span data-stu-id="22a54-238">windowsInformationProtectionDomain</span></span>|<span data-ttu-id="22a54-239">String</span><span class="sxs-lookup"><span data-stu-id="22a54-239">String</span></span>|<span data-ttu-id="22a54-240">Domínio de proteção de informações do Windows (WIP) para associar a essa conexão.</span><span class="sxs-lookup"><span data-stu-id="22a54-240">Windows Information Protection (WIP) domain to associate with this connection.</span></span>|
|<span data-ttu-id="22a54-241">trafficRules</span><span class="sxs-lookup"><span data-stu-id="22a54-241">trafficRules</span></span>|<span data-ttu-id="22a54-242">coleção [vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)</span><span class="sxs-lookup"><span data-stu-id="22a54-242">[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md) collection</span></span>|<span data-ttu-id="22a54-243">Regras de tráfego.</span><span class="sxs-lookup"><span data-stu-id="22a54-243">Traffic rules.</span></span> <span data-ttu-id="22a54-244">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="22a54-244">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="22a54-245">rotas</span><span class="sxs-lookup"><span data-stu-id="22a54-245">routes</span></span>|<span data-ttu-id="22a54-246">coleção [vpnRoute](../resources/intune-deviceconfig-vpnroute.md)</span><span class="sxs-lookup"><span data-stu-id="22a54-246">[vpnRoute](../resources/intune-deviceconfig-vpnroute.md) collection</span></span>|<span data-ttu-id="22a54-247">Roteia (opcional para provedores de terceiros).</span><span class="sxs-lookup"><span data-stu-id="22a54-247">Routes (optional for third-party providers).</span></span> <span data-ttu-id="22a54-248">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="22a54-248">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="22a54-249">dnsRules</span><span class="sxs-lookup"><span data-stu-id="22a54-249">dnsRules</span></span>|<span data-ttu-id="22a54-250">coleção [vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)</span><span class="sxs-lookup"><span data-stu-id="22a54-250">[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md) collection</span></span>|<span data-ttu-id="22a54-251">Regras DNS.</span><span class="sxs-lookup"><span data-stu-id="22a54-251">DNS rules.</span></span> <span data-ttu-id="22a54-252">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="22a54-252">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="22a54-253">trustedNetworkDomains</span><span class="sxs-lookup"><span data-stu-id="22a54-253">trustedNetworkDomains</span></span>|<span data-ttu-id="22a54-254">String collection</span><span class="sxs-lookup"><span data-stu-id="22a54-254">String collection</span></span>|<span data-ttu-id="22a54-255">Domínios de rede de perímetro</span><span class="sxs-lookup"><span data-stu-id="22a54-255">Trusted Network Domains</span></span>|



## <a name="response"></a><span data-ttu-id="22a54-256">Resposta</span><span class="sxs-lookup"><span data-stu-id="22a54-256">Response</span></span>
<span data-ttu-id="22a54-257">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22a54-257">If successful, this method returns a `201 Created` response code and a [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22a54-258">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22a54-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="22a54-259">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22a54-259">Request</span></span>
<span data-ttu-id="22a54-260">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22a54-260">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3387

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="22a54-261">Resposta</span><span class="sxs-lookup"><span data-stu-id="22a54-261">Response</span></span>
<span data-ttu-id="22a54-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22a54-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3559

{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
  "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
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
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "profileTarget": "device",
  "connectionType": "f5EdgeClient",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "Dns Suffixes value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "Name value",
    "objectIdentifier": "Object Identifier value"
  },
  "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
  "eapXml": "ZWFwWG1s",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "universal",
      "identifier": "Identifier value"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "Name value",
      "protocols": 9,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 11,
          "upperNumber": 11
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "appId": "App Id value",
      "appType": "desktop",
      "routingPolicyType": "splitTunnel",
      "claims": "Claims value"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "Destination Prefix value",
      "prefixSize": 10
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "Name value",
      "servers": [
        "Servers value"
      ],
      "proxyServerUri": "Proxy Server Uri value",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "Trusted Network Domains value"
  ]
}
```




