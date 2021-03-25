---
title: Criar windowsPhone81VpnConfiguration
description: Crie um novo objeto windowsPhone81VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7d4c1578dfa97cd73a22e72308a7eead0b43fd73
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150945"
---
# <a name="create-windowsphone81vpnconfiguration"></a><span data-ttu-id="b8b6f-103">Criar windowsPhone81VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="b8b6f-103">Create windowsPhone81VpnConfiguration</span></span>

<span data-ttu-id="b8b6f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8b6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b8b6f-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8b6f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8b6f-107">Crie um novo [objeto windowsPhone81VpnConfiguration.](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-107">Create a new [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8b6f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b8b6f-108">Prerequisites</span></span>
<span data-ttu-id="b8b6f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8b6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8b6f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8b6f-111">Permission type</span></span>|<span data-ttu-id="b8b6f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8b6f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b8b6f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8b6f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b8b6f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8b6f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-116">Not supported.</span></span>|
|<span data-ttu-id="b8b6f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8b6f-117">Application</span></span>|<span data-ttu-id="b8b6f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8b6f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8b6f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8b6f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b8b6f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8b6f-120">Request headers</span></span>
|<span data-ttu-id="b8b6f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8b6f-121">Header</span></span>|<span data-ttu-id="b8b6f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b8b6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8b6f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8b6f-123">Authorization</span></span>|<span data-ttu-id="b8b6f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8b6f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b8b6f-125">Accept</span></span>|<span data-ttu-id="b8b6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b8b6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8b6f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8b6f-127">Request body</span></span>
<span data-ttu-id="b8b6f-128">No corpo da solicitação, fornece uma representação JSON para o objeto windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-128">In the request body, supply a JSON representation for the windowsPhone81VpnConfiguration object.</span></span>

<span data-ttu-id="b8b6f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o windowsPhone81VpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-129">The following table shows the properties that are required when you create the windowsPhone81VpnConfiguration.</span></span>

|<span data-ttu-id="b8b6f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8b6f-130">Property</span></span>|<span data-ttu-id="b8b6f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8b6f-131">Type</span></span>|<span data-ttu-id="b8b6f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8b6f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8b6f-133">id</span><span class="sxs-lookup"><span data-stu-id="b8b6f-133">id</span></span>|<span data-ttu-id="b8b6f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8b6f-134">String</span></span>|<span data-ttu-id="b8b6f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-135">Key of the entity.</span></span> <span data-ttu-id="b8b6f-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8b6f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b8b6f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8b6f-138">DateTimeOffset</span></span>|<span data-ttu-id="b8b6f-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b8b6f-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b8b6f-141">roleScopeTagIds</span></span>|<span data-ttu-id="b8b6f-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8b6f-142">String collection</span></span>|<span data-ttu-id="b8b6f-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b8b6f-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b8b6f-145">supportsScopeTags</span></span>|<span data-ttu-id="b8b6f-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="b8b6f-146">Boolean</span></span>|<span data-ttu-id="b8b6f-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b8b6f-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b8b6f-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b8b6f-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-150">This property is read-only.</span></span> <span data-ttu-id="b8b6f-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b8b6f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b8b6f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b8b6f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b8b6f-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b8b6f-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b8b6f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b8b6f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b8b6f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b8b6f-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b8b6f-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b8b6f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b8b6f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b8b6f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b8b6f-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b8b6f-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8b6f-164">createdDateTime</span></span>|<span data-ttu-id="b8b6f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8b6f-165">DateTimeOffset</span></span>|<span data-ttu-id="b8b6f-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-166">DateTime the object was created.</span></span> <span data-ttu-id="b8b6f-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-168">descrição</span><span class="sxs-lookup"><span data-stu-id="b8b6f-168">description</span></span>|<span data-ttu-id="b8b6f-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8b6f-169">String</span></span>|<span data-ttu-id="b8b6f-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b8b6f-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b8b6f-172">displayName</span></span>|<span data-ttu-id="b8b6f-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8b6f-173">String</span></span>|<span data-ttu-id="b8b6f-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b8b6f-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-176">versão</span><span class="sxs-lookup"><span data-stu-id="b8b6f-176">version</span></span>|<span data-ttu-id="b8b6f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b8b6f-177">Int32</span></span>|<span data-ttu-id="b8b6f-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-178">Version of the device configuration.</span></span> <span data-ttu-id="b8b6f-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-180">connectionName</span><span class="sxs-lookup"><span data-stu-id="b8b6f-180">connectionName</span></span>|<span data-ttu-id="b8b6f-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8b6f-181">String</span></span>|<span data-ttu-id="b8b6f-182">Nome da conexão exibido ao usuário.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-182">Connection name displayed to the user.</span></span> <span data-ttu-id="b8b6f-183">Herdado do [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-183">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-184">servers</span><span class="sxs-lookup"><span data-stu-id="b8b6f-184">servers</span></span>|<span data-ttu-id="b8b6f-185">[Coleção vpnServer](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-185">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="b8b6f-186">Lista de servidores VPN na rede.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-186">List of VPN Servers on the network.</span></span> <span data-ttu-id="b8b6f-187">Certifique-se de que os usuários finais possam acessar esses locais de rede.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-187">Make sure end users can access these network locations.</span></span> <span data-ttu-id="b8b6f-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-188">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b8b6f-189">Herdado do [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-189">Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-190">customXml</span><span class="sxs-lookup"><span data-stu-id="b8b6f-190">customXml</span></span>|<span data-ttu-id="b8b6f-191">Binário</span><span class="sxs-lookup"><span data-stu-id="b8b6f-191">Binary</span></span>|<span data-ttu-id="b8b6f-192">Comandos XML personalizados que configuram a conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-192">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="b8b6f-193">(Matriz de byte codificado UTF8) Herdado do [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-193">(UTF8 encoded byte array) Inherited from [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-194">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="b8b6f-194">applyOnlyToWindows81</span></span>|<span data-ttu-id="b8b6f-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8b6f-195">Boolean</span></span>|<span data-ttu-id="b8b6f-196">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-196">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="b8b6f-197">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-197">This property is read-only.</span></span> <span data-ttu-id="b8b6f-198">Herdado do [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-198">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-199">connectionType</span><span class="sxs-lookup"><span data-stu-id="b8b6f-199">connectionType</span></span>|[<span data-ttu-id="b8b6f-200">windowsVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="b8b6f-200">windowsVpnConnectionType</span></span>](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|<span data-ttu-id="b8b6f-201">Tipo de conexão.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-201">Connection type.</span></span> <span data-ttu-id="b8b6f-202">Herdado [do windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b8b6f-202">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).</span></span> <span data-ttu-id="b8b6f-203">Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-203">Possible values are: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.</span></span>|
|<span data-ttu-id="b8b6f-204">loginGroupOrDomain</span><span class="sxs-lookup"><span data-stu-id="b8b6f-204">loginGroupOrDomain</span></span>|<span data-ttu-id="b8b6f-205">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8b6f-205">String</span></span>|<span data-ttu-id="b8b6f-206">Grupo de logon ou domínio quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-206">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="b8b6f-207">Herdado do [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-207">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-208">enableSplitTunneling</span><span class="sxs-lookup"><span data-stu-id="b8b6f-208">enableSplitTunneling</span></span>|<span data-ttu-id="b8b6f-209">Booleano</span><span class="sxs-lookup"><span data-stu-id="b8b6f-209">Boolean</span></span>|<span data-ttu-id="b8b6f-210">Habilitar o túnel dividido para a VPN.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-210">Enable split tunneling for the VPN.</span></span> <span data-ttu-id="b8b6f-211">Herdado do [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-211">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-212">proxyServer</span><span class="sxs-lookup"><span data-stu-id="b8b6f-212">proxyServer</span></span>|[<span data-ttu-id="b8b6f-213">windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="b8b6f-213">windows81VpnProxyServer</span></span>](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|<span data-ttu-id="b8b6f-214">Servidor Proxy.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-214">Proxy Server.</span></span> <span data-ttu-id="b8b6f-215">Herdado do [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b8b6f-215">Inherited from [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)</span></span>|
|<span data-ttu-id="b8b6f-216">bypassVpnOnCompanyWifi</span><span class="sxs-lookup"><span data-stu-id="b8b6f-216">bypassVpnOnCompanyWifi</span></span>|<span data-ttu-id="b8b6f-217">Booleano</span><span class="sxs-lookup"><span data-stu-id="b8b6f-217">Boolean</span></span>|<span data-ttu-id="b8b6f-218">Ignorar VPN no Wi-Fi da empresa.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-218">Bypass VPN on company Wi-Fi.</span></span>|
|<span data-ttu-id="b8b6f-219">bypassVpnOnHomeWifi</span><span class="sxs-lookup"><span data-stu-id="b8b6f-219">bypassVpnOnHomeWifi</span></span>|<span data-ttu-id="b8b6f-220">Booleano</span><span class="sxs-lookup"><span data-stu-id="b8b6f-220">Boolean</span></span>|<span data-ttu-id="b8b6f-221">Ignorar VPN no Wi-Fi 2.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-221">Bypass VPN on home Wi-Fi.</span></span>|
|<span data-ttu-id="b8b6f-222">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b8b6f-222">authenticationMethod</span></span>|[<span data-ttu-id="b8b6f-223">vpnAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b8b6f-223">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="b8b6f-224">Método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-224">Authentication method.</span></span> <span data-ttu-id="b8b6f-225">Os valores possíveis são: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-225">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`, `azureAD`.</span></span>|
|<span data-ttu-id="b8b6f-226">rememberUserCredentials</span><span class="sxs-lookup"><span data-stu-id="b8b6f-226">rememberUserCredentials</span></span>|<span data-ttu-id="b8b6f-227">Booleano</span><span class="sxs-lookup"><span data-stu-id="b8b6f-227">Boolean</span></span>|<span data-ttu-id="b8b6f-228">Lembre-se das credenciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-228">Remember user credentials.</span></span>|
|<span data-ttu-id="b8b6f-229">dnsSuffixSearchList</span><span class="sxs-lookup"><span data-stu-id="b8b6f-229">dnsSuffixSearchList</span></span>|<span data-ttu-id="b8b6f-230">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8b6f-230">String collection</span></span>|<span data-ttu-id="b8b6f-231">Lista de pesquisa de sufixo DNS.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-231">DNS suffix search list.</span></span>|



## <a name="response"></a><span data-ttu-id="b8b6f-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8b6f-232">Response</span></span>
<span data-ttu-id="b8b6f-233">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-233">If successful, this method returns a `201 Created` response code and a [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8b6f-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8b6f-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8b6f-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8b6f-235">Request</span></span>
<span data-ttu-id="b8b6f-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2016

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
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
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b8b6f-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8b6f-237">Response</span></span>
<span data-ttu-id="b8b6f-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8b6f-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2188

{
  "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
  "id": "7cecc0db-c0db-7cec-dbc0-ec7cdbc0ec7c",
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
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "customXml": "Y3VzdG9tWG1s",
  "applyOnlyToWindows81": true,
  "connectionType": "f5EdgeClient",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  },
  "bypassVpnOnCompanyWifi": true,
  "bypassVpnOnHomeWifi": true,
  "authenticationMethod": "usernameAndPassword",
  "rememberUserCredentials": true,
  "dnsSuffixSearchList": [
    "Dns Suffix Search List value"
  ]
}
```




